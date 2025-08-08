# Jira Sync Overview

### Jira Sync Overview

Try Shortcut with minimal disruption by syncing a Jira project to Shortcut and see how much easier and better it is to work in Shortcut!

### What is Jira Sync? <a href="#h_01hqk961dpjfgy495b9zr5awa5" id="h_01hqk961dpjfgy495b9zr5awa5"></a>

* The Jira Sync helps remove friction when new users currently using Jira are evaluating Shortcut. You can try Shortcut with minimal disruption to your existing Jira instance during your trial! It is an opportunity to work in Shortcut and update stakeholders on the status of your team’s work.&#x20;

### What does Jira Sync do when it is turned on in a Shortcut Workspace? <a href="#h_01hqk961dpkn4e62v0arw0mq5a" id="h_01hqk961dpkn4e62v0arw0mq5a"></a>

* New Stories created in the Shortcut workspace will be created as issues in the Jira project&#x20;
* New issues created in the Jira project will be created in Shortcut.
* Shortcut Story Workflow States updates with be reflected in Jira.
* The following table shows what is and what is not synced upon and after a **Story or Issue creation**:

| **What is Synced?**                                                                                                                                                                                                                                                                                                                                                                                                                                                                                | **What is not Synced?**                                                                                                                                                                                                                                                                                                                  |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <ul><li><p>Shortcut Issue creation &#x3C;--> Jira Issue creation:</p><ul><li>Story/Issue Title</li><li>Story/Issue Description</li><li>Story/Issue Requestor</li><li>Link to Shortcut Story in Jira Issue description/Link to Jira Issue on the Shortcut Story </li></ul></li><li><p>Shortcut Issue Update &#x3C;--> Jira Issue Update:</p><ul><li>Story/Issue Title</li><li>Story/Issue Description</li></ul></li><li>Shortcut Issue Workflow State Update --> Jira Issue Status Update</li></ul> | <ul><li>After Story creation, any changes to Story metadata (excluding title and description) will not sync over in Jira.</li><li><p>The Workflow State status is not bidirectional.</p><ul><li>Post-sync updates in Shortcut sync back to Jira however updates in Jira will not sync back to Shortcut at this time.</li></ul></li></ul> |

### How do you set up Jira Sync? <a href="#h_01hqk961dp0vketrfhar700sbf" id="h_01hqk961dp0vketrfhar700sbf"></a>

**Step 1: Import Jira Data**

* Import and map your Jira data using Auto-import for Jira. You can find detailed steps for completing this import process in [our Help Center article for Importing data from Jira into Shortcut.](https://help.shortcut.com/hc/en-us/articles/360045791591)

![mceclip0.png](https://help.shortcut.com/hc/article_attachments/13376660674196)

* Please note that in the last step of the import process, you will be asked if you would like to turn on Jira Sync and select a Team that newly synced Stories will be assigned to in Shortcut. If not, simply complete the import process.

![TurnOnJiraSyncNew.png](https://help.shortcut.com/hc/article_attachments/13530965166612)

**Step 2: Set Up Jira Sync**

* If you have already imported the data from Jira to Shortcut, skip step 1 and navigate to [your Settings > Import/Sync page](https://app.shortcut.com/settings/import) and select the "Set Up Jira Sync" option.

![mceclip2.png](https://help.shortcut.com/hc/article_attachments/13467479822740)

**Step 3: Map the Data**

* When you select that setup option, the below modal will show where you can select the Jira Project you are hoping to sync with a Shortcut Workflow.&#x20;
  * Please note that only one Sync can be active at a time per Workspace&#x20;

![](https://lh5.googleusercontent.com/IbeNS8Hutcff_BOyEmQIOfYWXM9Qp37dCuKImlHvSDCyU_SoOFclZdhbRhDNg0DXIZy_HkgX9n4GBpajbklHYY0adOpZ88FhYdKXI1T43kVmVJENg00o3iQ-AFq5v_kJrcg9p8UrSPGxS1Rckugdj6qzag=s2048)

* If you have already imported Jira data into Shortcut, when you turn on the Jira Sync you will be asked to choose a Shortcut Team (you can also select no Team) to assign stories to upon creation.

![mceclip3.png](https://help.shortcut.com/hc/article_attachments/13476158848404)

### After the Sync: <a href="#h_01hqk961dqwfa5j4qecn8zcaz5" id="h_01hqk961dqwfa5j4qecn8zcaz5"></a>

* The UI shows the live sync connection.
* The option to disable sync is provided.
  * Please note that if you would like to sync another Jira project, you will have to remove the Jira sync that is active.

![mceclip4.png](https://help.shortcut.com/hc/article_attachments/13476348444820)

* Shortcut Stories will show the Shortcut <> Jira connection:
  * On the Story Card **after** Story creation:

![](https://lh3.googleusercontent.com/m8Opfb-1MQx0NFAoNg7WqLa2_nTcDUdjcwvnZ4K5x1KJ-kmJL4ahv59MsIF48yOf3FMY2QhUtG4Hq1d2zuElAbxtM_LiKttSooLnQMCwKj1LYv4pYTxlthHKSp3NRx3mXiPyEaQY7w2tTo_KXdpsv6WhxQ=s2048)

*
  * In the Story modal **after** Story creation:

![mceclip0.png](https://help.shortcut.com/hc/article_attachments/13533202851092)

*
  * In the Story modal **during** Story Creation:

![](https://lh6.googleusercontent.com/tNs5alL80UHqOmTgCUPMvZ6zsr9A8BoX3TK8F78O2l0Xgr69zIl143KXRg-c7J_R4w9P-DK2Br456JjwsnI2CF4A9-6DjUeAhGaMcVVnZXG4dC2JIfbjzbDri-jnNqvLGFB23-tO-JGfnTHubgJWhykNNQ=s2048)
