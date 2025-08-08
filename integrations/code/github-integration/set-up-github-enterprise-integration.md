# Set Up GitHub Enterprise Integration

With the Shortcut GitHub integration, specially formatted commit messages can be used to link stories to commits, branches and pull requests, as well as move stories across your workflow. Following these instructions, you can configure the Shortcut GitHub integration to work with one or more GitHub repositories.

**Before continuing**

[Contact our support team](https://help.shortcut.com/hc/en-us/requests/new) to have the GitHub Enterprise integration enabled in your account, before continuing this guide.

#### Setting up the integration in Shortcut

![mceclip0.png](https://help.shortcut.com/hc/article_attachments/4406846955796)

1. In the Shortcut app, click the **User** icon in the lower-left corner, click **Integrations**, and then click **GitHub**.
2. Copy the **GitHub Enterprise Payload URL**. Now head over to your GitHub repo page.

#### Setting up the integration in GitHub

![Setting up the integration](https://help.shortcut.com/hc/article_attachments/16570486739348)

From your repository page in GitHub, select the **Settings** tab.

**Note**

If you wish to add this to the entire GitHub Org, navigate to the Organization Settings page instead, and continue the steps below.

1. On the settings page, click **Webhooks**.
2. Click **Add webhook** in the top right.
3. In the **Payload URL** box, enter the Payload URL you copied from our GitHub Integration dialog.
4. Under "Which events would you like to trigger this webhook", select **Send me everything\***.
5. Content-type should be set to _application/JSON_
6. Click **Add webhook**.

Our GitHub integration is now enabled for this repository!&#x20;

**\***&#x49;f you want to use the **"Let me select individual events**" option, you will need to have at least Create, Delete, Comment, Pull Request and Push selected to capture all events. See image below:

![Selected Events in GitHub Webhook Settings](https://help.shortcut.com/hc/article_attachments/16570499770132)

#### Connecting Individual Accounts

Individuals will need to ensure that their primary email address in GitHub is the same as one of their email addresses in Shortcut. In Github, check your personal account settings, under the email tab.

\
![GitHub\_Primary\_Email\_Address.png](https://help.shortcut.com/hc/article_attachments/16570499771540)

If this is not the same email address used to create your Shortcut account, you'll need to [add that email address to Shortcut](https://help.shortcut.com/hc/en-us/articles/360044062252).

#### GitHub Event Handlers

To set up your integration to use our GitHub Event Handlers, [follow these instructions.](https://help.shortcut.com/hc/en-us/articles/204909925) When you're done, make sure to check out our [the guide to using our GitHub integration.](https://help.shortcut.com/hc/en-us/articles/204909925)
