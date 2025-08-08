# Iteration Burndown Chart

### Iteration Burndown Chart

![burndown.png](https://help.shortcut.com/hc/article_attachments/21919776763924)

The Iteration Burndown Chart is a graphical representation and projection of remaining unfinished work in that Iteration. In an Iteration, the Burndown Chart is located in the Reports tab of the [Iteration Detail Page](https://help.shortcut.com/hc/en-us/articles/360029292711-The-Iteration-detail-page).

The start date and end date of the Iteration Burndown Chart correlates to the start date and end date of the Iteration. &#x20;

#### Understanding the Burndown Chart <a href="#h_01hhqphtjqg96zct9nheeyc7zb" id="h_01hhqphtjqg96zct9nheeyc7zb"></a>

The Burndown Report shows unfinished work remaining in an iteration as time progresses. This is the _Actual Remaining_ section of the chart. Remaining work decreases as work is finished or increases if work is added. Remaining work is shown alongside an _Ideal Remaining_ line which charts a constant, "idealized" burndown of work from the start of the iteration until the end.

Deviations from the expected burndown, such as a large difference in _Remaining_ versus _Ideal_, are an opportunity to drill down to find the root cause and fix it before a sprint or product release is derailed.

#### Chart Mechanics <a href="#h_01hhqppnhem71cxm5h6yne4env" id="h_01hhqppnhem71cxm5h6yne4env"></a>

**Actual Remaining**

_Actual Remaining_ is the amount of unfinished work in an iteration. This work can be in any Started or Unstarted workflow state.

The dots represent total remaining work at the **end of each day** in the iteration. Each data point demonstrates the net change in remaining work from the end of the previous day to the end of the next day.

➡️ For example, if a team completes 5 stories, but also adds 5 stories, the line will remain flat.

**Ideal Remaining**

_Ideal Remaining_ is a calculated line that progresses linearly from the starting amount of Stories or Points in the iteration down to zero on the last day.  This line is not meant to be followed precisely, but acts as a pacing barometer for an iteration. If the ideal line is way above or below remaining work, this is an indication work may be ahead or behind schedule and allows the team to take steps to correct if they desire.

The ideal line flattens across non-working days to indicate work is not expected to progress on these days. Working days can be adjusted in your [**General Settings**](http://localhost:3000/internal/settings/workspace).

_Ideal Line Starts Today_ is a toggle in the legend to show the ideal pace to finish starting from the remaining work in the iteration "today". This setting is useful for teams who add work throughout the iteration, making the first day an inaccurate starting point for the ideal line.

**Starting Point**

The initial point for both the _Actual Remaining_ and _Ideal Remaining_ lines is finalized at the **end of the first day** of an iteration. This means your team can add stories throughout the first day, or during an iteration planning meeting, and these will count towards the starting point of the ideal line.&#x20;

**Tooltips**

Tooltips show counts of work _Added_, _Completed_ or _Removed_ each day. This breakdown helps understand the net change for a day. For example, the line might be flat because work was both completed and added.

The "Today" tooltip also shows the status of all remaining work to give a clearer picture of actual progress.

**Stories vs. Points**

The chart defaults to Stories (total count) or Points, depending on your [**Estimate Scale**](http://localhost:3000/internal/settings/estimates) settings. There is a toggle to quickly switch between the two on the report.

**Non-Working Days**

Non-working days are noted on the chart with hatched bars. The ideal line flattens across non-working days to indicate work is not expected to progress on these days. Working days for your Workspace can be adjusted in your [**General Settings**](http://localhost:3000/internal/settings/workspace).

**Note**

An Iteration's Burndown Chart will "freeze" once its end date has passed. If you are viewing your Iteration Burndown chart in Points, the Burndown Chart will reflect the current Points of the corresponding Stories, **up to the last day of the Iteration**. That is, if the Points Estimate of a Story in an Iteration changes _after_ the Iteration has ended, it will not be reflected in the Burndown Chart. Similarly, if you are viewing your Iteration Burndown chart in Story Counts, the number of Stories added to or removed from the Iteration _after_ the Iteration has ended, will not be reflected in the Iteration's Burndown Chart.&#x20;
