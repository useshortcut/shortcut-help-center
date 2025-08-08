# HoneyBadger integration

The Honeybadger integration allows you to set preferences about when and where you want errors to be sent to Shortcut as Stories.&#x20;

![honeybadger1.png](https://help.shortcut.com/hc/article_attachments/19577352853652)

**Setting Up the Honeybadger Integration**

To set up this integration, just follow these steps:

1. Go to your Honeybadger project's settings \

2. Scroll down the Integrations section
3. Set your Workspace - This is the name of the Workspace that you created when you set up your account. You can find this immediately after the domain name in the URL: e.g., for _**https://app.shortcut.com/honeybadger the Workspace name is \`honeybadger\`**_
4. Set the API Token - Your API Token can be found in the Shortcut UI by clicking on **Settings > API Tokens**. Choose a name for your token (like Honeybadger) and then click "Generate Token". Copy the highlighted token, and paste it in the API Token field.
5.  Fetch project info - Click the "Fetch Project Info" button to make a request to the Shortcut API to get a list of your Shortcut Projects and Workflow States. This will populate and enable the remaining checkboxes on the form.Choose the project and workflow states.

    Each Honeybadger project is associated with one Shortcut project, and you can make that choice here. You can also choose which of your Shortcut workflow states will be chosen for stories when they are marked as resolved or unresolved. The stories will be updated to those states if you also enable the respective Error Events options.

![Screenshot 2023-07-25 at 9.54.12 AM.png](https://help.shortcut.com/hc/article_attachments/19577352857748)

**Creating Stories with the Honeybadger Integration**

Honeybadger users can create Stories in Shortcut by clicking the "Create Story" button on the error detail page in the Honeybadger UI. By default, these stories will be created as the Shortcut user whose API Token is configured in the integration settings. Users can have stories associated with their own Shortcut account by getting an API Token as described previously and adding it to their [authentication settings](https://app.honeybadger.io/users/edit#authentication).

_Please note, this integration is managed by Honeybadger, so you will need to contact them with any issues._&#x20;
