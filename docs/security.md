---
tags: [documentation]
---

# Security

It's very important to secure your transaction so only the authorized party in your side that can do the transaction by API call. 

## Protect Your API Key

It's very important to keep your API key secret especially in production environment. When someone know your API key, there is a chance that they can call API to do transaction.

## Whitelist Your IP

In sandbox environment you don't need to whitelist IP but when it in production environment, you need to whitelist IP so our service can allow your account to do real transaction from your whitelist IP and deny outside whitelist IP.

![Whitelist IP](../assets/images/whitelist-ip.png)

<!-- theme: danger -->

> ### Watch Out!
> Actually you can allow transaction from any IP but if you use this option, any person from any IP can use your 
> account if they know your API KEY. We suggest you to use whitelist IP and input your IP for security reason.

## Callback Notification

### IAK Outgoing IP Address

IAK send request to your callback URL through IP address. In case you want to whitelist our IP please add below IP to your system.

<!--
type: tab
title: Sandbox
-->

```json
52.76.169.212
```

<!--
type: tab
title: Production
-->

```json
52.220.38.194
```

<!-- type: tab-end -->

### Authentication 

Our request body to your callback URL is contain field **sign** which you can use as authentication. The sign field is hashed with md5 with the combination below. 

<!--
title: "Authentication formula"
-->

```javascript
md5({username} + {api_key} + {ref_id})
```
