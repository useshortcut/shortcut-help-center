# Rollbar integration

Rollbar is an error monitoring, alerting, and analytics tool for for teams building software and applications. You can integrate Rollbar with Shortcut by following these steps:

**Step 1: Generate an API Token**

Go to your Workspace's **Settings**>**API Tokens** (under **Your Account**).

Name the token, and then click "Generate Token."

Copy or write down the Rollbar token for use in your Rollbar account (the token will be highlighted in yellow).

![Clubhouse\_Generating\_an\_API\_Token.png](https://help.shortcut.com/hc/article_attachments/360002143966/Clubhouse_Generating_an_API_Token.png)

**Step 2: Connect Your Rollbar and Shortcut Accounts**

![b82F3jundq.gif](https://help.shortcut.com/hc/article_attachments/360000434046/b82F3jundq.gif)![Screen\_Shot\_2018-02-07\_at\_3.28.05\_PM.png](https://help.shortcut.com/hc/article_attachments/360000392626/Screen_Shot_2018-02-07_at_3.28.05_PM.png)

Log in to your Rollbar account, go to **User Settings** > **Connected Accounts,** and click on the Shortcut tab.

Enter the API token you generated in Shortcut into the API token field and save it.

**Step 3: Enable the Shortcut Channel in Your Rollbar Account**

To enable the Shortcut channel, go to **Projects** in your Rollbar account, and then click on the Rollbar project you want to connect to your Shortcut Workspace. Then click on **Notifications** (under **Integrations** in the sidebar).

![find\_projects\_and\_notifications.gif](https://help.shortcut.com/hc/article_attachments/360000403683/find_projects_and_notifications.gif)

Enter your Workspace name, and edit any other settings you wish to, then click "Enable Shortcut Integration."

**Note:** The Workspace name you enter here should match your Shortcut Workspace URL exactly. The Workspace name in Rollbar is case-sensitive, and should not contain spaces (since Shortcut URLs cannot contain spaces).

![Screen\_Shot\_2018-02-09\_at\_10.31.55\_PM.png](https://help.shortcut.com/hc/article_attachments/360000433926/Screen_Shot_2018-02-09_at_10.31.55_PM.png)

Rollbar will confirm that the integration has been enabled with a green alert message: "Shortcut integration is now set up. You can customize below."

![Screen\_Shot\_2018-02-07\_at\_3.39.10\_PM.png](https://help.shortcut.com/hc/article_attachments/360000392766/Screen_Shot_2018-02-07_at_3.39.10_PM.png)

**Step 4: Configure the Settings for Your Shortcut Channel**

You can now edit the Shortcut integration's Project, Epic, State, and Label settings. Click "Save Settings" when finished.

![Screen\_Shot\_2018-02-09\_at\_10.39.13\_PM.png](https://help.shortcut.com/hc/article_attachments/360000432583/Screen_Shot_2018-02-09_at_10.39.13_PM.png)

You can also add or edit Rules for the Shortcut integration.

![Screen\_Shot\_2018-02-07\_at\_4.11.11\_PM.png](https://help.shortcut.com/hc/article_attachments/360000392826/Screen_Shot_2018-02-07_at_4.11.11_PM.png)

**Step 5: Test the Integration (Optional)**

You can test the Shortcut integration by click on the Send Test Notification button (found next to the Enabled/Disabled switch).

Rollbar will confirm that a test story was successfully created with a green alert message: "Test story created. View in Shortcut."

![Screen\_Shot\_2018-02-07\_at\_3.39.28\_PM.png](https://help.shortcut.com/hc/article_attachments/360000393066/Screen_Shot_2018-02-07_at_3.39.28_PM.png)

![Screen-Shot-2018-02-07-at-3.40.59-PM-2.png](https://help.shortcut.com/hc/article_attachments/360000962563/Screen-Shot-2018-02-07-at-3.40.59-PM-2.png)

**Note:** Our friends at Rollbar built and maintain this integration, so if it breaks, [be sure to let them know](https://rollbar.com/contact/)!
