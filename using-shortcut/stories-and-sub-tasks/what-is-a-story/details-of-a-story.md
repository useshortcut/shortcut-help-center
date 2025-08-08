# Details of a Story

### Details of a Story

![Story Details](https://help.shortcut.com/hc/article_attachments/14730807963924)

Stories are the standard unit of work in Shortcut. Stories are where collaboration and documentation for said unit of work happens.

Think of the right side bar of a story as it's attributes. It allows you to designate the type of a story, the project it belongs to, as well as who is to work on it. In addition, you can specify which Epic the story is a part of, it's due date, and even associate custom label(s) make finding and/or reporting easier. This article will break down these attributes by their respective elements.

### Story Fields

*   The State, or Workflow State, refers to the to name of a particular workflow step. Stories move through workflow states in order to be completed.

    The drop-down in the Story dialog allows you to quickly move a story from one workflow state to another.
*   Teams typically map to groups of people that focus on certain areas of work (e.g. Frontend, Backend, Product, Design, etc). Teams can also be used to refer to open-ended projects or company initiatives.

    The drop-down in the Story dialog allows you to quickly select a Team and assign it to the Story. Keep in mind that because [Teams and Workflows are linked](https://help.shortcut.com/hc/en-us/articles/4407290960916), choosing a Workflow will filter the Teams accordingly.
*   [Epics are collections of stories](https://help.shortcut.com/hc/en-us/articles/360017524632) that represent a large amount of work.

    You can assign a story to specific Epic right from the Epic drop-down. If you are unable to find an Epic after entering the text in the drop-down, Shortcut will allow you to create a new Epic based on that term right from the drop-down and immediately assign it to the story in question.

    Additionally, you can immediately navigate to that Epic after assigning to the story by clicking on the View Epic Page button next to the Epic's name.

    ![Epic navigation from Story](https://help.shortcut.com/hc/article_attachments/14834985118740)
*   An [Iteration](https://help.shortcut.com/hc/en-us/articles/360028953452) (aka Sprints) is a defined, time-boxed period of development for a collection of Stories. In Shortcut, Iterations can span multiple Epics, Projects, and Workflows.

    The drop-down allows you to select which iteration the story should belong to.
*

    ![Story Type](https://help.shortcut.com/hc/article_attachments/14835001838868)

    There are 3 types of stories in Shortcut: **Features**, **Bugs**, and **Chores**. Features are enhancements to the product. Bugs are issues that disrupt the usability of the product. Chores are any work that has to be completed but does not quite fall within the aforementioned types.&#x20;

    You can quickly change the type of a story from the drop-down at any time.
*

    ![Story Requester](https://help.shortcut.com/hc/article_attachments/14835005384724)

    When you create a Story, you are automatically assigned as the Requester. You can change the requester in the Story dialog if you would like someone else to be credited as Requester.

    Requesters are automatically added as **Followers.**
*   Owners are the people who will be doing the actual work outlined in the Story and tasks. While some teams like to determine an Owner upon Story creation, others wait until the work is ready for development and moved into a Started workflow state to determine an Owner.

    ![Story Owners](https://help.shortcut.com/hc/article_attachments/14835063201300)

    Owners are automatically added as Followers to the Stories that they own and will receive all notifications of changes in Story status.
*   Shortcut allows stories to be estimated using points, and supports any whole number as an estimate.

    ![Story Estimate](https://help.shortcut.com/hc/article_attachments/14835082779540)

    The numbers in the drop-down are based on the workspace's estimate scale [set in settings](https://help.shortcut.com/hc/en-us/articles/209984986-Workspace-Settings).
*   The Story's due date represents when work for this story is expected to be completed. Due date can be changed at any time from the story dialog.

    In addition to being able to search for stories by when due date, the date of stories is used to showcase upcoming due stories in [your personal dashboard](https://help.shortcut.com/hc/en-us/articles/205630749).
*

    ![Story Followers](https://help.shortcut.com/hc/article_attachments/14835091125652)

    Followers are users who receive all notifications of changes in Story status.&#x20;

    Story requesters and owners are automatically added as followers. If you no longer wish to be a follower, simply de-select your name from the Followers dropdown.

    Additionally, whenever you add a comment to a Story, you will be automatically made a Follower of the Story, if you aren't already.
*

    ![Custom Fields](https://help.shortcut.com/hc/article_attachments/14835317068308)

    [Custom Fields](https://help.shortcut.com/hc/en-us/articles/4423932934804) are a sophisticated method of categorizing Stories according to defined attributes (e.g. Product Area, Skill Set, etc).

    You can assign Custom Fields to a Story by selecting the appropriate Custom Field and then selecting a value from the dropdown menu.

    Custom Fields can be managed by a Workspace Admin under Settings > Workspace Features > Custom Fields.
*   [Labels](https://help.shortcut.com/hc/en-us/articles/205702619) are a way to associate Stories. You can filter against Labels throughout various Shortcut views and search for Stories that carry them in the Stories filter section and on the Search page.

    ![Story Labels](https://help.shortcut.com/hc/article_attachments/14835123217940)

    You can assign labels from the drop-down in the story after clicking _Add Labels_. If you are unable to find a label after entering the text in the drop-down, Shortcut will allow you to create a new label based on that term right from the drop-down and immediately assign it to the story in question.

### Assigning an Owner

If you wish to assign an Owner or multiple Owners, you can make the change in the Owners dropdown in the Story dialog.

![Assigning Story Owners](https://help.shortcut.com/hc/article_attachments/14835164139156)

You can also remove Owners in this dropdown.

If a story does not have an Owner when it is dragged or changed over from an Unstarted to a Started workflow state, the person who makes that change will be assigned as the Owner.

If a story is created in a Started state, the person who created the Story will be assigned as its Owner by default.

### Enable or Disable Automatic Story ownership

When new Stories are added, they default to being Unstarted and without Owners.

If a story does not have an Owner when it is dragged or changed over from an Unstarted to a Started workflow state, **the person who makes that change will be assigned as the Owner.**

If a story is created in a Started state, the person who created the Story will be assigned as its Owner by default.

This behavior can, however, be disabled by navigating to Settings > Workflow States > Select the Workflow you wish from the drop-down > Uncheck ![mceclip7.png](https://help.shortcut.com/hc/article_attachments/360058578712/mceclip7.png)
