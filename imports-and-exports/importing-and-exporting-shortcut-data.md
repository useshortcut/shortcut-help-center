# Importing and Exporting Shortcut Data

Look for the "Export as CSV" prompt to export all of the Stories from a single Workspace, Iteration, Epic, Label, or Project.

* To Export all Stories in a Workspace as CSV, that option is located on [your Organization and Workspace dashboard](https://app.shortcut.com/organizations).



* If seeking to export a CSV of a specific set of Stories, such as from an Epic, Iteration, or Label for example, that Export as CSV option is located in the top right of the Stories Table.



* To export a filtered Space on the new Stories page, the Export option is within the dropdown for that Space.

![](https://help.shortcut.com/hc/article_attachments/36301529824020)

#### All exports include the following information about each Story:  <a href="#h_01j53m3tzq6d4fhfme4zp0y3ht" id="h_01j53m3tzq6d4fhfme4zp0y3ht"></a>

| **Column**                 | **Description**                                                                                                            |
| -------------------------- | -------------------------------------------------------------------------------------------------------------------------- |
| id                         | Story ID                                                                                                                   |
| name                       | Story Name                                                                                                                 |
| type                       | Story Type                                                                                                                 |
| requester                  | Story Requester                                                                                                            |
| owners                     | A list of Story Owners, if assigned                                                                                        |
| description                | Story Description                                                                                                          |
| is\_completed              | TRUE/FALSE boolean noting if a Story has been Completed                                                                    |
| created\_at                | The date and time the Story was created                                                                                    |
| started\_at                | The date and time the Story was moved to a Started state                                                                   |
| updated\_at                | The date and time of the last update to the Story                                                                          |
| moved\_at                  | The date and time that the Story last changed states                                                                       |
| completed\_at              | The date and time the Story was moved to a Completed state                                                                 |
| estimate                   | Estimate points for the Story, if assigned                                                                                 |
| external\_ticket\_count    | Number of attached external tickets                                                                                        |
| external\_tickets          | The URLs of the attached external tickets                                                                                  |
| is\_blocked                | TRUE/FALSE boolean noting if a Story is blocked by another Story                                                           |
| is\_a\_blocker             | TRUE/FALSE boolean noting if a Story blocks another Story                                                                  |
| due\_date                  | The due date of the Story                                                                                                  |
| labels                     | List of Labels applied to the Story. \*Note\* These are only Story Labels. Epic Labels will not be displayed in this list. |
| epic\_labels               | List of Epic Labels for the Epic a Story is associated with.                                                               |
| tasks                      | List of Tasks in a Story. Completion is marked with an X, and the Task owner (if assigned) is included.                    |
| state                      | Workflow state of the Story when the download was initiated                                                                |
| epic\_id                   | ID of Epic the Story is in (if any)                                                                                        |
| epic                       | Epic Name                                                                                                                  |
| epic\_label                | Epic labels that are linked to the story                                                                                   |
| project\_id                | ID of the Project the Story is in                                                                                          |
| project                    | Project Name                                                                                                               |
| iteration\_id              | ID of the Iteration that the Story belongs to, if it belongs to one                                                        |
| iteration                  | Name of the Iteration that the Story belongs to, if it belongs to one                                                      |
| utc\_offset                | The user's UTC offset, which affects the times displayed (this is different than the Organization UTC offset)              |
| is\_archived               | TRUE/FALSE boolean noting if a Story has been archived                                                                     |
| team\_id                   | Team ID for the Team that is associated with the Story                                                                     |
| team                       | Team name that is associated with the Story                                                                                |
| epic\_state                | Workflow State of the Epic                                                                                                 |
| epic\_is\_archived         | TRUE/FALSE boolean noting if an Epic has or has not been archived                                                          |
| epic\_started\_at          | The date and time the Epic was moved to a Started state                                                                    |
| epic\_due\_date            | The due date of the Epic                                                                                                   |
| epic\_created\_at          | The date and time the Epic was created                                                                                     |
| objective\_id              | ID of the Objective                                                                                                        |
| objective                  | Name of the Objective                                                                                                      |
| objective\_state           | Workflow State of the Objective                                                                                            |
| objective\_created\_at     | The date and time the Objective was created                                                                                |
| objective\_started\_at     | The date and time the Objective was moved to a Started state                                                               |
| objective\_due\_date       | The due date of the Objective                                                                                              |
| objective\_categories      | The categories created an Objective                                                                                        |
| epic\_planned\_start\_date | The Start Date set for an Epic                                                                                             |
| workflow                   | The name of the Workflow that a Story is in                                                                                |
| workflow\_id               | Public ID of the Story's Workflow                                                                                          |
| priority                   | The Priority Field values associated with a Story                                                                          |
| severity                   | The Severity Field values associated with a Story                                                                          |
| product\_area              | The Product Area Field values associated with a Story                                                                      |
| skill\_set                 | The Skill Set Field values associated with a Story                                                                         |
| technical\_area            | The Technical Area Field values associated with a Story                                                                    |
| custom\_fields             | The Advanced Custom Field Values associated with a Story                                                                   |
