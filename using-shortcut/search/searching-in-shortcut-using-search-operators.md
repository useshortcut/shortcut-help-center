# Searching in Shortcut: Using Search Operators

Story search queries will look for matches in Story titles, descriptions, and comments. By default, all queries will use `AND` logic when combining multiple operators (`OR` logic is not available in Search at this time, but it is available [when filtering on the Stories page](https://help.shortcut.com/hc/en-us/articles/206296205-Filtering-the-Stories-Page)).

There are two categories of search operators available when searching for Stories: [Story-specific search operators](https://help.shortcut.com/hc/en-us/articles/360000046646#heading-1) (which will find results only for Stories), and [general search operators](https://help.shortcut.com/hc/en-us/articles/360000046646#heading-2) (which will find results across Stories, Epics, and Objectives).

### Story-Specific Search Operators <a href="#h_01hj1ctqef0npqpc49rd6zv2wm" id="h_01hj1ctqef0npqpc49rd6zv2wm"></a>

| **type:**                              | Finds all Stories of a specific type (feature, bug, or chore). A query that contains more than one unique type operator will yield no results.                                                                                   |
| -------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **estimate:**                          | Finds all Stories of a specific point value. This is a numeric value, i.e. _`estimate:4`_. See our [Estimate Scale](https://help.shortcut.com/hc/en-us/articles/209984986) article for more information about point estimations. |
| **has:attachment**                     | Finds all Stories with attachments. This operator only searches for attached files, not anything pasted or uploaded in comments                                                                                                  |
| **has:task**                           | Finds all Stories with tasks                                                                                                                                                                                                     |
| **has:epic**                           | Find all Stories added to an Epic                                                                                                                                                                                                |
| <p><strong>has:branch</strong><br></p> | Find all Stories that have a VCS branch associated                                                                                                                                                                               |
| <p><strong>has:commit</strong><br></p> | Find all Stories that have a VCS commit associated                                                                                                                                                                               |
| <p><strong>has:pr</strong><br></p>     | Find all Stories that have a VCS pull request associated                                                                                                                                                                         |
| <p><strong>branch:</strong><br></p>    | Find all Stories that have a VCS branch with the given name associated                                                                                                                                                           |
| <p><strong>commit:</strong><br></p>    | Find all Stories that have a VCS commit with the given full hash or url associated                                                                                                                                               |
| <p><strong>pr:</strong><br></p>        | Find all Stories that have a VCS pull request with the given number or url associated                                                                                                                                            |
| **is:blocked**                         | Finds all Stories that have been marked using [Story Relationships](https://help.shortcut.com/hc/en-us/articles/360044391911-Contents-of-a-Story) as blocked by another Story                                                    |
| **is:blocker**                         | Finds all Stories that have been marked using [Story Relationships](https://help.shortcut.com/hc/en-us/articles/360044391911-Contents-of-a-Story) as blocking another Story.                                                     |
| **is:story**                           | Returns only Stories in search results.                                                                                                                                                                                          |

### General Search Operators  <a href="#h_01hj1ctqefwnbe0d3sr72d1vrw" id="h_01hj1ctqefwnbe0d3sr72d1vrw"></a>

### id: <a href="#h_01hj1d5e5pwfhh3qhysq99jw5k" id="h_01hj1d5e5pwfhh3qhysq99jw5k"></a>

* `id:123`

### title: <a href="#h_01f6r3erv2t7s5azts4zzd9vaq" id="h_01f6r3erv2t7s5azts4zzd9vaq"></a>

Searches Story, Epic, Objective, and Iteration titles:

* `title:hello` will search for "hello" in titles of stories and epics.
* `title:"hello world"` will search for "hello world" in titles.
* `title:hello world` will search for "hello" in titles  _AND_ "world" in titles/descriptions/comments.

### description: <a href="#h_01f6r3f3mqj8ja698m28yxye0j" id="h_01f6r3f3mqj8ja698m28yxye0j"></a>

Searches Story, Epic, and Objective descriptions:

* `description:hello` will search for "hello" in description of stories and epics.
* `description:"hello world"` will search for "hello world" in descriptions.
* `description:hello world` will search for "hello" in descriptions _AND_ "world" in titles/descriptions/comments.

### comment: <a href="#h_01f6r3fghfr48zs2kbe5jbfcbw" id="h_01f6r3fghfr48zs2kbe5jbfcbw"></a>

Searches Story and Epic comments.

* `comment:hello` will search for "hello" in comments of stories and epics.
* `comment:"hello world"` will search for "hello world" in comments.
* `comment:hello world` will search for "hello" in comments _AND_ "world" in titles/descriptions/comments.

### project: <a href="#h_54b5ccde-38af-456b-806e-0f229d8ad9eb" id="h_54b5ccde-38af-456b-806e-0f229d8ad9eb"></a>

Finds Stories in a specific Project (may use the Project name or Project ID). Or Epics with stories in a specific Project. For best results, queries for multi-word Project titles should be placed in double-quotes.

* `project:frontend`
* `project:"growth hacks"`

\* Please note that Projects is a Legacy feature and may not be available or enabled in your Workspace. \*

### epic: <a href="#h_50a9a10a-e19e-40f1-a466-60b20fae6b8f" id="h_50a9a10a-e19e-40f1-a466-60b20fae6b8f"></a>

Finds all Stories in a specific Epic. For best results, queries looking for an exact match should be placed in double-quotes.

* `epic:growth` will find all stories in epics that contain "growth" in their title
* `epic:"growth hacks"`

### objective: <a href="#h_78ae65e1-b9f6-44a1-8d67-b6a220eb5a02" id="h_78ae65e1-b9f6-44a1-8d67-b6a220eb5a02"></a>

Finds all Stories in the Epics within a specific Objective. For best results, queries for multi-word Objective titles should be placed in double-quotes.

### state: <a href="#h_e37b1f77-d062-46c6-8cab-1e2601bee6d3" id="h_e37b1f77-d062-46c6-8cab-1e2601bee6d3"></a>

Finds all Stories in a specific Workflow state. For best results, queries for multi-word workflow state titles should be placed in double-quotes.

* `state:"ready for dev"`
* `state:completed`

### Searching across Workflow States with is: <a href="#h_01hj1ctqege8zqab7wqr4rcg2w" id="h_01hj1ctqege8zqab7wqr4rcg2w"></a>

In addition to the **state:** operator, the following operators search over the different types of [workflow states](https://help.shortcut.com/hc/en-us/articles/205268889-Setting-Up-Your-Organization-s-Workflow).

Since stories can only have one workflow state, using more than one of these operators can yield no results.

* `is:unstarted`
* `is:started`
* `is:done`

### label: <a href="#mention" id="mention"></a>

Finds all Stories or Epics with a specific Story label. For best results, queries for multi-word labels should be placed in double-quotes.

* `label:"needs copy"`
* `label:release`

Note: Stories in an Epic do not inherit the Epic labels.

### owner: <a href="#h_01hqty7c4at6tytdgebr58g1fp" id="h_01hqty7c4at6tytdgebr58g1fp"></a>

Finds all Stories or Epics owned by a user. This query requires the user's full mention name (also known as their @-name) to work. Do not include the @ symbol at the beginning of the mention name.

Suggestions will be provided once the first few letters are typed.

* `owner:johnsmith`
* `owner:bartsimpson`

### requester: <a href="#h_d832aaf8-986c-4d18-92b0-a1e2df160d97" id="h_d832aaf8-986c-4d18-92b0-a1e2df160d97"></a>

Finds all Stories or Epics requested by a user. This query requires the user's full mention name (also known as their @-name) to work. Do not include the @ symbol at the beginning of the mention name.

* `requester:johnsmith`
* `requester:bartsimpson`

### team: <a href="#h_01hj1exj5tray80kv2jrdx27xv" id="h_01hj1exj5tray80kv2jrdx27xv"></a>

Finds all Stories, Epics, and Iterations associated with a specific Team. Enter the Team's Name directly following `team:`. Note: This is _not_ the team's Mention Name.

For example: To return only Epics owned by the Engineering team, you could do `is:epic team:Engineering`. For a team named Product Development, you would use `team:"Product Development"`.

### Custom Fields: <a href="#h_01hw8e69pwym51datxvq64brh0" id="h_01hw8e69pwym51datxvq64brh0"></a>

Find all Stories that contain one or more of the following Shortcut Defined Custom Fields

\* Please note that Advanced Custom Fields are not able to be entered as a Search Operator at this time. \*

* `skill-set:`
* `product-area:`
* `technical-area:`
* `priority:`
* `severity:`

### Inversions and Exclusions: <a href="#h_c49fcfe8-08a0-47d2-a5a8-f732233bafa9" id="h_c49fcfe8-08a0-47d2-a5a8-f732233bafa9"></a>

Of note, you can search for the inverse or exclude an operator by adding an **!** or **-** in front of the operator. This is equivalent to a **NOT** boolean operator.

For example, i.e. _`!has:comment`_ and _`-has:comment`_ will return Stories with no comments.

### Dates and Date Ranges: <a href="#date" id="date"></a>

First, it's important to use the correct date formatting in your searches. The format [Shortcut](https://www.shortcut.com/) recognizes is 4 digit year-2 digit month-2 digit day:

* `YYYY-MM-DD`

When searching for a date range, separate your dates with two periods:

* `YYYY-MM-DD..YYYY-MM-DD`

You can make your date range open-ended (or unbounded, in search parlance) by adding an asterisk (**\***) on one side of the range.&#x20;

An asterisk on the left side of the date range would find you all Stories **before** the specified date:

* `*..YYYY-MM-DD`

And an asterisk on the right side of the date range would find you all Stories **after** the specified date:

* `YYYY-MM-DD..*`

You can also search using the terms **yesterday** and **today**, as well as **tomorrow** (but this latter term can only be used when searching for due dates, more on this below).

Please note that numerical date values and date terms currently can't be mixed -- so a search for   `2018-04-01..today` is not valid.

### Date-Based Operators: <a href="#h_01hravrynft0tjj59nw6smw0y2" id="h_01hravrynft0tjj59nw6smw0y2"></a>

You can search for Stories that have been created, updated, completed, or moved using a specified date or date range, or the terms **yesterday** or **today**.

You can also search for Stories that are (or were) due on a specified date or date range, or using the terms **yesterday**, **today**, or **tomorrow**&#x20;

* `created:2023-01-01`
* `updated:today`
* `completed:yesterday`
* `moved:*..2023-02-01`
* `due:tomorrow`

When using the **updated:** operator, keep in mind that it asks "What Stories or Epics were _**last**_ updated on/before/after this date or within this date range?"

The **moved:** operator will only find Stories that have changed workflow state (i.e., those which have "moved" to a different workflow state column) on or within a specified time period.

### The \`has:\` and \`is:\` Operators: <a href="#estimate" id="estimate"></a>

* `has:`

| **has:comment**  | Finds all Stories with comments.   |
| ---------------- | ---------------------------------- |
| **has:label**    | Finds all Stories with a label.    |
| **has:deadline** | Finds all Stories with a due date. |
| **has:owner**    | Finds all Stories with an owner.   |

* `is:`

| **is:unestimated** | Finds all Stories with a point value of 0 (in other words, Stories with no point estimation). |
| ------------------ | --------------------------------------------------------------------------------------------- |
| **is:overdue**     | Finds all Stories with a due date in the past.                                                |
| **is:archived**    | Finds all archived Stories.                                                                   |
| **is:epic**        | Finds only Epics (does not work as expected when on the Advanced Search page)                 |
