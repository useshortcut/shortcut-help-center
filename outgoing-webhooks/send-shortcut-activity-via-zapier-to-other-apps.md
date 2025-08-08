# Send Shortcut activity via Zapier to other Apps

![](https://help.shortcut.com/hc/article_attachments/19493256463636)

Outgoing webhooks can be utilized to gather information from your Shortcut Workspace and integrate it with external services. Once configured, events in Shortcut will fire to the URL(s) of your choice and can be used to create applications for various purposes, such as notifications and reporting. This guide will cover how to use Shortcut Webhooks to send events to a Zapier URL, which will allow you to use said events to connect to any of the [1,500+ Zapier apps](https://zapier.com/apps).

### **How to enable Shortcut Webhooks** <a href="#h_01hb6a81k90v050n6b6r42hr22" id="h_01hb6a81k90v050n6b6r42hr22"></a>

In the lower left-hand corner of any Shortcut page, navigate to "Integrations" and click on "Webhooks."

![mceclip1.png](https://help.shortcut.com/hc/article_attachments/360042988872)

From within the Webhook dialog, click **+ Add New Webhook**, you will then be asked to provide a Payload URL. (_The secret is not needed for this integration._)

![](https://help.shortcut.com/hc/article_attachments/19493077334292)

### **Getting the Payload URL from Zapier** <a href="#h_01hb6a81k9g2hq6dwzx6s5epct" id="h_01hb6a81k9g2hq6dwzx6s5epct"></a>

The Payload URL is where Shortcut will send event data to. This will allow Zapier to listen to said event and update your favorite app(s). To get this from Zapier:&#x20;

1. &#x20;[Login](https://zapier.com/app/login/) to your Zapier account.
2. &#x20;Click the "Create Zap" when on your Dashboard.
3. &#x20;Search for the "**Webhooks by Zapier**" app. _Please note_: _this is a_ [_premium app_](https://zapier.com/help/create/basics/learn-key-concepts-in-zapier#step-14)_._
4. &#x20;Under Choose Trigger Event, select **Catch Hook.**
5. &#x20;Click Continue.
6. &#x20;Copy the Payload URL generated.
7. ![mceclip1.png](https://help.shortcut.com/hc/article_attachments/360042907571)
8. Return to the Webhooks integration in Shortcut, paste the Payload URL, and click "Add New Webhook".
9. Switch back to Zapier and click "Continue".

### **Test that Shortcut Activity is Being Received by Zapier** <a href="#h_01hb6a81k9x1jnqwjbw0rr3fh2" id="h_01hb6a81k9x1jnqwjbw0rr3fh2"></a>

![mceclip2.png](https://help.shortcut.com/hc/article_attachments/360042908911)

To ensure that Zapier is detecting the events you want it to detect, these need to be triggered in Shortcut. Examples of common events:

* If a Story is moved to "Ready for QA"
* If an Epic is moved to the "Started" state
* If a Story had a Label added/removed
* If a Story in a particular Project has a deadline set
* Log whenever Stories are Created, Started, or Completed

Click "**Test & Review**" as shown above. Zapier will now 'listen' for any of the aforementioned Shortcut events. During this moment, go back to Shortcut and manually trigger the event you wish for Zapier to capture. This will be picked up by Zapier once you see the Hook:

![mceclip3.png](https://help.shortcut.com/hc/article_attachments/360042878192)

### **Connecting this trigger to your favorite app** <a href="#h_01hb6a81k992rmyxt9h36rdnjg" id="h_01hb6a81k992rmyxt9h36rdnjg"></a>

After confirming Zapier caught the Shortcut event, it is now time to choose what happens when said event occurs by selecting your favorite app from this list.

![mceclip0.png](https://help.shortcut.com/hc/article_attachments/360043018291)

_Follow that app's on-screen instructions as to what is supposed to happen in said app_

### **Zapier Templates** <a href="#h_01hb6a81k96ezhf8dsh3gnf2mx" id="h_01hb6a81k96ezhf8dsh3gnf2mx"></a>

Need ideas on getting started? Below are just a few webhook templates to get you started. Click on the image to take you to the Zap editor.&#x20;

[![mceclip4.png](https://help.shortcut.com/hc/article_attachments/360043025151)](https://zapier.com/app/editor/template/11509?selected_apis=WebHookAPI%2CGitHubAPI\&referrer=explore-page\&from_url=https%3A%2F%2Fzapier.com%2Fapps%2Fintegrations%2F)

[![mceclip5.png](https://help.shortcut.com/hc/article_attachments/360043025451)](https://zapier.com/app/editor/template/1597?selected_apis=WebHookAPI%2CSlackAPI\&referrer=explore-page\&from_url=https%3A%2F%2Fzapier.com%2Fapps%2Fintegrations%2F)

[![mceclip7.png](https://help.shortcut.com/hc/article_attachments/360042992432)](https://zapier.com/app/editor/template/8647?selected_apis=WebHookAPI%2CZendeskV2API\&referrer=explore-page\&from_url=https%3A%2F%2Fzapier.com%2Fapps%2Fintegrations%2F)

[![mceclip8.png](https://help.shortcut.com/hc/article_attachments/360042992932)](https://zapier.com/app/editor/template/10651?selected_apis=WebHookAPI%2CWebHookAPI\&referrer=explore-page\&from_url=https%3A%2F%2Fzapier.com%2Fapps%2Fintegrations%2F)
