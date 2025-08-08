# Google Sheets integration

### Google Sheets Integration

Our Google Sheets integration allows for real-time updates of [Shortcut](https://www.shortcut.com/) data to be sent to a Google Sheet. Once set up, any updates that happen in your Shortcut Workspace will be dynamically updated in your Google Sheet. The time zone for the Google Sheets integration is based off of the workspace's UTC offset.

Your Google Sheet integration can be linked to any BI tool that ingests Google Sheets, allowing you to visually model your Shortcut data and unlock custom analytics in real-time.&#x20;

To ensure proper data accuracy:

* **Don't** rename the sheet/tab (You may create additional sheets/tabs)\

* **Don't** delete or reorder columns\

* **Don't** add new columns\

* **Don't** change cell values\

* **Don't** use the "Filter" feature to re-sort, filter, or hide rows

You may:

* Hide columns\

* Create new sheets that cross-reference for any additional sorting or filtering needs

**Note:** the integration re-syncs to the specific Story, it does not re-sync the entire Worksheet each time.

The data that is sent from Shortcut to Google is the same data represented when you [manually integrate Workspace data to CSV](https://help.clubhouse.io/hc/en-us/articles/360044295392-Importing-and-Exporting-Clubhouse-Data)

Currently, you can only have one Google Sheet per Workspace.

### Enabling the Google Sheets Integration <a href="#h_01hayx0adjsr7nsewahq9a03n9" id="h_01hayx0adjsr7nsewahq9a03n9"></a>

To enable the Google Sheets Integration navigate to your **Integrations** <> **Google Sheets Integration** (if you haven't upgraded to a paid plan you will need to do so in order to access the integration).&#x20;

* Select **Integrations**
* Select **Google Sheets**
* **Authorize** with Google
* Yahtzee - you're done!

We'll create a new Google Sheet with a _live_ connection to your Shortcut data. Each row will contain rich Story data and all changes within Shortcut will override the existing information for that particular element within the Google Sheet. **The sheet is private to you**, but you can share it with a wider audience as you see fit.&#x20;

### Disabling the Google Sheets Integration <a href="#h_01hayx0xe9ctc701xpd1czjbtr" id="h_01hayx0xe9ctc701xpd1czjbtr"></a>
