# VCS Event Handlers

With the Shortcut VCS integrations, you can move your stories across the Shortcut board while staying in your regular VCS workflow.

![Event Handlers](https://help.shortcut.com/hc/article_attachments/32877306415252)

After configuring your organization's VCS integration, navigate to **Integrations > VCS of choice** and over to the **Event Handlers section.** \


1. Select "Add New Event Handler".&#x20;
2. Select the VCS event you would like to listen for. We currently support:
   * **Branch associated with Story**
   * **Branch merged**
   * **Commit associated with Story**
   * **Pull Request approved**
   * **Pull Request labeled** (not available for Bitbucket Cloud)
   * **Pull Request opened**
   * **Pull Request review requested** (not available for Gitlab.com)
3. Enter the name of the branch where this event will occur or the label name, where appropriate. Examples we use are "development", "product", or "trunk", but you may be using a multi-branch development workflow.
4. Select the workflow state you would like the linked story to move to.&#x20;
5. Click "Add New Event Handler" again to save.&#x20;

Your stories will now automatically update as you follow your [development workflow](https://help.clubhouse.io/hc/en-us/articles/207540323-Using-The-Clubhouse-GitHub-Integration), and merge events will affect commits as well as pull requests.

#### Pending work and our Event Handlers <a href="#h_01jen78fh31cjf6zfwfnwrw3ck" id="h_01jen78fh31cjf6zfwfnwrw3ck"></a>

Our integration can detect “open work” that’s associated with a Story when determining when to execute our “PR Opened” or “Branch Merged” event handler. If any open work exists, then the handler is not invoked.&#x20;

What constitutes “open work”?&#x20;

1. Another open Pull Request being associated with the Story other than the PR that is triggering the event. If you have multiple PRs associated with a Story, taking action with just one of them will not move the Story forward.
2. A non-deleted, non-merged Branch other than the branch that led us to the Story from the event (this could be a branch that we found via the tree of merges (in which case it would be merged already) on a push event or the branch for a PR from a PR event.
