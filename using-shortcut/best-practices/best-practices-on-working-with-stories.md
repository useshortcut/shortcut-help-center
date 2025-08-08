# Best Practices on Working with Stories

Learn best practices on Stories including how large each Story should be, how long a Story should take, and how to use Tasks.

#### Overview <a href="#h_01hw3sjn6d6mjrp02r8b4gmt8z" id="h_01hw3sjn6d6mjrp02r8b4gmt8z"></a>

A Story represents an individual piece of work to be completed in a Workflow. Now that we know a Story’s definition, let’s break it down even more.&#x20;

#### How much work should be included in each Story? <a href="#h_01hw3sjn6d0be5fhxd7cy0d0fw" id="h_01hw3sjn6d0be5fhxd7cy0d0fw"></a>

A Story should really be an individual piece of work. For example, “Allow configuring Slack integration” should be broken down into “Build Upsert endpoint”/”Build List endpoint”/”Build Delete endpoint” as related Story cards mapping to the concept of “Allow configuring Slack integration.”

With this model it’s important to ask yourself, should this Story actually be an Epic? Epics are a core part of the organizational structure. If you find a Story is very complex, it will take work from multiple people, has a long list of tasks, or will take a week or two to complete, there are two recommendations:\
‍\
1\) We recommend converting it into an Epic. These aren’t hard rules but are a good indicator your Story is getting too big and should be broken up into an Epic with Stories. This is easy to do. When you convert a Story to an Epic the tasks will become Stories and the Story will become an Epic.

![](https://assets-global.website-files.com/6284144cb1a1fee6254fd9f3/632ae8318de4b7225b460f2e_convert%20story%20to%20epic.png)

2\) If you have a few tasks to complete a Story, we recommend breaking the Story into separate Stories and relating them to each other. When the work is too big for one Story but not quite the Epic size, create a few Stories and relate them to each. For example, you have a Front End and Back End task to complete the Story. This makes it easier to track progress and by relating them to each other it’s simple to stay organized and focused on the larger goal. You can change relationships to "blocking" or "blocked" if you want to establish a defined order of which story should be completed first.

![](https://assets-global.website-files.com/6284144cb1a1fee6254fd9f3/632ae87aafcd1a7399a7bb91_relate%20stories.png)

#### How long should a Story take to complete? <a href="#h_01hw3sjn6d2hh6c9h7k7ww502n" id="h_01hw3sjn6d2hh6c9h7k7ww502n"></a>

A story should not take more than a week to complete, but we recommend scoping your stories to 1 to 2 days. As a rule, a  Story should take a day or two to complete, but if it does need to be larger keep it no longer than a week to complete. We suggest breaking things down into smaller chunks so that progress towards deadlines are easier to track and it’s easier for Product and other team members to figure out the status of work and how things are progressing.&#x20;

#### How to think about Tasks <a href="#h_01hw3sjn6dpek3wgg5z2rxcwjh" id="h_01hw3sjn6dpek3wgg5z2rxcwjh"></a>

Tasks in Shortcut are meant to help you create a checklist of the items that need to be done in order to complete the Story, remind and assign out steps, and help outline what will go into a Story. If you have a Task that is going to take a day or more or is a few points in itself, that should likely be a Story.&#x20;

As a general rule of thumb, a task shouldn’t take more than an hour to complete.  It’s a common mistake we see to use Tasks as Stories. A nicely sized task could be something like “Deploy to production” or “Let Customer Support know the bug is fixed.” A task that’s probably too big would be something like “Update DB model” or “Create API contract”.

If you’ve got a Story that doesn’t quite feel big enough to be an Epic, but still has some large chunks of work you want to call out explicitly, convert your tasks to Stories, which will automatically create a story relationship between the two - update to a "blocking" or "blocked" relationship to show the order in which they should be completed.

![632ae97b2fb191b9e50d3519\_convert task-p-1080.png](https://help.shortcut.com/hc/article_attachments/26203354594068)

By breaking these larger “tasks” into Stories, we make their dependency ordering explicit as well as making it easy to see the progress of the work at a glance.

![632aeba186a899292b0cd732\_recommended.png](https://help.shortcut.com/hc/article_attachments/26203358222228)
