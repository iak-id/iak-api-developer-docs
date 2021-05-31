# Quick Start

Here's a quick start to integrate into our service : 

1. Get API Key

    To connect with our API, you need API key as identifier. Get your API key [here](https://developer.iak.id/access-key)

    Learn [more](./api-key.md) about API key.

2. Read API Reference

    Start to explore our documentation to integrate with our products.

    [Read the docs](https://api.iak.id/docs/api-reference/docs/introduction.md)

3. Testing sandbox

    IAK provide sandbox report to help you integrate in sandbox environment. Everything in sandbox report is only simulation, not real transaction.

    Learn [here](./sandbox-report.md) to explore sandbox report.

4. Whitelist IP

    You can increase the security by set whitelist IP. 

<!-- theme: warning -->

> ### Important!
> It's really important to whitelist your IP. 
> [Learn more](../security.md#whitelist-your-ip)

5. Set Callback URL

    In **prepaid** product, we will send you a response to your callback URL to inform you about the prepaid transaction you did before. 
    There are only two possible response that we will send to your callback url:

   1. Success
   2. Failed

    Set your callback URL for [sandbox](https://developer.iak.id/dev-setting) and [production](https://developer.iak.id/prod-setting).

<!-- theme: info -->

> Learn [here](./../security.md) to secure your callback URL.

6. Topup Deposit

    After you integrate your web or apps into our API, you need to topup deposit. We will deduct your deposit based on the price.

    Learn [here](./../topup-deposit.md) how to topup.

7. Call Production API

    Now you are ready to call API in production environment. To switch between sandbox and production you only need do the following:

   1. Change base URL from sandbox to production

      Learn here about base URL [prepaid](docs/api-reference/docs/prepaid%20v1%20(legacy)/base-url.md) and [postpaid](docs/api-reference/docs/postpaid/base-url.md).

   2. Change API key from sandbox to production
      Get your API key [here](https://developer.iak.id/access-key)

8. See Report

    After doing real transaction via production environment, you can see the report for finance needs.

    [See report](https://iak.id/webapp/report/prepaid)


---

  **Question?** See our [FAQ](../faq.md) or contact us at [techsupport@mobilepulsa.com](mailto:techsupport@mobilepulsa.com)
