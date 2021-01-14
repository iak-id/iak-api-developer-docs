# Check Balance

![Check Balance](../../assets/images/checkbalance.png)

### Parameter

| Field    | Type     | Description                           |
| -------- | -------- | ------------------------------------- |
| commands | string   | balance                               |
| username | string   | Your Registered Phone Number          |
| sign     | string   | Signature - md5(username+api_key+"bl")|

```json json_schema
{
  "type": "object",
  "properties": {
    "commands": {
      "type": "string",
      "description": "balance",
      "default": "balance"
    },
    "username": {
      "type": "string",
      "description": "Your Registered Phone Number"
    },
    "sign": {
      "type": "string",
      "description": "md5(username+api_key+'bl')"
    }
  }
}
```

### Request

<!-- theme: warning -->

> ### Watch Out!
>
> You can only use **JSON** and **XML**!

<!--
type: tab
title: Request JSON
-->

```json
{
	"commands" : "balance",
	"username" : "087888067165",
	"sign"     : "51cf7677af84d08103400cf9abe208a7"
}
```

<!--
type: tab
title: Request XML
-->

```json
<?xml version="1.0" ?>
<mp>
    <commands>balance</commands>
    <username>087888067165</username>
    <sign>51cf7677af84d08103400cf9abe208a7</sign>
</mp>
```
<!-- type: tab-end -->

### Response Paramater

| Field    | Type     | Description |
| -------- | -------- | ----------- |
| balance  | Double   | Your Balance|


```json json_schema
{
  "type": "object",
  "properties": {
    "balance": {
      "type": "number"
    }
  }
}
```

### Success Response 

<!-- theme: success -->

> ### Success response!
>
> Here is success response!

```json
{
	"data": {
		"balance": 997136249
	}
}
```

### Testing

<!-- theme: info -->

> ### A thing to know
>
> You can testing development and production

<!--
type: tab
title: Development
-->

```json http
{
  "method": "post",
  "url": "https://testprepaid.mobilepulsa.net/v1/legacy/index"
}
```

<!--
type: tab
title: Production
-->

```json http
{
  "method": "post",
  "url": "https://mobilepulsa.net/v1/legacy/index"
}
```

<!-- type: tab-end -->
