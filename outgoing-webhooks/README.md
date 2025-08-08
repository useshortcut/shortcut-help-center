# Outgoing Webhooks

### Setting up Outgoing Webhooks

![](https://help.shortcut.com/hc/article_attachments/31075412879636)

_**Note:** This article describes manually setting up webhooks. If you're building a custom integration and want to manage webhooks programmatically, see_ [_Registering Outgoing Webhooks (API)_](https://help.shortcut.com/hc/en-us/articles/34734717380756)_._

Outgoing webhooks can be used to gather organization information and integrate with external services. Once configured, events will fire to the URL(s) of your choice and can be used to create applications for various purposes, such as notifications and reporting.

Developer documentation for our webhooks can be found [here](https://developer.shortcut.com/api/webhook/v1#Shortcut-Outgoing-Webhooks).

### How to Enable Shortcut Webhooks <a href="#h_01j9pb6ge548hkzz51r2tfrtaq" id="h_01j9pb6ge548hkzz51r2tfrtaq"></a>

Click the gear wheel in the upper right-hand corner of any Shortcut page. Navigate to "Integrations" and click on "Webhooks."

![](https://help.shortcut.com/hc/article_attachments/31075412881556)

From the Webhook dialogue, click Add New Webhook, you will be asked to provide a Payload URL.

![](https://help.shortcut.com/hc/article_attachments/34765005975572)

### Setting the Payload URL <a href="#h_01j9pb6p5eph6v0edsecvjbrmw" id="h_01j9pb6p5eph6v0edsecvjbrmw"></a>

You will need to set distinct URL for the webhook to send events to, it can be any URL you wish. Webhook data is sent as JSON in the POST request body. The events that are sent to the webhook are outlined in the [developer documentation](https://developer.shortcut.com/api/webhook/v1#Shortcut-Outgoing-Webhooks).&#x20;

### Setting a Secret API Token <a href="#h_01j9pb6thnz1y4tsjdb2zq0knb" id="h_01j9pb6thnz1y4tsjdb2zq0knb"></a>

Setting a secret API token is optional, but if you choose to do so, Shortcut will use it to create a hash signature with each payload that is passed along in the Shortcut-Signature header. Shortcut uses an HMAC hexdigest to compute the hash.

Please refer to our [developer documentation](https://developer.shortcut.com/api/webhook/v1#Shortcut-Outgoing-Webhooks) for additional information such as webhook formats and example use cases.
