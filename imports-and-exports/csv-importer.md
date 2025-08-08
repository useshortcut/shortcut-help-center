# CSV Importer

### CSV Importer

If you're switching from a tool like Linear, ClickUp, Pivotal Tracker, Monday.com, or Zenhub, or if you need to recreate existing Story data in another Shortcut Workspace, you can import that work using our **CSV import tool**.

### Initiate Import Request <a href="#h_01h9670187h7aqt988rvnfqn68" id="h_01h9670187h7aqt988rvnfqn68"></a>

The import process is assisted by our friendly Support team. Please follow the following steps inside Shortcut:

1. Navigate to **Settings**
2. Click **Import / Sync** under Workspace Settings
3. Select which tool you are coming from to access the [CSV Import Guide](https://help.shortcut.com/hc/en-us/articles/15240344441108-CSV-Importer?_gl=1*1cd84yb*_gcl_au*MTYzNTcyOTA3Ny4xNzQwNzU1NTkw) and CSV template, follow the instructions in the file to complete the data entry.
4. Once finished, download the "Import Template" sheet as a CSV, and send that file **support@shortcut.com** to import. Note: Multiple imports can be performed if needed.

We will get back to you shortly and share the CSV template needed to get started!

![Video\_25-03-20\_21-52-08.gif](https://help.shortcut.com/hc/article_attachments/35858550084756)

**If seeking to Import from JIRA Server...**

...Follow the Import Request flow above to begin the process and export the issues from your JIRA Server Instance that you want to import into your Shortcut Workspace by using the Search Function:

1. Navigate to "All Issues"
2. Filter to the Issues you would like to Import
3. Select "Export">"CSV All Fields"
4. Use the CSV template provided obtained in the UI (noted above) to properly format your file to import in the preferred Shortcut Workspace.

### CSV Template Formatting <a href="#h_01h967018701gs1bhtr2bsqna7" id="h_01h967018701gs1bhtr2bsqna7"></a>

Support will have reached out to you via email with a blank template in the format our system accepts. After you've exported your data as CSV from your existing tool, simply ensure that the data in the columns of our template match how Shortcut expects data. Here's a list of the field columns we accept via CSV, as well as their definitions and possible value/restrictions:

| **Field**         | **Content**                                                                                                            | **Notes**                                                                                                                                                                                                          |
| ----------------- | ---------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| name              | Title of the Story                                                                                                     | <p><em><strong>Required field</strong></em>.</p><p>5,000 character limit</p>                                                                                                                                       |
| id                | A reference on the story to an External ID. This can be used to help track the ID the story had in the source platform | Numerical values only.                                                                                                                                                                                             |
| state             | The state the Story currently resides in                                                                               | <p><em><strong>Required field</strong></em></p><p>This value can be mapped to an existing Shortcut state during import.</p>                                                                                        |
| type              | The type of Story that is being imported. Story types can be feature, bug, or chore                                    | _**Note: only feature, bug, or chore string values will import into shortcut as story types.**_ Any other string value will default to feature story stype.                                                        |
| requester         | The person who requested (e.g. created) the Story                                                                      | <p>Email Address, Name, or username is acceptable.</p><p>You will be able to map this user to an existing Shorcut user during or post-import.</p>                                                                  |
| owners            | The name(s) of the user(s) who own the Story                                                                           | Email Address, Name, or username is acceptable.                                                                                                                                                                    |
| description       | The content that will be used to describe the Story                                                                    | <p>20,000 character limit. </p><p>Supports Markdown and light HTML.</p>                                                                                                                                            |
| labels            | Tags that you can associate with your Stories                                                                          | <p>Separate multiple labels by semi-colon</p><p>Example: <code>Label A;Label B;Label C</code></p>                                                                                                                  |
| external\_tickets | Linked URLs associated with the Story                                                                                  | "https://shortcut.com" for example                                                                                                                                                                                 |
| created\_at       | The date the Story was created                                                                                         | <p>Format: <code>yyyy/MM/dd HH:mm:ss</code></p><p>Example: <code>2023/03/18 15:44:18</code> </p><p>If empty or omitted, the created date will default to today’s date.</p><p>Future dates are not allowed.</p>     |
| started\_at       | The date the Story was started                                                                                         | <p>Format: <code>yyyy/MM/dd HH:mm:ss</code></p><p>Example: <code>2023/03/18 15:44:18</code> </p><p><br>Future dates are not allowed.</p>                                                                           |
| is\_completed     | Confirmation that the Story is done                                                                                    | This is a boolean TRUE or FALSE field.                                                                                                                                                                             |
| completed\_at     | The date the Story was completed                                                                                       | <p>Format: <code>yyyy/MM/dd HH:mm:ss</code></p><p>Example: <code>2023/03/18 15:44:18</code> </p><p><br>Future dates are not allowed.</p>                                                                           |
| due\_date         | The date the Story is due                                                                                              | <p>Format: <code>yyyy/MM/dd HH:mm:ss</code></p><p>Example: <code>2023/03/18 00:00:00</code> </p><p><br>Past and future dates are allowed.</p>                                                                      |
| epic              | The name of the Epic the Story belongs to (Note: Stories do not map to existing Epics, a new Epic will be created)     | <p>Alphanumeric value accepted.</p><p>In Shortcut, <a href="https://help.shortcut.com/hc/en-us/articles/360045483932-Single-Epic-Page">Epics</a> are a collection of stories that represent large initiatives.</p> |
| epic\_created\_at | The time the Epic was created                                                                                          | <p>Format: <code>yyyy/MM/dd HH:mm:ss</code></p><p>Example:<code>2023/03/18 15:44:18</code></p><p><br>Future dates are not allowed.</p>                                                                             |
| tasks             | To-do items to add to the Story                                                                                        | <p>String format for each item. Example:</p><p><code>[X] task 1;[ ] task 2</code></p><p>The X represents a completed task.</p>                                                                                     |

At this time, the CSV import does not support Custom Fields, Teams, Objectives, or Iterations. However, these may be assigned post-import by bulk editing imported stories accordingly.

#### Here's an example of a filled-out template: <a href="#h_01h9670187bx7rb34t4yvwg5jx" id="h_01h9670187bx7rb34t4yvwg5jx"></a>

![](https://help.shortcut.com/hc/article_attachments/38100964175380)

_Click the image to enlarge_

Send your completed CSV file back to Support, and we will start the import process for you!

### Mapping Stories & Users During Import <a href="#h_01h96701870jcjmcbsgsnz35t1" id="h_01h96701870jcjmcbsgsnz35t1"></a>

Once you've sent Support your CSV file with the data filled as per the values outlined above, you're ready to go! Once support uploads the CSV file in the backend, you will be notified that the imported data is ready to be mapped via the bottom right corner once you log back into Shortcut:

![mceclip0.png](https://help.shortcut.com/hc/article_attachments/15296566965140)

#### Map to Existing Workflow and Workflow States <a href="#h_01h9670187erkp92an99rhzzyr" id="h_01h9670187erkp92an99rhzzyr"></a>

![Screen\_Recording\_2023-05-01\_at\_10.31.27.04\_PM.gif](https://help.shortcut.com/hc/article_attachments/15296664547860)

In the following screens, you will be able to choose which workflow and workflow states these stories will be imported into.

You can currently import the stories you provided in the CSV to a Single Workflow at a time. We recommend importing all stories into a workflow and then bulk-editing them into their correct workflow/workflow state afterward.

If you have a large number of stories that would make bulk editing unrealistic, we recommend sending Support a _separate_ CSV file. You may then import the stories in their corresponding workflow and workflow states separately.

#### Map Imported Users to Existing Shortcut Users <a href="#h_01h9670187m5frbhk2k2vjcnek" id="h_01h9670187m5frbhk2k2vjcnek"></a>

![](https://help.shortcut.com/hc/article_attachments/15296750692884)

The last step is to map the users you added to the `requester` or `owner` fields to existing Shortcut users.

If the user does not yet exist in Shortcut, we recommend first inviting them via **Settings** > **Invite New Users**. Then navigate back to **Settings** > **Import / Sync** > _Past Import tab_, and map the users there.

#### Success! <a href="#h_01h9670187vw53375pehxhjnqt" id="h_01h9670187vw53375pehxhjnqt"></a>

![w\_900.png](https://help.shortcut.com/hc/article_attachments/15296863066260)

Once the import has been completed, your data is now in Shortcut!

We highly recommend bulk editing the Stories to move them and assign new Fields, Owners, etc. accordingly.
