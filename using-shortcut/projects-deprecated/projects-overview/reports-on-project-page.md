# Reports on Project Page

![Lead\_Cycle\_Gif.gif](https://help.shortcut.com/hc/article_attachments/360092449451)

Cycle and Lead Time Reports provide your team with the data you need to plan and allocate resources more effectively.

#### Chart Types <a href="#h_01hnf2xq46txtnhbzgg3zhswbm" id="h_01hnf2xq46txtnhbzgg3zhswbm"></a>

![Screen\_Recording\_2021-04-15\_at\_08.02.08.24\_AM.gif](https://help.shortcut.com/hc/article_attachments/360092504871)

**The Cycle Time Chart** can be accessed via upper right-hand corner drop-down. This chart represents how long it takes a Story to be completed after it is Started. This can provide insights such as: "_On average it takes us a X amount of days to complete certain types of Stories_" or surface outlier Stories.

**The Lead Time Chart** can be accessed via upper right-hand corner drop-down. This chart represents the amount of time that has passed between when a Story is _created_ and when it is _completed_. This can provide insights such as, "_We have a really long timespan before we pick up created Stories._"

**Custom** type can be accessed via the upper right hand corner drop down. This chart type allows you to select the Start and Date used to calculate the Cycle time in the chart. You must first select a workflow; this type does not support custom states for all workflows.&#x20;

#### Adjust States used in Calculations <a href="#h_01hnf2xq469m0dxzhgsrt6de3k" id="h_01hnf2xq469m0dxzhgsrt6de3k"></a>

Once you’ve selected the **Custom** Chart Type, you can also modify which states are included in the calculations. This is useful if you have workflows states that should (or shouldn’t) be included in calculating Lead/Cycle time. When adjusting the workflow states, they must be continuous; you cannot exclude a Workflow state in between your selected Start and End state. For example, if you have a Backlog or Icebox state that shouldn’t really count towards Lead Time, you can remove it from the calculation. Or, you may have many States in your Done workflow state category and you want to include all of the states for a Story to be considered completed.

![Screen\_Recording\_2021-04-15\_at\_08.15.28.00\_AM.gif](https://help.shortcut.com/hc/article_attachments/360092519312)

#### Chart Axes <a href="#h_01hnf2xq46b83fszdcdp6qe5d8" id="h_01hnf2xq46b83fszdcdp6qe5d8"></a>

The Y-axis of the chart represents the number of days.&#x20;

The X-axis represents the completion dates of the Stories in the selected date range, Epic, Objective, Iteration or Project in which you are viewing Cycle Time or Lead Time reports.

#### Report Stats <a href="#h_01hnf2xq46a8etrh0bsx0dektp" id="h_01hnf2xq46a8etrh0bsx0dektp"></a>

![Lead\_Cycle\_Report\_Stats.png](https://help.shortcut.com/hc/article_attachments/360092464072)

The chart provides an average Cycle Time and Lead Time as well as Minimum time. The average is also represented in the chart as the dashed line across the chart:

![Lead\_Cycle\_Average.png](https://help.shortcut.com/hc/article_attachments/360092449911)

#### Trailing Average and Story Type Filter <a href="#h_01hnf2xq4613vpzmp21xs3byb7" id="h_01hnf2xq4613vpzmp21xs3byb7"></a>

A 7-day trailing average is also included in the chart. The trailing average does not calculate the average over the last 7 consecutive days, rather the last 7 days of available data.

![Trailing\_Average.gif](https://help.shortcut.com/hc/article_attachments/360092464092)

Stories within the chart are represented by colored dots. Clicking on a dot will open the selected Story. Each Cycle Time and Lead Time chart can also be filtered by Story Type (Bug, Feature & Chore) as well as a 7 day trailing average.
