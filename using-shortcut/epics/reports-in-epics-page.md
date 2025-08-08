# Reports in Epics Page

The Velocity Bar Chart is a visual representation of Stories or Story Points completed across several iterations and also surfaces trends in how your team has performed over the last 12 weeks and highlights the average amount of Stories or Story Points over that time period.

Each [individual Epic Page](https://help.shortcut.com/hc/en-us/articles/205274149-Epics-and-The-Epics-Page) has a Velocity Bar Chart that visualizes Stories or Story Points completed across several intervals. This chart surfaces trends about how your team has performed and highlights the average and trailing average number of Stories or Story Points completed over that time period.

Using Velocity Charts can help agile teams understand patterns and set targets for future work.

![velocitychart.png](https://help.shortcut.com/hc/article_attachments/4406053945108)

The Velocity Chart is located in the Reports tab on each individual Epic page.&#x20;

For data to appear in your Epic's Velocity Bar Chart, two requirements must be met:

1. The Epic must be in an "In Progress" state
2. The Epic must contain Stories that are in a "Started" workflow state

**Using the Sum Using dropdown to aggregate data by Story Count or Story Points**\
\
The Sum Using dropdown allows users to toggle aggregation between Story Count and Story Points.

When using Story Count, the height of the bar represents total number of Stories completed in that interval.

When using Story Points, the height of the bar represents the amount of completed points associated with completed stories in that Interval. Completed Stories that have 0 points or are unestimated, do not contribute to the calculation of Story Points.

No matter which aggregation you select, you can always see the number of unestimated Stories in the top left of the chart.  The bars are color coded to represent different story types: Feature Stories (yellow), Bug Stories (red), and Chore Stories (blue).

Hovering your mouse over a single bar will produce a pop up with a quantitative breakdown of the Story types, as well as the total number of Stories or Story Points completed within the interval.&#x20;

The dotted green line shows you the overall average of velocity. This is the total number of points or stories across the entire date range, divided by the total number of intervals in the chart.

The solid green line shows you the trailing average of velocity. The number of intervals used to calculate this changes depending on the Group By filter at the top of the page:

* Day uses a 7 day trailing average, inclusive of that day
* Week uses a 4 week trailing average, inclusive of that week
* Month uses a 3 month trailing average, inclusive of that month
* Iteration uses 4 iteration trailing average, inclusive of that iteration\
  Note: The trailing average uses data outside of the selected date range to show an accurate metric at the start of the graph. For example, if the chart is Grouped By Day, the first Trailing Average calculation uses Stories completed that day, and the previous 6 days (which are not on the chart)

**Using the Group by dropdown to segment data by Day, Week, Month, or Iteration**

The Group By dropdown allows you to group data in the chart by different time frames: Day, Week, Month, or Iterations.

Some Group by options may be impacted by the date range of the entity:

* The Date Range of the entity must be at least the length of the set Group By value
* Group by Day: Only available for date ranges of 6 months or less.
* Group by Week: Only Available for date ranges of 2 years of less.
* Group by Iteration: Only available for date ranges of 2 years or less. Only Iterations that start and end within the date range are included.

Related: [Editing the Estimate Scale](https://help.shortcut.com/hc/en-us/articles/209984986)
