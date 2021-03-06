# Methodologies
This document aims to provide a lightweight reference about software development methodologies and processes, making emphasis on agile software development.

## Traditional

### RUP

RUP is not a single concrete prescriptive process, but rather an adaptable process framework, intended to be tailored by the development organizations and software project teams that will select the elements of the process that are appropriate for their needs. RUP is a specific implementation of the unified process.

#### Concepts

#### Building blocks
RUP is based on a set building blocks and content elements, describing what is to be produced, the necessary skills required and the step-by-step explanation describing how specific development goals are to be achieved. The main building blocks, or content elements, are the following:

- Roles (who) – A role defines a set of related skills, competencies and responsibilities.
- Work products (what) – A work product represents something resulting from a task, including all the documents and models produced while working through the process.
- Tasks (how) – A task describes a unit of work assigned to a Role that provides a meaningful result.

#### Life cycle phases
The RUP has determined a project life-cycle consisting of four phases. These phases allow the process to be presented at a high level in a similar way to how a 'waterfall'-styled project might be presented, although in essence the key to the process lies in the iterations of development that lie within all of the phases

##### Inception
The primary objective is to scope the system adequately as a basis for validating initial costing and budgets. In this phase the business case which includes business context, success factors (expected revenue, market recognition, etc.), and financial forecast is established.

##### Elaboration
The primary objective is to mitigate the key risk items identified by analysis up to the end of this phase. The elaboration phase is where the project starts to take shape. In this phase the problem domain analysis is made and the architecture of the project gets its basic form.

##### Construction
The primary objective is to build the software system. In this phase, the main focus is on the development of components and other features of the system. This is the phase when the bulk of the coding takes place. In larger projects, several construction iterations may be developed in an effort to divide the use cases into manageable segments that produce demonstrable prototypes.
This phase produces the first external release of the software. Its conclusion is marked by the initial operational capability milestone.

##### Transition
The primary objective is to 'transit' the system from development into production, making it available to and understood by the end user. The activities of this phase include training the end users and maintainers and beta testing the system to validate it against the end users' expectations. The product is also checked against the quality level set in the Inception phase.
If all objectives are met, the product release milestone is reached and the development cycle is finished.
## Agile

Agile methodologies are an alternative to traditional project management, typically used in software development. They help teams respond to unpredictability through incremental iterative work cadences, known as sprints particulary in Scrum, or helping to manage the work flow, as Kanban does.
Agile methodologies are an alternative to waterfall, or traditional sequential development.

### Scrum
Scrum is a management framework for incremental product development using one or more cross-functional, self-organizing teams of about seven people each.
It provides a structure of roles, meetings, rules, and artifacts. Teams are responsible for creating and adapting their processes within this framework.
Scrum uses fixed-length iterations, called Sprints, which are typically 1-2 weeks long (never more than 30 days).
Scrum teams attempt to build a potentially shippable (properly tested) product increment every iteration.

#### Concepts

#### Roles
There are three core roles in the scrum framework. These core roles are those committed to the project in the scrum process; they are the ones producing the product (objective of the project). They represent the scrum team. Although other roles may be encountered in real projects, scrum does not define any team roles other than those described below.

##### Product owner
The product owner represents the stakeholders and is the voice of the customer, who is accountable for ensuring that the team delivers value to the business. The product owner writes (or has the team write) customer-centric items (typically user stories), ranks and prioritizes them, and adds them to the product backlog. Scrum teams should have one product owner, this role should not be combined with that of the scrum master. The product owner should be on the business side of the project, and should never interfere or interact with team members on the technical aspects of the development task.

##### Scrum master
Scrum is facilitated by a scrum master, who is accountable for removing impediments to the ability of the team to deliver the product goals and deliverables. The scrum master is not a traditional team lead or project manager, but acts as a buffer between the team and any distracting influences. The scrum master ensures that the scrum process is used as intended. The scrum master helps ensure the team follows the agreed scrum processes, often facilitates key sessions, and encourages the team to improve. The role has also been referred to as a team facilitator or servant-leader to reinforce these dual perspectives.

##### Development team
The development team is responsible for delivering potentially shippable increments (PSIs) of product at the end of each sprint (the sprint goal). A team is made up of 3–9 individuals who do the actual work (analyse, design, develop, test, technical communication, document, etc.). Development teams are cross-functional, with all of the skills as a team necessary to create a product increment. The development team in scrum is self-organizing, even though there may be some level of interface with project management offices (PMOs).

#### Workflow
A sprint (or iteration) is the basic unit of development in scrum. The sprint is a timeboxed effort; that is, it is restricted to a specific duration. The duration is fixed in advance for each sprint and is normally between one week and one month, with two weeks being the most common.
Each sprint starts with a sprint planning event that aims to define a sprint backlog, identify the work for the sprint, and make an estimated commitment for the sprint goal. Each sprint ends with a sprint review and sprint retrospective, that reviews progress to show to stakeholders and identify lessons and improvements for the next sprints.
Scrum emphasizes working product at the end of the sprint that is really done. In the case of software, this likely includes that the software has been integrated, fully tested, end-user documented, and is potentially shippable.

##### Sprint Planning
During the sprint planning meeting, the product owner describes the highest priority features to the team. The team asks enough questions that they can turn a high-level user story of the product backlog into the more detailed tasks of the sprint backlog.

The product owner doesn't have to describe every item being tracked on the product backlog. A good guideline is for the product owner to come to the sprint planning meeting prepared to talk about two sprint's worth of product backlog items. To make an example really simple, suppose a team always finishes five product backlog items. Their product owner should enter the meeting prepared to talk about the top 10 priorities.

###### Whats the outcome of the Sprint Planning?
There are two defined artifacts that result from a sprint planning meeting:

- The sprint goal
  - The sprint goal can be used for quick reporting to those outside the sprint. There are always stakeholders who want to know what the team is working on, but who do not need to hear about each product backlog item (user story) in detail.
- The sprint backlog
  - The sprint backlog is the other output of sprint planning. A sprint backlog is a list of the product backlog items the team commits to delivering plus the list of tasks necessary to delivering those product backlog items. Each task on the sprint backlog is also usually estimated.

###### Who attends to the Sprint Planning?
- Product owner
- Scrum master
- Development team

##### Daily scrum
The Daily Scrum is a 15-minute time-boxed event for the Development Team to synchronize activities and create a plan for the next 24 hours. This is done by inspecting the work since the last Daily Scrum and forecasting the work that could be done before the next one. The Daily Scrum is held at the same time and place each day to reduce complexity. During the meeting, the Development Team members explain:
- What did I do yesterday that helped the Development Team meet the Sprint Goal?
- What will I do today to help the Development Team meet the Sprint Goal?
- Do I see any impediment that prevents me or the Development Team from meeting the Sprint Goal?

###### What's the outcome of the Daily Scrum?
- An updated scrum board to improve visibility of the progress.
- A list of blockers or impediments that need to be dealed with by the Scrum Master.

###### Who attends to the Daily Scrum?
- Scrum master
- Development team

##### Sprint review
A Sprint Review is held at the end of the Sprint to inspect the Increment and adapt the Product Backlog if needed. During the Sprint Review, the Scrum Team and stakeholders collaborate about what was done in the Sprint. Based on that and any changes to the Product Backlog during the Sprint, attendees collaborate on the next things that could be done to optimize value. This is an informal meeting, not a status meeting, and the presentation of the product increment is intended to elicit feedback and foster collaboration.

###### What's the outcome of the Sprint Review?
- A progress status report
- An update from the product vision and feedback given by the Product Owner and stakeholders

###### Who attends to the Sprint Review?
- All the Scrum Team including the Product Owner
- Stakeholders may attend as well

##### Sprint Retrospective
The Sprint Retrospective is an opportunity for the Scrum Team to inspect itself and create a plan for improvements to be enacted during the next Sprint. The Sprint Retrospective occurs after the Sprint Review and prior to the next Sprint Planning.

This is a three-hour time-boxed meeting for one-month sprints. For shorter sprints, the event is usually shorter. The Scrum Master ensures that the event takes place and that attendants understand its purpose. The Scrum Master teaches all to keep it within the time-box. The Scrum Master participates as a peer team member in the meeting from the accountability over the
Scrum process.

###### What's the outcome of the Sprint Retrospective?
- A detailed plan to continuosly improve the work process
- A status report of completed action items in the continous improvement plan since last Restrospective

###### Who attends to the Sprint Review?
- The Scrum Master
- The Development Team

#### Metrics

##### Sprint burndown

Scrum teams organize development into time-boxed sprints. At the outset of the sprint, the team forecasts how much work they can complete during a sprint. A sprint burndown report then tracks the completion of work throughout the sprint. The x-axis represents time, and the y-axis refers to the amount of work left to complete, measured in either story points or hours. The goal is to have all the forecasted work completed by the end of the sprint.

A team that consistently meets its forecast is a compelling advertisement for agile in their organization. But don't let that tempt you to fudge the numbers by declairing an item complete before it really is. It may look good in the short term, but in the long run only hampers learning and improvement.

![Burndown chart](https://raw.githubusercontent.com/ricardocasares/grow/methodologies/assets/methodologies/burndown_chart.png "Burndown chart")

###### Anti-patterns to watch for

- The team finishes early sprint after sprint because they aren't committing to enough work. 
- The team misses their forecast sprint after sprint becase they're committing to too much work. 
- The burndown line makes steep drops rather than a more gradual burndown because the work hasn't been broken down into granular pieces.
- The product owner adds or changes the scope mid-sprint.

##### Velocity

Velocity is the average amount of work a scrum team completes during a sprint, measured in either story points or hours, and is very useful for forecasting. The product owner can use velocity to predict how quickly a team can work through the backlog, because the report tracks the forecasted and completed work over several iterations–the more iterations, the more accurate the forecast.

Let's say the product owner wants to complete 500 story points in the backlog. We know that the development team generally completes 50 story points per iteration. The product owner can reasonably assume the team will need 10 iterations (give or take) to complete the required work.

It's important to monitor how velocity evolves over time. New teams can expect to see an increase in velocity as the team optimizes relationships and the work process. Existing teams can track their velocity to ensure consistent performance over time, and can confirm that a particular process change made improvements or not. A decrease in average velocity is usually a sign that some part of the team's development process has become inefficient and should be brought up at the next retrospective.

![Velocity report](https://raw.githubusercontent.com/ricardocasares/grow/methodologies/assets/methodologies/velocity_report.png "Velocity report")

###### Anti-patterns to watch for

When velocity is erratic over a long period of time, always revisit the team's estimation practices. During the team's retrospective, ask the following questions:

- Are there unforeseen development challenges we didn't account for when estimating this work? How can we better break down work to uncover some of these challenges?
- Is there outside business pressure pushing the team beyond its limits? Is adherance to development best practices suffering as a result?
- As a team, are we overzealous in forecasting for the sprint? 


#### Summary
Scrum’s roles, artifacts, events, and rules are immutable and although implementing only parts of Scrum is possible, the result is not Scrum. Scrum exists only in its entirety and functions well as a container for other techniques, methodologies, and practices.

Scrum does a strong emphasis on cross-functional teams, time-boxed and to-the-point meetings. Team motivation, trust and transparency are key aspects of it.


### Kanban

Unlike other methods that force fit change from the get-go, Kanban is about evolution, not revolution. It hinges on the fundamental truth that you can’t get where you want to go without first knowing where you are.
Kanban is similar to Scrum, in that it helps teams release software early and often. However, Kanban gives more flexibility in terms of planning and execution. Instead of working in time-based sprints, work is continuously delivered in Kanban, and your team pulls single pieces of work from the backlog, and then moves them to done.

#### Concepts

##### Visualize the workflow
In short, you should be able to, at any time, look at your overall workflow, be able to determine quickly what you should work on next, have visual cues for priority and time to complete, and that system should be easy to add, remove, and re-organize. The main form of visualization is the Kanban board.

##### Limit the work-in-progress
In Kanban systems the work-in-progress (WIP) at each state in the workflow is limited and new work is "pulled" into when there is available capacity within the local WIP limit.

##### Manage the flow
The flow of work items through each state in the workflow should be monitored and reported - often referred to as Measuring Flow. By flow we mean movement. We are interested in the speed of movement and the smoothness of that movement. Ideally we want fast smooth flow. Fast smooth flow means our system is both creating value quickly, which is minimizing risk and avoiding (opportunity) cost of delay, and is also doing so in a predictable fashion.

##### Make the work explicit
Until the mechanism of software development or IT operations process is made explicit it is often hard or impossible to hold a discussion about improving it. Without an explicit understanding of how things work and how work is actually done, any discussion of problems tends to be emotional, anecdotal and subjective. With an explicit understanding it is possible to move to a more rational, empirical, objective discussion of issues. This is more likely to facilitate consensus around improvement suggestions.

##### Implement feedback loops
An evolutionary process cannot work without feedback loops. The purpose of feedback loops is to be able to compare expected outcomes with actual outcomes and make adjustments. Specifically, we want to make process and policy adjustments as a result of the feedback and understanding the current outcomes in comparison with our expectations or desires.

##### Improve and evolve
It is the WIP limit that ultimately stimulates conversations about process problems. Things which impede flow, or introduce perturbations that mean flow is inconsistent or ragged, often result in a challenge to the WIP limit. The team has the option to break the limit, ignore the problem and carry on, or to face up to the issue, discuss it and suggest a change.

When teams have a shared understanding of theories about work, workflow, process, and risk, they are more likely to be able to build a shared comprehension of a problem and suggest improvement actions which can be agreed by consensus


#### Metrics

##### Lead time
Lead time is the time taken from when an issue is logged until work is completed on that issue.

##### Cycle time
Cycle time is the time spent working on an issue — typically, the time taken from when work begins on an issue to when work is completed, but also includes any other time spent working on the issue. For example, if an issue is reopened, worked on, and completed again, then the time for this extra work is added to the cycle time.

##### Throughput
In Kanban throughput is mainly used for tracking team's performance. Logically, the objective is to continuously improve it. Throughput is the number of work items that the team is capable to deliver in a given time period, e.g. week, month, provided that they keep a bearable work load.

---

##### Sources
- [Rational unified process](https://es.wikipedia.org/wiki/Proceso_Unificado_de_Rational)
- [Scrum reference cards](http://scrumreferencecard.com/scrum-reference-card/)
- [The Scrum guide](http://www.scrumguides.org/docs/scrumguide/v1/scrum-guide-us.pdf)
- [Scrum (Software development)](https://en.wikipedia.org/wiki/Scrum_(software_development))
- [Scrum Practitioners Open Questions](https://www.scrum.org/Forums/aft/1292/afpg/2)
