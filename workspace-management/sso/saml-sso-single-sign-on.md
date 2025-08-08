# SAML SSO (Single Sign On)

![](https://help.shortcut.com/hc/article_attachments/28594961134356)

With Shortcut SSO, your team can quickly manage how associated users access the [Shortcut](https://www.shortcut.com/) tool.  Shortcut SSO is currently available to all Organization's on a paid plan as an Add-on but is included for Organization's on an Enterprise plan. For more information on the specific entitlements allotted for each plan, please visit [the Pricing page on Shortcut.com to view the Pricing and Plans comparison table](https://www.shortcut.com/pricing#plan).

### What IDP (Identity Provider) clients do we support? <a href="#h_01j33e4636sdh644b3bpb0dz8w" id="h_01j33e4636sdh644b3bpb0dz8w"></a>

While we offer support for a variety of IDP clients such as, Okta, OneLogin, Google Workspace, Microsoft EntraID, etc., please feel free to reach out if you have specific questions regarding a particular IDP that your team uses.

Please note that while we do offer SCIM provisioning, this is currently only supported via the Okta client. For more information, please see our Help Center documentation for [Configuring Okta to Manage Shortcut Users with SCIM.](https://help.shortcut.com/hc/en-us/articles/12335315792788-Configuring-Okta-to-Manage-Shortcut-Users-with-SCIM)

### How to set up SAML SSO: <a href="#h_01j33ea1jkgs1t8q1hz0en8dan" id="h_01j33ea1jkgs1t8q1hz0en8dan"></a>

Please connect with our Support team at [support@Shortcut.com](mailto:support@Shortcut.com) to start the process. They will be able to connect with the respective Shortcut Team members to discuss Add-on pricing.

If your Organization is already on an Enterprise plan, our Support team can get you up and running fairly quickly.

Either way, when reaching out for more information or to setup SSO, it may be a good to note the IDP client your Organization is seeking to utilize. This may determine the configuration details we provide to you, and we can more quickly be able to get your team up and running.

### How to Login Using SSO: <a href="#h_01j33fffm4skzdr1t0mjhzaxsx" id="h_01j33fffm4skzdr1t0mjhzaxsx"></a>

There are two methods of signing into Shortcut using SSO:

1. Using an Identity-Provider-initiated login link.
2. Using the [Shortcut SSO Login Page](https://app.shortcut.com/sso) and entering in the Organization URL slug.

### Important Points to Note: <a href="#h_01j33f2fa4nxnw4twskkzhkr1q" id="h_01j33f2fa4nxnw4twskkzhkr1q"></a>

* As noted above, SCIM Provisioning is only supported via the Okta IDP client.
* Please ensure all users have a Shortcut user account associated with the email address used in the IDP client.
  * If not utilizing SCIM provisioning, users must first create a Shortcut user account after either being:
    * Invited to a Workspace by an Admin via email or using a generated invite link.
    * Or if it is enabled for the respective Workspace, by joining a Workspace using the "auto-join via email domain" functionality. See the "Via Email Domain" tab within [Managing Invitations – Shortcut Help Center](https://help.shortcut.com/hc/en-us/articles/360033599271-Managing-Invitations#heading-1) for more details on this invite method.
* SSO can enforced as a mandatory login method. This would be a setting we would need to enable in the backend.
  * In order to set SSO as the mandatory login method, any users that are associated with your Organization in Shortcut, are not able to be associated with another Shortcut Organization.
    * This mandatory SSO setting can be enabled or disabled as needed at any time.
* The SSO session duration is by default set to 12 hours for security purposes, but we can also adjust this if needed.&#x20;

If you'd like to enforce SSO the mandatory login method or need the session duration to be extended or shortened, please reach out to Shortcut Support at [support@shortcut.com](mailto:support@shortcut.com)
