# Check Balance

![Check Balance](../../assets/images/checkbalance.png)

### Parameter

| Field | Type | Description |
| -------- | -------- | -------- |
| A1       | B1       | C1       |
| A2       | B2       | C2       |
| A3       | B3       | C3       |


### Request

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

| Field | Type | Description |
| -------- | -------- | -------- |
| A1       | B1       | C1       |
| A2       | B2       | C2       |
| A3       | B3       | C3       |

### Success Response 

```json
{
	"data": {
		"balance": 997136249
	}
}
```

### Testing
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
