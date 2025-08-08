# Github integration

For instructions on setting up the Version Control System of your choice, please expand the one desired below:

### ![GitHub](https://help.shortcut.com/hc/article_attachments/360091316071)**GitHub** <a href="#h_01j8g86jkmqqry8thhd55cvytr" id="h_01j8g86jkmqqry8thhd55cvytr"></a>

With the [Shortcut](https://shortcut.com/) GitHub integration, specially formatted commit messages can be used to link stories to commits, branches and pull requests, as well as move stories across your workflow. Following these instructions, you can configure the Shortcut GitHub integration to work with one or more GitHub repositories.

#### Setting up the GitHub integration in Shortcut <a href="#h_01j8g86jkn7zys280yxkhcn8h9" id="h_01j8g86jkn7zys280yxkhcn8h9"></a>

![GitHub Settings](https://help.shortcut.com/hc/article_attachments/30639919535252)

\


1. In the Shortcut app, click the **Integrations** icon in the lower left corner, and then select **GitHub**.
2. Click **Add Account.**

#### Setting up the integration in GitHub <a href="#h_28088cd9-440e-44e5-9535-a6daeb3d439f" id="h_28088cd9-440e-44e5-9535-a6daeb3d439f"></a>

![GitHub Repository Configuration](https://help.shortcut.com/hc/article_attachments/30639909789716)

After clicking Add Account in Shortcut, you will be taken to GitHub to select which GitHub account to link. From this next screen, you can authorize access to all repositories in the account, or only select repositories.

Successful installation of our integration requires the user performing this action to be an Admin in both Shortcut and GitHub. Additionally, while the GitHub integration will connect to multiple Workspaces, it will only connect with one Organization at a time.

Once all, or the select repos have been selected, click **Install**. You will be redirected back to Shortcut with the GitHub integration window reflecting the newly connected account:

![GitHub Settings](https://help.shortcut.com/hc/article_attachments/30639909796628)

#### Connecting Individual Accounts <a href="#h_01j8g86jkpt4mme9n806pvxef2" id="h_01j8g86jkpt4mme9n806pvxef2"></a>

Individuals will need to ensure that their primary email address in GitHub is the same as one of their email addresses in Shortcut. In GitHub, check your personal account settings, under the email tab.

![GitHub Email](https://help.shortcut.com/hc/article_attachments/30639909802260)

If this is not the same email address used to create your Shortcut account, you'll need to [add that email address to Shortcut](https://help.clubhouse.io/hc/en-us/articles/360044503211).

#### GitHub Event Handlers <a href="#h_01j8g86jkp0y5zkx5wq7pz46a5" id="h_01j8g86jkp0y5zkx5wq7pz46a5"></a>

To set up your integration to use our Event Handlers, [follow these instructions.](https://help.clubhouse.io/hc/en-us/articles/360023113952) When you're done, make sure to check out our [guide to using our VCS integration with PRs and Branches.](https://help.shortcut.com/hc/en-us/articles/207540323)

### ![GitLab](https://help.shortcut.com/hc/article_attachments/360091316131)**GitLab** <a href="#h_01j8g86jkprp98ves5b0dtnbpg" id="h_01j8g86jkprp98ves5b0dtnbpg"></a>

With the Shortcut GitLab integration you can link Stories to commits, branches and pull requests, as well as move Stories across your workflow. Following these instructions, you can configure the Shortcut GitLab integration to work with your GitLab account.

**Note:** This integrates with GitLab.com and self-managed GitLab installations using version 9.5 or higher.

**For self-managed GitLab users:** Our GitLab integration needs to talk to the API of your self-managed GitLab install to properly process some event payloads. It determines the address of the API using the URLs included in the webhook payloads, and that address needs to be publicly accessible for us to reach it. Non-resolvable hostnames will cause the integration to not work correctly.

#### Setting up the integration in Shortcut <a href="#h.ytnm42t9da3x" id="h.ytnm42t9da3x"></a>

Only Admins and Owners can activate this integration in Shortcut. In the Shortcut app, click the **Integrations** option in the lower left corner of the UI, and then click **GitLab.** Click the **Slider** to enable, then **copy the GitLab Payload URL** and **open your GitLab account.**

![](https://help.shortcut.com/hc/article_attachments/17477297306132)

In GitLab, choose specific Projects that you want to send data to Shortcut, or if your GitLab.com plan supports Group Webhooks, you can send data from every Project in the Group. From the **Project page (or Group page)**, click **Settings >Webhooks**, then paste the GitLab Payload URL into the Integrations URL field.

![mceclip1.png](https://help.shortcut.com/hc/article_attachments/17473660094228)

Next, check that the correct events will be sent to Shortcut. Click the checkbox for:

* Push Events
* Comments
* Merge request events

You may optionally include Confidential Comments.

![](https://help.shortcut.com/hc/article_attachments/17473664287380)

If you are not using GitLab's Group webhooks, be sure that you've added the GitLab Payload URL to the Webhook Settings for each Project that should send data to Shortcut. **Add user(s) email address as public in GitLab** in order for Shortcut's event handler to determine which GitLab user performed certain actions in Shortcut, we match the email from GitLab payload to that of the Shortcut user. Ensure that the public email in **Settings (click on the user icon options)** > **Edit Profile** is set to the appropriate email for the user in Shortcut.

![](https://help.shortcut.com/hc/article_attachments/17476832409492)

#### Access Token <a href="#h_01j8g86jkpdremgwhw91wg9qgw" id="h_01j8g86jkpdremgwhw91wg9qgw"></a>

The last step is to place a personal access token from GitLab into Shortcut. You may use an individual user's token, but it is recommended that you create a bot user in GitLab.&#x20;

**1.** Create a new user on your GitLab.com organization. Consider using a name that signifies this user connects GitLab to Shortcut, like 'Shortcut Bot'.

**2.** In GitLab, invite your bot user to the Projects that you want Shortcut to access, and grant that user Developer permissions.

**3.** Log in with the bot user account and open the User Settings.

**4.** Generate a [personal access token ](https://docs.gitlab.com/ee/user/profile/personal_access_tokens.html)scoped to have API access &#x20;

![](https://help.shortcut.com/hc/article_attachments/17476889824148)

![](https://help.shortcut.com/hc/article_attachments/17476932146196)

**5.** Copy the personal access token and paste it into the API Access Token field in the GitLab integration pane. Click Update API Access Token to save the token value.

![](https://help.shortcut.com/hc/article_attachments/17477015692436)

#### GitLab Event Handlers <a href="#h_01j8g86jkpwaa9cj8majgbppyy" id="h_01j8g86jkpwaa9cj8majgbppyy"></a>

To set up your integration to use our GitHub Event Handlers, [follow these instructions.](https://help.clubhouse.io/hc/en-us/articles/360023113952) When you're done, make sure to check out our [the guide to using our VCS integration with PRs and Branches.](https://help.shortcut.com/hc/en-us/articles/207540323)

### ![bitbucket\_128x128-2fcc9012d1.png](https://help.shortcut.com/hc/article_attachments/360091316111) **BitBucket** <a href="#h_01j8g86jkp5ckndnaac4aqv5gm" id="h_01j8g86jkp5ckndnaac4aqv5gm"></a>

With the Shortcut Bitbucket integration, you can link Stories to commits, branches and pull requests, as well as move Stories across your workflow. Following these instructions, you can configure the Shortcut Bitbucket integration to work with your Bitbucket Cloud account.

**Note: This integrates with Bitbucket Cloud and not Bitbucket Server.**

#### Setting up the integration in Shortcut <a href="#h.ytnm42t9da3x" id="h.ytnm42t9da3x"></a>

Only Admins and Owners can activate this integration in Shortcut. In the Shortcut app, click the **Integrations** icon near the bottom-left of the UI, and then select **Bitbucket. Click "Connect to Bitbucket Cloud"** to begin the authorization process.

![BitBucket Integration Window](https://help.shortcut.com/hc/article_attachments/30822218084372)

Next, authorize the Bitbucket account you would like to connect to the Shortcut Workspace.

**Note:** You can connect multiple Shortcut Workspaces to the same Bitbucket account, but you cannot connect multiple Bitbucket accounts to the same Shortcut Workspace.

![BitBucket to Shortcut Authorization](https://help.shortcut.com/hc/article_attachments/30822228940692)

When you’ve successfully authorized Shortcut to access your Bitbucket account you’ll see which Bitbucket account Shortcut is connected to in the integrations screen.

![Success!](https://help.shortcut.com/hc/article_attachments/30822228941716)

#### BitBucket Event Handlers <a href="#h_01j8g86jkqwz8rkq5jpctjqr11" id="h_01j8g86jkqwz8rkq5jpctjqr11"></a>

To set up your integration to use our BitBucket Event Handlers, [follow these instructions.](https://help.clubhouse.io/hc/en-us/articles/360023113952) When you're done, make sure to check out [the guide to using our VCS integration with PRs and Branches.](https://help.shortcut.com/hc/en-us/articles/207540323)
