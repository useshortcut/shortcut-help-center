# Docs Use Case Templates

### Docs Use Case Templates

Welcome to the Docs Use Case templates! These example templates are designed to help you easily get started in Shortcut Docs. You can also see them all in our cool [demo workspace](https://app.shortcut.com/demoorg/write/all-docs) if you would prefer to view and copy them from there.

We are working on building out true templates in Shortcut, in the meantime, you can _copy and paste_ any of these into a Shortcut Doc. The formatting here looks a little off, but when pasted into a Shortcut Doc it looks much better. Click the link to the template you want to try to quickly navigate to that template.

* [Product Requirement Doc](broken-reference)
* [1:1 Meeting](broken-reference)
* [ADR (Architecture Decision Record)](broken-reference)
* [Incident Postmortem](broken-reference)
* [MVP Ideation](broken-reference)
* [OKRs](broken-reference)
* [Project Kickoff](broken-reference)
* [Sprint/Iteration Planning](broken-reference)
* [Squad Daily Standup](broken-reference)
* [Technical Design Doc](broken-reference)

***

### Product Requirement Doc  <a href="#h_01g9dqp0y2tnvvkqcexfj54g17" id="h_01g9dqp0y2tnvvkqcexfj54g17"></a>

_Use this **Product Requirements Doc (PRDs**) template to define the requirements of a particular product, including the product's purpose, features, functionality, and behavior. Use this as a guide for business and technical teams to help build, launch, or market the product._

**Overview**

### Overview

| **Target release**    | Insert Date          |
| --------------------- | -------------------- |
| **Epic**              | Type '/' to add Epic |
| **Document status**   | DRAFT                |
| **Document owner**    | @ mention owner      |
| **Designer**          | @ mention designer   |
| **Tech lead**         | @ mention lead       |
| **Technical writers** | @ mention writers    |
| **QA**                | @ mention QA         |

***

### **Objective**

_Outline the customer problem you are solving and how it relates to your vision, goals, and initiatives._

**Success metrics**

**Hypothesis**

_We believe \<this feature> will achieve \<this outcome>._

| **Goal**                             | **Metric**                                 |
| ------------------------------------ | ------------------------------------------ |
| eg., Decrease page load times by 25% | eg., Customer satisfaction score increases |
|                                      |                                            |

### **Assumptions**

_List any assumptions you have about your users, technical constraints, or business goals._

### **Product Requirements**

| **Requirement**                   | **High-Level User Story**                             | **Story**             | **Notes**                                   |
| --------------------------------- | ----------------------------------------------------- | --------------------- | ------------------------------------------- |
| e.g., Load times must remain fast | e.g., Engineers enjoy using a tool that loads quickly | Type '/' to add Story | ⁠⁠⁠⁠⁠⁠e.g., Research confirmed last quarter |

### **Designs**&#x20;

_Click + Edit Block to insert an image or paste in other design assets. For teams using Figma paste the link for a design preview._

### **Open Questions**

_Add any unanswered questions here._

| **Question**                            | **Next Steps**         | **Owner**         | **Due Date** |
| --------------------------------------- | ---------------------- | ----------------- | ------------ |
| e.g., Will the layout impact load times | e.g., Meet with design | '@ mention' owner | Insert date  |
|                                         |                        |                   |              |

### **Scope**

_Outline what is in and out of scope for the initial launch and what is planned for a later date._&#x20;

_**In Scope for \<date> launch**_

* eg., Out of Scope for \<date> launch
* eg., Edge Cases

***

### 1:1 Meeting <a href="#h_01g9dqrpe6hnnnwf86dsew3j2h" id="h_01g9dqrpe6hnnnwf86dsew3j2h"></a>

_Use this template to take notes for your **1:1 meeting** with your manager or teammates. Docs default to being shared with your workspace but you can update to private or share with individual teammates for 1:1 docs._

### \<Insert Date>

**Participants: @ mention attendees**&#x20;

#### Agenda

* Added agenda items
* Type '/' to insert related Docs, Stories, or Epics

#### Questions

* Insert questions
* Type '/' to insert related Docs, Stories, or Epics

#### Action Items

* \[@ mention item owner] insert action item
* &#x20;

***

### \<Insert Date>

**Participants: @ mention attendees**&#x20;

#### Agenda

* Added agenda items

#### Questions

* Insert questions

#### Action Items

* Insert action items

***

### ADR (Architecture Decision Record) <a href="#h_01g9dqs1p9jqgmpnc168hajth2" id="h_01g9dqs1p9jqgmpnc168hajth2"></a>

_An **Architecture Decision record (ADR)** captures an important architectural decision made along with its context and consequences._

### Status

State the status, e.g., proposed, accepted, rejected, deprecated, superseded, etc.

### Context

This is the context explaining the problem we are looking to resolve and what is motivating this decision or change (technical, goals, project)?

### Decision

Summary of the decision or outcome.

### Related decisions

List any related decisions here or include a visual such as a traceability matrix or decision tree.

### Consequences

Describe what becomes easier or more difficult because of this change.

### Proposal

Outline the details of the change that you're proposing.

### Other Notes

Because the decision-making process can take weeks, we’ve found it useful to capture notes and issues that the team discusses during the socialization process.

***

### Incident Postmortem <a href="#h_01g9dqynanew1e3t0jbp280ywn" id="h_01g9dqynanew1e3t0jbp280ywn"></a>

_The purpose of a **postmortem** is to share things we learned from the incident and help us get better. Psychological safety is critical for improvement. We keep postmortems blameless to focus on systems and processes, not human error._&#x20;

| Postmortem owner | @ mention owner                   |
| ---------------- | --------------------------------- |
| Incident         | Brief description of the incident |
| Priority         | P0/ P1 / P2                       |
| Affected Areas   |                                   |

### Bug Name: Type / to insert bug Story

Video recording: link to visual of the bug

### What happened?

Short description of what happened.

### Timeline in EST (adjust timezone as needed)

Important items to include in the timeline are:

1. How & when was it reported/discovered
2. Who was involved, and when
3. Any notable events
4. When was the incident resolved

Example:

* &#x20;3:35 AM- First report in Zendesk (link to ticket) of a user being unable to view the website
  * Ultimately 8 Zendesk tickets were connected to this issue
* 7:43 AM - (@ mention name) created bug in Shortcut (Type / to add the link to the Story)

### Users affected

Summarize how many users were affected and in what way.

### Resolution

Summarize the final resolution.

### Contributing Factors

Failure in complex systems are complex and are rarely from a root cause or a linear chain of causes. What factors contributed to the failure? People generally act in a way that seems correct to them based on the info they have ("local rationality"). Why did these actions seem correct at the time? What systems, practices, and information contributed?

### Discussion

Describe what you learned, what went well, and how you can improve.

### Action Items

Action items are "we really need to do this", not "we could do this" (put those in discussion).

Best practice recommendations for action items:

* Reify as Stories, assigned owners, and have a [severity field](https://help.shortcut.com/hc/en-us/articles/4423932934804-Fields-Overview), and due date.
* Stories are [labeled](https://help.shortcut.com/hc/en-us/articles/205702619-Shortcut-Labels-and-the-Labels-Page-) with "postmortem" so they are easily searchable

***

### MVP ideation <a href="#h_01g9dqz02eenv3pvy0xeb8xmzw" id="h_01g9dqz02eenv3pvy0xeb8xmzw"></a>

_Use the **MVP (Minimum Viable Product)** template document to outline goals, success metrics, key value props, marketing, and release plan of a feature or project._

***

### Problem to solve

Why are you building the MVP? What problem are you trying to solve?

***

### MVP Solution

Describe the solution to the problem above.

***

### Value Props and Messaging

Describe the selling propositions of the MVP.&#x20;

**Value Prop 1**

**Value Prop 2**

***

### Target Market

Name the specific users or personas that are the target market for the MVP.

***

### Competitors/Current State of the Market

What is your target market/group/users using right now for this problem? What is lacking in those solutions?

| **Competitor**          | **Problems**                                          | **Strengths**                      |
| ----------------------- | ----------------------------------------------------- | ---------------------------------- |
| Name of your competitor | e.g., Their solution doesn't integrate with key tools | e.g., UX feedback is very positive |
|                         |                                                       |                                    |

***

### Success Metrics

Outline how you will know if the MVP has been successful and solved the problem outlined.

**Primary:**

Describe primary success metrics

* \_\_\_%

**Secondary:**

Describe secondary success metrics

Adoption

* \_\_\_%&#x20;

***

### Key Steps and Timelines

| **Key Step/Epic**                                | **Timeline**                 | Owner            |
| ------------------------------------------------ | ---------------------------- | ---------------- |
| Type '/' to insert Epic or describe the key step | Add date or general timeline |  @ mention owner |
|                                                  |                              |                  |

***

### OKRs <a href="#h_01g9dqzjacghr38yn71x4vdr0m" id="h_01g9dqzjacghr38yn71x4vdr0m"></a>

_Use the **OKR** template to help your team set and track measurable goals._

| **Timeline** | Add the timeline for these OKRs |
| ------------ | ------------------------------- |
| **Docs**     | Type '/' to add other key docs  |

#### **Objective:** e.g., Create the lowest carbon footprint in our industry.

**Owner:** @ mention owner

**Epic:** Type / to add an Epic

**Key Results 1:** e.g., Pay 100% carbon offset for calculated carbon dioxide emissions.

**Key Results 2:** e.g., Supply chain and shipping infrastructure 99% zero waste.

#### **Objective:** e.g., Create the lowest carbon footprint in our industry.

**Owner:** @ mention owner

**Epic:** Type / to add an Epic

**Key Results 1:** e.g., Pay 100% carbon offset for calculated carbon dioxide emissions.

**Key Results 2:** e.g., Supply chain and shipping infrastructure 99% zero waste.

#### **Objective:** e.g., Create the lowest carbon footprint in our industry.

**Owner:** @ mention owner

**Epic:** Type / to add an Epic

**Key Results 1:** e.g., Pay 100% carbon offset for calculated carbon dioxide emissions.

**Key Results 2:** e.g., Supply chain and shipping infrastructure 99% zero waste.

***

### Project Kickoff <a href="#h_01g9dqzzatp9sxqjsdzpeb7yn5" id="h_01g9dqzzatp9sxqjsdzpeb7yn5"></a>

_Use the **Project kickoff** to ensure your team understands the project’s vision, mission, and strategy._

### Overview

| **Initiative**             | High level overview                 |
| -------------------------- | ----------------------------------- |
| **Epic**                   | Type '/' to add Epic                |
| **Date**                   | Add a date                          |
| **Resources**              | Type '/' to add other relevant Docs |
| **Project Owner**          | @ mention project owner             |
| **Design Researcher**      | @ mention Design Researcher         |
| **Product representation** | @ mention Product                   |
| **Design representation**  | @ mention Design                    |
| **Eng representation**     | @ mention Eng                       |

### Overview

### Project Goals&#x20;

### Project Deliverables

| **Deliverable** | **Date** |
| --------------- | -------- |
| e.g., Phase 1   | 6/1/2022 |
| e.g., Phase 2   | 9/1/2022 |

### Open Questions

***

### Sprint/Iteration Planning <a href="#h_01g9dr0fk0122tzwb1gs5rx2h5" id="h_01g9dr0fk0122tzwb1gs5rx2h5"></a>

_Whether your team runs Sprints (or some version of them) use this **Sprint/Iteration Planning** template to set goals, plan team capacity, and set your team up for success. For the purpose of this template, we are using Sprints and Iterations interchangeably._&#x20;

### **General Check-In**

* Staffing / organizational announcements

### **Capacity Check-In**

What's your capacity for this Sprint? (0-10 out of 10 days). Include OOO and any other capacity-reducing items.

* % total eng capacity: `n` / <# eng x 10>

| Name           | Capacity (0-10) | Notes                         |
| -------------- | --------------- | ----------------------------- |
| @ mention name | insert capacity | e.g., Out of office on Friday |
|                |                 |                               |

### **Check in on previous goals, create new iteration**

* Look at the previous sprint goals. See if you met them or not. Don’t let this discussion last too long, or feel free to address in a retro.
* [Create a new Iteration/Sprint](https://help.shortcut.com/hc/en-us/articles/360028953452-Iterations-Overview). Tip: Create a naming convention to create consistency and make finding past sprints easier.
* Talk about what the most important goals are from a Product Manager perspective. You’re not going to formalize what exactly is going to get done, but we should know after this moment what is most important.

### **Housekeeping**

* Clean up the previous Sprint
  * View all Started Iterations/Sprints by going to the Stories board page, then filter by Team & Started Iterations. This will include all previous and current issues.
* Add to Stories to the current Sprint.

### **Decide on Realistic Goals**

Working together, come up with 1-3 sentence long goals that describe what the team will accomplish.&#x20;

### **Any blockers / open questions?**

Ask the team whether there are any other concerns.

### **Name the Sprint**

Name the Sprint, have fun with it!

### **Go team! 🎉**

***

### Squad Daily Standup <a href="#h_01g9dr12qepat09pvwyz4nd658" id="h_01g9dr12qepat09pvwyz4nd658"></a>

_Use this **Squad Daily Standup** with your team to help your team uncover and coordinate interdependencies, and bring visibility to what you are working on as a team. Standups can be run synchronously during a meeting or asynchronously via a Doc._&#x20;

_**Tip:** Try filtering the board by each person, Team or Iteration or showing the_ [_Status view_](https://app.shortcut.com/internal/status?team_id=13575\&group_ids=5eeb7693-7834-43b4-a52d-a27ae8e19775\&cf_workflow=500105268) _to make sure everyone is covered._&#x20;

### **Meeting** **Format:**

Ask each person to state the high-level points of their updates. Aim to be concise in each of your updates. If the discussion needs to be more than a minute or two, ask the involved folks to regroup after standup or schedule a deeper discussion for later.

#### What did you accomplish **yesterday?**

_Provide a quick overview of the things you've done since yesterday's meeting_

* Add relevant Stories by Typing / to insert&#x20;

#### What you are planning to do **today?**

_Provide a quick overview of what's on your agenda to tackle today._

* Add relevant Stories by Typing / to insert&#x20;
* Call out non-sprint work - interviews, meetings, etc.&#x20;

#### What **risks** there are to getting this done?

1. _Call out work that needs a ticket that is **out of scope** of an active ticket to be added to draft for future refinement_
2. _Call out **dependencies** on other tickets or people needed for progress on active ticket_
3. _Call out **the need for pairing** for more team support_

***

### Technical Design Doc <a href="#h_01g9dr20bscqaat8967e4cexdd" id="h_01g9dr20bscqaat8967e4cexdd"></a>

_A T**echnical Design Document** lets an engineering team define, evaluate, and iterate on a solution when it's cheapest: before implementing it. This shares knowledge within the engineering team and can be the basis for future documentation._

***

### Problem

#### Problem Statement

What is this for? What problem are you addressing?

#### Goals

What are the goals of the feature? What outcomes will make this a success? How is the code, the system, the product, or THE WORLD 🌎 different?

* Goal 1

#### Non-Goals

What is not in scope? This helps reviewers focus on the important parts of the solution instead of pointing out areas that were deliberately not addressed.

* Not a goal of this feature

***

### Solution

#### Solution Summary

A few sentences giving a high-level summary of the solution.

#### History

Provide relevant background information to give context about why the solution makes sense. Designs are often path-dependent. This is your chance to lay out the path.

#### Solution Overview

The technical approach to solving the problem. This can include pseudocode and diagrams. This is the longest part of the design doc and requires the most research, planning, and preparation.&#x20;

***

### Considered Options

Describe the alternatives considered. (This section is optional.)

#### Pros

Outline the pros of alternatives considered.

#### Cons

Outline the cons of alternatives considered.

### Related

Links to internal process documentation of the decision, e.g. Stories, Epics, Docs, etc.

| **Link**                                                     | **Notes**                        |
| ------------------------------------------------------------ | -------------------------------- |
| Type / to insert Story or Epic or copy and paste other links | Any relevant callouts about link |
