# GitLab integration

### Setting up the Clubhouse GitLab Integration

With the Clubhouse GitLab integration you can link Stories to commits, branches and pull requests, as well as move Stories across your workflow.

Following these instructions, you can configure the Clubhouse GitLab integration to work with your GitLab account.

**Note: This integrates with GitLab.com and self-managed GitLab installations using version 9.5 or higher.**&#x20;

**For self-managed GitLab users:** Our GitLab integration needs to talk to the API of your self-managed GitLab install to properly process some event payloads. It determines the address of the API using the URLs included in the webhook payloads, and that address needs to be publicly accessible for us to reach it. Non-resolvable hostnames will cause the integration to not work correctly.&#x20;

### Setting up the integration in Clubhouse <a href="#h.ytnm42t9da3x" id="h.ytnm42t9da3x"></a>

Only Admins and Owners can activate this integration in Clubhouse.

In the Clubhouse app, click the **Gear** icon in the upper right corner, click **Integrations**, and then click **GitLab.**

Click the **Slider** to enable, then **copy the GitLab Payload URL** and **open your GitLab account.**

![Clubhouse\_GitLab\_Integration\_Enabled.png](https://help.shortcut.com/hc/article_attachments/360023724012/Clubhouse_GitLab_Integration_Enabled.png)

In GitLab, choose specific Projects that you want to send data to Clubhouse, or if your GitLab.com plan supports Group Webhooks, you can send data from every Project in the Group.

From the P**roject page (or Group page)**, click **Settings > Integrations**, then paste the GitLab Payload URL into the Integrations URL field.

![Clubhouse\_GitLab\_Integration\_Webhook\_Setup.png](https://help.shortcut.com/hc/article_attachments/360023762051/Clubhouse_GitLab_Integration_Webhook_Setup.png)

Next, check that the correct events will be sent to Clubhouse.

Click the checkbox for:

* Push Events
* Comments
* Merge request events

&#x20;You may optionally include Confidential Comments.

![\_gitlab-testing\_\_\_GitLab\_2019-03-15\_11-00-01.png](https://help.shortcut.com/hc/article_attachments/360023884972/_gitlab-testing___GitLab_2019-03-15_11-00-01.png)

If you are not using GitLab's Group webhooks, be sure that you've added the GitLab Payload URL to the Integrations Settings for each Project that should send data to Clubhouse.

**Add user(s) email address as public in GitLab**

In order for Clubhouse's event handler to determine which GitLab user performed certain actions in Clubhouse, we match the email from GitLab payload to that of the Clubhouse user. Ensure that the public email in **Settings (under user icon)** > **Main Settings** is set to the appropriate email for the user in Clubhouse.

![mceclip0.png](https://help.shortcut.com/hc/article_attachments/360039476271/mceclip0.png)

The last step is to place a personal access token from GitLab into Clubhouse. You may use an individual user's token, but it is recommended that you create a bot user in GitLab.

1\. Create a new user on in your GitLab.com organization. Consider using a name that signifies this user connects GitLab to Clubhouse, like 'Clubhouse Bot'.

2\. In GitLab, invite your bot user to the Projects that you want Clubhouse to access, and grant that user Developer permissions.

3\. Log in with the bot user account and open the User Settings.

4\. Generate a [personal access token](https://docs.gitlab.com/ee/user/profile/personal_access_tokens.html) scoped to have api access

![Clubhouse\_GitLab\_Access\_Token.png](https://help.shortcut.com/hc/article_attachments/360023751552/Clubhouse_GitLab_Access_Token.png)

![Clubhouse\_GitLab\_Access\_Token\_Generated.png](https://help.shortcut.com/hc/article_attachments/360023751652/Clubhouse_GitLab_Access_Token_Generated.png)

5\. Copy the personal access token and paste it into the API Access Token field in the GitLab integration pane. Click Update API Access Token to save the token value.

![Clubhouse\_GitLab\_Access\_Token\_added.png](https://help.shortcut.com/hc/article_attachments/360023751892/Clubhouse_GitLab_Access_Token_added.png)
