# Configuring Okta to Manage Shortcut Users with SCIM

### Configuring Okta to Manage Shortcut Users with SCIM

This documentation covers step-by-step how to configure Okta to enable SCIM provisioning in Shortcut.

### Features

* **Push New Users -** Users created in Okta that are assigned the Shortcut application will be created in your Shortcut Workspace
* **Push Profile Updates -** Updates made to the user's profile through Okta will be pushed to Shortcut
* **Push User Deactivation -** Deactivating, or disabling the user's access to Shortcut via Okta will disable the user in Shortcut

### Requirements

In order to enable SCIM provisioning with Shortcut, you will need to meet the following requirements:

* SCIM provisioning is only available to Shortcut customers on Enterprise plans (Included) and Business plans (Add-On). To learn more about Shortcut's plans and their respective entitlements, please see our [Shortcut Pricing and Plans comparison table](https://www.shortcut.com/pricing#section-plan).
* You must have access to a Shortcut account with Owner or Admin privileges.
* You must have added **both** the [**Shortcut**](https://www.okta.com/integrations/shortcut/) and [**Shortcut SCIM**](https://www.okta.com/integrations/shortcut-scim/) apps to Okta and have SSO or SAML enabled on your Shortcut organization. For more information on configuring SAML 2.0 for Shortcut, [please visit our Okta documentation](https://saml-doc.okta.com/SAML_Docs/How-to-Configure-SAML-2.0-for-Shortcut.html?baseAdminUrl=https://shortcut-admin.okta.com\&app=shortcut\&instanceId=0oa3tvtus74trKCsh697).
* You must set your workspace to invitation only. This setting can be found under **Settings > Invite New User > Settings**
* You must have requested that SCIM be enabled on your account by contacting [support@shortcut.com,](mailto:support@shortcut.com,) and have received your **Shortcut Workspace ID** and **API Token**.

### Step-by-Step Configuration Instructions

### Shortcut SCIM Configuration (SCIM)

1. From your Okta Admin console click **Applications**
2. Select **Browse App Catalog** and search for [**Shortcut SCIM**](https://www.okta.com/integrations/shortcut-scim/)
3. Click on [**Shortcut SCIM**](https://www.okta.com/integrations/shortcut-scim/) and then **Add Integration**
4. On the **General Settings** tab of the **Add Shortcut SCIM** window, be sure to check the boxes next to both of the following options:
   * _**Do not display application icon to users**_
   * _**Do not display application icon in the Okta Mobile App**_**Note**: The [**Shortcut SCIM**](https://www.okta.com/integrations/shortcut-scim/) application is specific to a Workspace in your Shortcut Organization. It is _only_ meant to provision/deprovision users. Logging into your Shortcut Organization should be done instead via the [**Shortcut**](https://www.okta.com/integrations/shortcut/) SAML application. To learn more about Shortcut Organizations and Workspaces, please see our documentation on [_managing organizations_](https://help.shortcut.com/hc/en-us/articles/360001083483-The-Organizations-and-Workspaces-Dashboard), and [_managing workspaces_](https://help.shortcut.com/hc/en-us/articles/360045988452-Managing-Your-Workspaces).![Clipboard\_2023-27-02\_at\_9.25.54\_AM.png](https://help.shortcut.com/hc/article_attachments/13526907339924)
5. Once you have added [**Shortcut SCIM**](https://www.okta.com/integrations/shortcut-scim/) to your Okta tenant, navigate to your **Provisioning** settings for [**Shortcut SCIM**](https://www.okta.com/integrations/shortcut-scim/) and click the **Configure API Integration** button.\
   ![SCR-20230214-ed1.png](https://help.shortcut.com/hc/article_attachments/13195982165012)
6. Check the **Enable API Integration** box.
7. In the **Organization ID** text field, enter the Organization ID you received from support.
8. In the **API Token** text field, enter the SCIM token you received from support.
9. With both **Organization ID** and **API Token** filled out, click **Test API Credentials**. If the credentials are successfully verified, click **Save**.\
   ![SCR-20230214-edk.png](https://help.shortcut.com/hc/article_attachments/13196008105108)
10. In the **Provisioning** settings for [**Shortcut SCIM**](https://www.okta.com/integrations/shortcut-scim/), navigate to the **To App** section and click **Edit**. Select the provisioning features you want to enable and click **Save**. \
    ![SCR-20230214-ei9.png](https://help.shortcut.com/hc/article_attachments/13196122915860)\
    **Note:** The **role** attribute is required and will ensure that a given user is assigned the appropriate Shortcut Role (Admin, Member, Observer) for your Shortcut Workspace. This attribute can be assigned to individual Okta users, or Okta groups based on app assignment preferences for the [**Shortcut SCIM**](https://www.okta.com/integrations/shortcut-scim/) application. For more information on Shortcut User Roles, [please see our documentation.](https://help.shortcut.com/hc/en-us/articles/360033599771-Managing-User-Roles)

### Shortcut Configuration (SAML)

To ensure continued SAML functionality after configuring SCIM, configure your **Sign On** settings tab for the [**Shortcut**](https://www.okta.com/integrations/shortcut/) Okta SAML Application as follows:

1. Set the **Application username format** dropdown menu equal to **Email** and click **Save.**\
   ![mceclip3.png](https://help.shortcut.com/hc/article_attachments/12490294954900)\


### Supported SCIM Attributes

Shortcut currently supports the following attributes mapping:

| **SCIM Attribute Name** | **Notes**                                                                                                                                                                                                                       |
| ----------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| userName                | (_Required_) User's email address                                                                                                                                                                                               |
| email                   | (_Required_) User's email address                                                                                                                                                                                               |
| displayName             | (_Required_) User's name in Shortcut                                                                                                                                                                                            |
| role                    | <p>(<em>Required</em>) User's Shortcut Role, currently supports options for <strong>Admin, Member,</strong> and <strong>Observer</strong></p><p>The <strong>Owner</strong> role is <strong>not currently supported</strong></p> |

**Note:** For all above attributes, the schema namespace used is **urn:ietf:params:scim:schemas:core:2.0:User**

### Advanced Resources

### Ability to define a custom **userName** field for the Shortcut SCIM app <a href="#custom-username-field" id="custom-username-field"></a>

1. The **userName** field by default is locked to to the Okta user's email address. This field is typically configurable via the Sign On tab for Okta apps that use SAML; however, Shortcut has separate apps for SCIM (provisioning users into Shortcut) and for SAML (the app that should be displayed to end users in Okta) and thus the Sign On tab will not be visible.
2. Okta has ability to unlock the **userName** field on a per-tenant basis. Please file a support ticket via [https://support.okta.com/help/s/?language=en\_US](https://support.okta.com/help/s/?language=en_US) asking support to disable the Feature Flag **CONSOLIDATE\_USERNAME\_EL**.
3. When the Feature Flag is disabled, you will be able to enter another attribute or expression to map for the **userName** variable like the screenshot below:![screenshot.png](https://help.shortcut.com/hc/article_attachments/17981919830420)
