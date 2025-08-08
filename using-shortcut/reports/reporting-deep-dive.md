# Reporting Deep Dive

### Reporting Deep Dive

#### Best practices for each Report type <a href="#h_01hnga936nmrjxa38rd7rh6jsm" id="h_01hnga936nmrjxa38rd7rh6jsm"></a>

Before we dive into each report type it is important to call out there are reports located on the Reports page and there are also reports on individual entity pages for Epics, Objectives, and Iterations. The difference in these reports is how Stories are counted. On the Reports page, all charts use completed Stories. "Completed" means stories moved into the "Done" workflow category which frequently includes a "canceled" state. You can see how your Workflows are configured [here.](https://help.shortcut.com/hc/en-us/articles/360016617052-Managing-Your-Workflows) This means the Reports page is very useful for historical reporting and measuring past performance. That is in contrast to the charts on the Entity pages (Epics, Objectives, and Iterations), which include all Stories. These reports are useful for in-progress metrics.

*   The Velocity Chart shows completed Stories broken down by Story type, which measures work completed for each interval. Velocity is not a metric to try to move on its own, but rather an input to be used in other planning.

    \
    A best practice for using the Velocity chart is to look for stability, this is an indicator of a good team rhythm. Empower your team to predict how quickly they can work through the backlog because the report tracks the forecasted and completed work over several sprints. The more sprints, the more accurate the forecast. The chart can be viewed as Story count or Story points, which allows you to extrapolate how many Story points your team can complete in a given amount of time. Together with other metrics and variables the Velocity chart can help to better plan and predict your team’s work for the next Sprint.

    **Velocity Chart Best Practices:**

    * Velocity Variation or Decrease- If you see a lot of variation in Velocity or decreasing Velocity indicates it’s a good time to start a conversation to identify things such as blockers, bugs, and problems with the practices within the team.
    * Group by Iteration- Good use of the velocity chart is noticing that velocity is decreasing over time when grouped by Iteration, which prompts the team to come together to discuss what issues they are facing.&#x20;
    * Velocity Chart on the Epics and Objective Pages- This will give you the ability to drill down the Velocity for each larger initiative. If you notice an Objective with volatile or decreasing Velocity you can drill down into the Objectives for clues on where there is room for improvement and conversation.
*   The Burndown Chart represents work left to do displayed over time. The remaining work can be represented by either points or Story count. This allows you to assess team progress on a regular basis. Changes from the expected burndown such as a large difference in Actual Points remaining and Ideal Points remaining or an unusually high increase in points added are an opportunity to drill down to find the root cause and fix it before it derails an entire sprint, or worse, a product release.

    \
    **The Burndown Chart on the Reports page:**

    * Look across initiatives- The reports page Burndown Chart is a great way to aggregate reports across Objectives and Epics.
    * Entities without reports- It is great for looking across entities that don't have reports on the entity pages such as by Team or owner. Just use the filters to adjust the chart as needed.

    **The Burndown Chart on the entity pages:**

    * Epics and Iterations Burndown Chart- If the Epic or Iteration is still in progress and has a set end date, we include a line showing the Ideal number of Stories/points that should be remaining in order to complete work on time. If the Epic or Iteration is still in progress without a set end date, we provide a forward-looking projection line based on the velocity of completed Stories/points.
    * Key use case- Use the Burndown Chart to see when you'll finish and if it's within your planned end date or not.
*   This chart allows you to look at both cycle time and lead time. Cycle Time is the total time between when a Story was started and when it was completed. Lead Time measures the time between when a Story was created and when it was completed.

    **Cycle Time Chart:**

    * Work Completion Predictions- Cycle times allow you to look at similar projects and provide data-driven predictions on the time it will take to complete similar projects. Lower cycle times mean you can better predict what work you can achieve. Basically, the less time it takes to do work, the better accuracy you have in that prediction.
    * Unstable cycle times- Chaotic or unstable cycle times can mean that team processes are not well established. This creates a good opportunity for discussion. On the other side, a stable cycle time indicates a team is working at a sustainable pace, and not encountering too many disruptions.
    * Custom- You have the option to view this chart in Type: Custom which allows you to select a specific workflow and the workflow states you would like include (or excluded). This is helpful for a custom workflow to ensure the data includes the correct stages.&#x20;

    \
    **Lead Time Chart:**

    * This chart can be interesting to view on the Epic page as it tells you how long Stories take to be completed for those specific initiatives.&#x20;
    * Backlog Considerations- Depending on how you manage your backlog this chart can end up being more or less impactful. A common way to manage backlog in Shortcut is through a “Backlog” workflow state, which depending on your team and process could mean the lead time is really long, and that’s okay!

    \
    **Cycle Time/Lead Time Chart Best Practices:**

    * Maintain Story Hygiene- The more defined your process is for moving Stories to completed, the more accurate your data will be. For cycle time, it's important to only move work to in-progress when it's actually ready (and move it back to unstarted if needed).
    * Filter on the Reports Page- Use these filters to drill into more targeted Cycle Time & Lead Time reporting around Dates, Teams, Story types, and more.&#x20;
    * Note the Trailing Average-  This will be the most insightful if you look at longer time periods.
    * Calculate how long Stories sit in an Unstarted State: Subtract Lead Time from Cycle Time.
*   Time Spent in Workflow State chart is the time completed Stories spent in each Workflow State and is a great way to uncover bottlenecks.

    \
    **Time Spent in Workflow State Chart Best Practices:**

    * Identify bottlenecks- A key indicator to pay attention to is if Stories are spending a lot of time in a particular state, this can help you identify bottlenecks or areas for process improvement. For example, if Stories are spending a lot of time in the "In Review" state this indicates the team may need to allocate more time to Peer Review or improve communication when a review is needed.&#x20;
    * Request for headcount- If Stories are spending a lot of time in a particular workflow state - we'll use QA as an example - it likely means the team's volume is outpacing the QA team's capacity.  Additional people may be needed.
    * Recommend changes to process- If Stories are spending little to no time in any particular state it indicates that the state is often being skipped. Could be that the state is unnecessary or that its importance needs to be highlighted to the team to ensure it's put to use.
* The Created vs. Completed chart represents work created and completed per interval over time.\
  \
  **Created vs. Completed Chart Best Practices:**
  * Track Bugs- Look at Stories created and completed by a certain story type. You can filter to view data just for just your Team or by Story Type, Epic, or Objective.
  * Visualize the pacing of work- See changes in the ratio of created vs completed, in particular when the divide grows further apart, comes together, or switches the balance.
  * Completed work overtime- Much like the Cumulative Flow Diagram (details below), you can also see trends on the Created vs. Completed chart on how quickly Stories are being created and completed over time.&#x20;
*   The Cumulative Flow Diagram shows work completed over time, grouped by workflow state. When used correctly, your Cumulative Flow Diagram can help you track changes as well as identify and unblock bottlenecks.

    \
    **Cumulative Flow Diagram Best Practices:**

    * A common way to read a Cumulative Flow Diagram is to look at the slopes of the "completed" chart area vs the slope of the "ready to start" area. If the "ready to start" slope is steeper than "completed" your backlog is growing.
    * The Iteration Burndown Chart is a graphical representation and projection of the remaining unfinished work in that Iteration.
    * The Epic Burndown Chart is a graphical representation of an Epic's number of Stories over time, grouped by Workflow State.

#### Saving your filtered reports <a href="#h_01hnga936p3sdvj1kh7h2gd7xv" id="h_01hnga936p3sdvj1kh7h2gd7xv"></a>

As outlined in the best practices above the use of filters is key to pulling the information you need to make an impact. Filter Ideas: Date range: Adjusting the date range allows you to save a set of reports with filter with relative dates (ie, last 30 days, 3 months, 2 quarters, etc) and the reports will always be up to date. Teams: Sort by Teams to quickly get data on how different squads are working. We recommend setting the filters as wanted per chart and then Add Bookmark (if using Chrome or similar functionality if using another browser) to each page. That way you can quickly pull up each report as needed without adjusting the filters.

#### API & Google Sheets Integration <a href="#h_01hnga936pnwjgb2pcj6zcca0t" id="h_01hnga936pnwjgb2pcj6zcca0t"></a>

If there is additional reporting your company would like to view that isn’t included in our Reports, you can user the API or Google Sheet Integration to build the metrics and dashboards that work for you. The [Shortcut API](https://shortcut.com/api/rest/v3#Introduction) provides a greater amount of control over your Workspace’s data than what is possible in the web app. The [Google Sheets integration ](https://help.shortcut.com/hc/en-us/articles/360045789091-Labs-Google-Sheets-Integration)allows for real-time updates of Shortcut data to be sent to a Google Sheet.

#### How to Build Trust Through Reporting <a href="#h_01hnga936prfq70wnma12jrzy5" id="h_01hnga936prfq70wnma12jrzy5"></a>

Healthy, high-performing software teams should consistently work towards building trust: within squads, across squads, between squads, and with their managers and stakeholders. One way to do this is through reporting and metrics. Read the blog post [How to Build Trust Through Reporting](https://shortcut.com/blog/its-valentines-day-which-means-were-going-to-talk) to learn more.&#x20;
