---
tags: [getting-started]
---

# Overview

Input Tutorial of getting started here...

Our API has predictable, resource oriented URL, and use HTTPS.
- We wrap every API response in JSON or XML
- Set the Content-Type as text/plain for XML or application/json for JSON in Prepaid transaction
- Set the Content-Type as application/xml for XML or application/json for JSON in transaction
- Follow the request method ( **POST** OR **GET** ) which you can find below each function
- Term "PULSA" means "Mobile Topup / Recharge"
- We'd suggest to set the time out to 60 seconds for postpaid transaction

| Column A | Column B | Column C |
| -------- | -------- | -------- |
| A1       | B1       | C1       |
| A2       | B2       | C2       |
| A3       | B3       | C3       |

```json json_schema
{
  "type": "object",
  "properties": {
    "id": {
      "type": "string"
    }
  }
}
```
