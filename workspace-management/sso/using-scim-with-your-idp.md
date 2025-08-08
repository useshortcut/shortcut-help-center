# Using SCIM with your IdP

### Using SCIM with your IdP

This documentation serves to aid you in configuring SCIM with your organization's Identity Provider (IdP). As of publication, the only official Shortcut supported SCIM integration is via [Okta.](https://help.shortcut.com/hc/en-us/articles/12335315792788)

### Supported SCIM Features

* **Push New Users -** Users created in your IdP that are assigned the Shortcut application will be created in your Shortcut Workspace
* **Push Profile Updates -** Updates made to the user's profile through your IdP will be pushed to Shortcut
* **Push User Deactivation -** Deactivating, or disabling the user's access to Shortcut via your IdP will disable the user in Shortcut

### Requirements

In order to enable SCIM provisioning with Shortcut, you will need to meet the following requirements:

* SCIM provisioning is only available to Shortcut customers on Enterprise plans. To learn more about Shortcut's plans and their offerings, please see our help center page, [Shortcut Plan](https://help.shortcut.com/hc/en-us/articles/360016616772-Shortcut-Plan-Options)[ Options](https://help.shortcut.com/hc/en-us/articles/360016616772-Shortcut-Plan-Options).
* You must have access to a Shortcut account with Owner or Admin privileges.
* Because SCIM operates at the Shortcut Workspace level, and SAML operates at the Shortcut Organization level, it is recommended that organizations with many Shortcut Workspaces create separate SCIM applications within their IdP for each Shortcut Workspace looking to leverage SCIM.
* You must set your workspace to invitation only. This setting can be found under **Settings > Invite New User > Settings**
* You must have requested that SCIM be enabled on your account by contacting [support@shortcut.com,](mailto:support@shortcut.com,) and have received your **Shortcut Workspace ID** and **API Token**.
  * The **Shortcut Workspace ID** will be used to create your SCIM URL:
    * `https://api.app.shortcut.com/integrations/scim/YOUR_WORKSPACE_ID`
  * The **API Token** will be used as your Bearer token for your requests' Authorization headers:
    * `Authorization: Bearer YOUR_API_TOKEN`

### Supported SCIM Attributes

Shortcut currently supports the following attributes mapping:

| **SCIM Attribute Name** | **Notes**                                                                                                                                                                                                                       |
| ----------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `userName`              | (_Required_) User's email address                                                                                                                                                                                               |
| `email`                 | (_Required_) User's email address                                                                                                                                                                                               |
| `displayName`           | (_Required_) User's name in Shortcut                                                                                                                                                                                            |
| `role`                  | <p>(<em>Required</em>) User's Shortcut Role, currently supports options for <strong>Admin, Member,</strong> and <strong>Observer</strong></p><p>The <strong>Owner</strong> role is <strong>not currently supported</strong></p> |

**Note:** For all above attributes, the schema namespace used is **urn:ietf:params:scim:schemas:core:2.0:User**

### SCIM Configuration

Depending on your IdP, the below fields may vary in name

*   **SCIM Base URI**:&#x20;

    `https://api.app.shortcut.com/integrations/scim/YOUR_WORKSPACE_ID`

    * To get your Shortcut Workspace ID, please contact [support@shortcut.com](mailto:support@shortcut.com,)
* **Authorization method**: `header auth`
  * To get your Shortcut Bearer token, please contact [support@shortcut.com](mailto:support@shortcut.com,)
* **Unique Identifier Field**: `email`
