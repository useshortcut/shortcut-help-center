# Importing data from Trello to Shortcut

Bringing the work your team has completed with you has never been easier. Your progress, history, insights, and all the wins you’ve made together in Trello can now be imported directly into Shortcut.

We’ll work to improve every facet of this import process using your direct feedback and insights along the way. Ready to get started?

**Team Preparation**

We’re excited to start this process with you! Let’s start by making sure you’ve considered the following:

* Ensuring you have proper Administrative permissions in Trello and Shortcut
* Speaking with the various teams on your side associated with the data you’re importing to ensure that you have a working knowledge of their needs

_Tip: We’ve heard collecting your import information in a spreadsheet can streamline this process._

### **Requesting Import Permissions** <a href="#h_01hmchr8sdpt2jgyzsrc57pb71" id="h_01hmchr8sdpt2jgyzsrc57pb71"></a>

Within Shortcut, we start by asking your team to set up permissioning that allows us to talk freely to Trello. Here’s what you’ll need to start the process:

* Your unique Trello **Auth Key**
* A unique **Auth Token** (can be revoked immediately after import process completes)

Your Auth Key helps our importer connect to the right Trello instance, and your Auth Token lets Trello know that we have permission to read and transfer your files.

To generate both of these, follow the steps below:

1. Login and navigate to "Power Up" [https://trello.com/power-ups/admin](https://trello.com/power-ups/admin)
2. Generate a new Auth Key and Token by selecting "New" on the dashboard main page, and follow the steps to generate a new Auth Key
3. Follow the embedded link to generate the Auth Token:

![Screenshot 2024-02-12 at 11.32.08 AM.png](https://help.shortcut.com/hc/article_attachments/23900482192660)

For more detailed information, please visit Atlassian's documentation: [https://developer.atlassian.com/cloud/trello/guides/rest-api/authorization/](https://developer.atlassian.com/cloud/trello/guides/rest-api/authorization/)&#x20;

### **Mapping** <a href="#h_01hmchre918ngqt7jr06dcv1j9" id="h_01hmchre918ngqt7jr06dcv1j9"></a>

Let’s dig into the heart of the import process - telling your Trello data where it will now live in Shortcut. We recommend working through this part as a team when possible to ensure that everyone is comfortable with where their data will be mapped.

Here's what you'll need to have handy:

* **Trello Board ID(s):** These are found within the URL of the board or boards you’re looking to import. Look for a number just like this from a logged-in view of Trello:

![Screen\_Shot\_2020-06-23\_at\_7.50.11\_AM.png](https://help.shortcut.com/hc/article_attachments/360060322931)

* **Board Name(s):** This helps us organize the data during the process and helps to keep the import readable.\

* **Target Shortcut Workspace name:** Which Workspace will this data be added into?
* **Target Shortcut Workflow(s) for each Board:** All cards from a Trello Board will be mapped directly into an existing Shortcut Workflow.
* **User Mapping:** Which Trello Users should be mapped to existing Shortcut Users? Which users can’t be mapped, and need an invite to Shortcut?
* **Default Story Requestor:** If we cannot find a Trello Card creator, which Shortcut User should be the fallback Story Requestor? (usually, this is the user running the import)

### **What else will be imported from Trello?** <a href="#h_01hmchrk1he7e41xfvx4wp1c5h" id="h_01hmchrk1he7e41xfvx4wp1c5h"></a>

In addition to the core functionality, we’re also excited to announce that the following data will also be imported:

*
  * Card Descriptions
  * Designations (Owners, Requesters/Creators, and Followers)
  * Labels
  * Comments
  * Attachments
  * Due Dates
  * Custom Fields (imported as Shortcut Labels)
  * Checklists (imported as Shortcut Tasks on a Story)

### **Mapping Logic**  <a href="#h_01hmchrpak1yx9dcbyh2x2why8" id="h_01hmchrpak1yx9dcbyh2x2why8"></a>

### **Bulk Editing Imported Data** <a href="#h_01hmchrswbxg6p79jk029shw73" id="h_01hmchrswbxg6p79jk029shw73"></a>

We find that our teams are able to easily find homes for the various values you’ve brought in by using our bulk editing functionality.

To read a little more about how to edit and assign large groups of Stories, please check out our article here on [Bulk Editing Multiple Stories](https://help.clubhouse.io/hc/en-us/articles/360044698631).

### **Reverting Imports** <a href="#h_01hmchrx7r8vd882b2vr9b2z52" id="h_01hmchrx7r8vd882b2vr9b2z52"></a>

Need to regroup after an import? Not to worry - we’ve made sure that Imports can be reverted. This will delete all Stories, Labels, and Users created during the import to give your team a clean slate and restore your Shortcut instance back to before the import process was started.

To request that your import be reverted, please create a new ticket [here](https://help.clubhouse.io/hc/en-us/requests/new) with the subject “Revert Trello Import” for the fastest support.

### **Need to Run a Second Import?** <a href="#h_01hmchs0fyjcbj3ht3we8ackxk" id="h_01hmchs0fyjcbj3ht3we8ackxk"></a>

Running a second import will create new stories for Trello cards that have already imported, resulting in duplicates.

There are a few of options to get those additional cards into Shortcut as Stories:

1. Create a new Trello board, move the new cards there, then import just that board (this is the easiest option, but note that these won’t be in the proper board in Trello, if that matters.)
2. Rollback the prior import completely and re-import to get the new stories (Note that this will cause any changes done on the Stories that were part of the prior import to be lost)
3. Do a new full import into a different board, then move the net new stories to the correct project, followed by a deletion of the remaining duplicates - very manual or would require scripting!
4. Create new Stories manually in Shortcut for the new tickets in Trello.
