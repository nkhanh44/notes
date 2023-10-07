**Agile Project Management**

[**Stories**](https://www.atlassian.com/agile/project-management/user-stories), also called "user stories," are short requirements or requests written from the perspective of an end user.

[**Epics**](https://www.atlassian.com/agile/project-management/epics) are large bodies of work that can be broken down into a number of smaller tasks (called stories).

-   **Initiatives** are collections of epics that drive toward a common goal.

![Screen Shot 2021-08-04 at 4 20 27 PM](https://github.com/nkhanh44/notes/assets/25881847/48e829d0-977a-46f0-a326-f06f0fb4a6ad)

**Agile epic vs. initiative**

![epics-vs-stories-agile-development](https://github.com/nkhanh44/notes/assets/25881847/a1a75753-a878-4bcd-8f47-a7a0f0da67cf)

**Measuring agile epics**

Burndown charts

-   **Purpose of Burndown Charts**: Burndown charts are used in Agile project management to visualize the progress of epics, keeping teams motivated and informing executive stakeholders.
-   **Components of an Epic Burndown Chart**: An epic burndown chart displays both the actual and estimated work to be done within a sprint or epic. It uses a horizontal x-axis for time and a vertical y-axis for stories or issues.
-   **Tracking Work Progress**: Burndown charts are essential for tracking the remaining work in a sprint or epic and projecting the likelihood of achieving the sprint goal. This tracking helps teams manage their progress and make necessary adjustments.
-   **Identifying Blockers**: Monitoring the burndown chart provides insights into how the team is progressing and highlights any obstacles or blockers that need attention.

**User Stories**

-   **Stories keep the focus on the user.** A to-do list keeps the team focused on tasks that need to be checked off, but a collection of stories keeps the team focused on solving problems for real users.

-   **Stories enable collaboration.** With the end goal defined, the team can work together to decide how best to serve the user and meet that goal.

-   **Stories drive creative solutions.** Stories encourage the team to think critically and creatively about how to best solve for an end goal.

-   **Stories create momentum.** With each passing story, the development team enjoys a small challenge and a small win, driving momentum.

**User story template and examples**

**"As a [persona], I [want to], [so that]."**

-   "As a [persona]": Who are we building this for? We're not just after a job title, we're after the persona of the person. Max. Our team should have a shared understanding of who Max is. We've hopefully interviewed plenty of Max's. We understand how that person works, how they think and what they feel. We have empathy for Max.
-   "Wants to": Here we're describing their intent --- not the features they use. What is it they're actually trying to achieve? This statement should be implementation free --- if you're describing any part of the UI and not what the user goal is you're missing the point.
-   "So that": how does their immediate desire to do something this fit into their bigger picture? What's the overall benefit they're trying to achieve? What is the big problem that needs solving?

**Metrics**

**Velocity**

Velocity is the average amount of work a scrum team completes during a sprint, measured in either story points or hours, and is very useful for forecasting

![Screenshot 2023-10-03 at 22 21 56](https://github.com/nkhanh44/notes/assets/25881847/b7eaaee1-477b-4002-a59f-fc24957808ad)

*ANTI-PATTERNS TO WATCH FOR*

When velocity is erratic over a long period of time, always revisit the team's estimation practices. During the team's retrospective, ask the following questions:

-   Are there unforeseen development challenges we didn't account for when estimating this work? How can we better break down work to uncover some of these challenges?
-   Is there outside business pressure pushing the team beyond its limits? Is adherance to development best practices suffering as a result?
-   As a team, are we overzealous in forecasting for the sprint?

**Control chart**

Control charts focus on the cycle time of individual issues--the total time from "in progress" to "done". Teams with shorter cycle times are likely to have higher throughput.

Measuring cycle time is an efficient and flexible way to improve a team's processes because the results of changes are discernable almost immediately, allowing them to make any further adjustments right away. The end goal is to have a consistent and short cycle time, regardless of the type of work (new feature, [technical debt](https://www.atlassian.com/agile/software-development/technical-debt), etc.).

*ANTI-PATTERNS TO WATCH FOR*

**Control charts can appear fickle at first. Don't be so concerned with every outlier. Look for trends. Here are two areas to watch out for:**

-   Increasing cycle time - Increasing cycle time saps the team of its hard-earned agility. In the team retrospective, take time to understand an increase. One exception: if the team's definition of done has expanded, cycle time will probably expand too.
-   Erratic cycle time -- The goal is to have consistent cycle time for work items that have similar story point values. Filter the control chart for each story point value to check for consistency. If cycle time is erratic on small and large story point values, spend time in the retrospective examining the misses and improving future estimation.

![Screenshot 2023-10-03 at 22 22 22](https://github.com/nkhanh44/notes/assets/25881847/5e303a8a-99b3-4224-ae73-a39eabaacb38)

**Cumulative flow diagram**

The cumulative flow diagram should look smooth(ish) from left to right. Bubbles or gaps in any one color indicate shortages and bottlenecks, so when you see one, look for ways to smooth out color bands across the chart.

![Screenshot 2023-10-03 at 22 23 34](https://github.com/nkhanh44/notes/assets/25881847/9b6445a8-b08e-477c-a974-10dc59677be0)

*ANTI-PATTERNS TO WATCH FOR*

-   Blocking issues create large backups in some parts of the process and starvation in others.
-   Unchecked backlog growth over time. This results from product owners not closing issues that are obsolete or simply too low in priority to ever be pulled in.

**Three Pillars of Scrum: Understanding Scrum's Core Principles**

**Transparency**: This principle emphasizes open and clear communication among project stakeholders. It involves various aspects of Scrum, such as maintaining a sprint backlog, a product backlog, sprint reviews, and clear task definitions. Transparency is vital for building trust and collaboration.

**Inspection**: Regularly evaluating project progress and the product itself is the core of the inspection principle. It occurs during sprint planning, daily stand-up meetings, sprint reviews, and retrospectives. Inspection drives continuous improvement by identifying deviations and issues early in the project.

**Adaptation**: Adaptation complements inspection by enabling teams to make adjustments based on insights gained from inspection. Teams can adapt their sprint backlog, daily plans, and strategies in response to changing requirements or emerging challenges. Adaptation leads to flexibility, enhanced quality, and optimized processes.

**Understanding Definition of Ready**

DoR means you can take immediate action. Before starting a project, your team needs to know:

-   **Your target customers**: What are their motivations, pain points, and needs?
-   **The project goals**: What's the purpose of the project? 
-   **The required tasks**: Are they valuable, both for the business and the user? Are they clear and feasible? 
-   **Technical requirements**: Do they have the necessary resources? Do they understand the technical approach or solution? Can you test it?
-   **Time estimates**: What's the timeline to complete the work? Have stakeholders and the team agreed on an end date?
-   **The definition of done (DoD)**: What does completion, or DoD, look like? What [Scrum metrics](https://www.atlassian.com/agile/scrum/scrum-metrics) do you plan to use to evaluate success?

**Kanban**

-   **Visual Boards**: Kanban uses visual boards, like a to-do list with sticky notes. Each sticky note represents a task. You move these notes across the board as you work on them.
-   **Work Limits**: You can't have too many notes in progress at once. Imagine you have a limit of three sticky notes in the "Doing" column. That means you can only work on three tasks at a time. This helps you focus.
-   **Pull, Don't Push**: Instead of someone telling you what to do, you decide what to work on next when you're ready. It's like going to the fridge when you're hungry instead of having meals served at set times.
-   **Continuous Flow**: Kanban wants work to move smoothly, like a river. No big rushes or bottlenecks. It's all about getting tasks done steadily.

![Elements_of_a_kanban_board](https://github.com/nkhanh44/notes/assets/25881847/b3338167-04fa-451e-9eee-8bfa0d3c50a6)

Digital boards

![image4](https://github.com/nkhanh44/notes/assets/25881847/32b6a14f-7a1e-458a-a7cf-6e87dcc25176)

![Screenshot 2023-10-07 at 19 41 30](https://github.com/nkhanh44/notes/assets/25881847/598f2a5d-8e72-4fd8-9c4e-d4b9d04ab0e2)

**1\. Framework vs. Method:**

-   **Scrum**: Scrum is a well-defined framework with specific roles, events (like sprints, daily stand-ups, and retrospectives), and artifacts (like the product backlog and sprint backlog). It provides a structured approach to project management.
-   **Kanban**: Kanban is a method or system rather than a framework. It offers guiding principles and practices but is more flexible and adaptable. Kanban doesn't prescribe specific roles or events; it allows teams to design their own workflow.

**2\. Work Management:**

-   **Scrum**: Scrum divides work into time-bound iterations called sprints, typically lasting 2-4 weeks. During each sprint, a set of user stories or backlog items is selected for completion. The work is tightly controlled within the sprint duration.
-   **Kanban**: Kanban focuses on continuous flow. Work items are managed on a Kanban board, and there are no fixed timeboxes like sprints. Teams pull work as capacity allows, and there is no inherent time pressure to complete specific items within a set timeframe.

**3\. Planning and Flexibility:**

-   **Scrum**: Scrum involves detailed sprint planning and commitment to a set of tasks for the sprint. Changes to the sprint scope are discouraged during the sprint to maintain stability.
-   **Kanban**: Kanban allows for more flexibility. Work items can be reprioritized or added/removed from the backlog at any time, without needing to wait for a sprint boundary. This flexibility makes it suitable for environments with rapidly changing priorities.

**4\. Roles:**

-   **Scrum**: Scrum defines specific roles, including Scrum Master, Product Owner, and Development Team. Each role has distinct responsibilities.
-   **Kanban**: Kanban doesn't prescribe specific roles. While teams may have roles like a facilitator or product owner, the roles are not as strictly defined as in Scrum.

**5\. WIP Limits:**

-   **Scrum**: Scrum doesn't have explicit Work in Progress (WIP) limits. Teams are expected to commit to a set of tasks at the beginning of the sprint but can't exceed that commitment.
-   **Kanban**: WIP limits are a fundamental aspect of Kanban. They restrict the number of items allowed in each column of the Kanban board, ensuring that teams don't take on too much work simultaneously.

**6\. Metrics:**

-   **Scrum**: Scrum typically focuses on metrics like velocity (amount of work completed in a sprint) and burndown charts (tracking work remaining in a sprint).
-   **Kanban**: Kanban emphasizes metrics like cycle time (time to complete a single task), lead time (time from request to completion), and cumulative flow diagrams (showing the flow of work items through stages).

**Agile at scale**

![Screenshot 2023-10-07 at 17 38 55](https://github.com/nkhanh44/notes/assets/25881847/9bdd3156-77db-4599-a00c-9c50d14174bb)

The objectives of Lean Portfolio Management are to:

-   **Maximize the throughput of value** - Actively manage the backlog of investments to find the highest-value opportunities, and actively manage WIP across groups of teams(team-of-teams) to speed the delivery of value into the marketplace
-   **Prevent bottlenecks** - Use the portfolio budget to balance the funding for capacity with the demand for the highest-value opportunities
-   **Demonstrate good servant leadership** - Remove obstacles to keep delivery cycle times low

The Spotify model is an approach used by organizations to scale agile practices. It emphasizes culture and networking as key drivers of innovation and productivity. Unlike traditional frameworks, it doesn't prescribe specific practices but focuses on how an organization should be structured for agility.

Here are the main components of the Spotify model:

-   Squads: These are autonomous teams of 6-12 individuals who work on a specific feature area. Each Squad has a unique mission, an agile coach for support, and a product owner for guidance. Squads can choose their agile methodology/framework.
-   Tribes: When multiple Squads work together on the same feature area, they form a Tribe. Tribes help maintain alignment and typically consist of 40-150 people. Each Tribe has a Tribe Lead to coordinate across Squads.
-   Chapters: Chapters are groups of specialists (e.g., Javascript Developers, DBAs) who ensure alignment on best practices within their discipline. A senior technology lead often leads a Chapter.
-   Guilds: Guilds are communities of interest where team members passionate about a topic come together. They can cross different Tribes and are entirely voluntary. There is no formal leader; a Guild Coordinator helps facilitate collaboration.
-   Trio: A Trio consists of a Tribe Lead, a product lead, and a design lead. Each Tribe has a Trio to ensure continuous alignment between these perspectives when working on feature areas.
-   Alliance: When multiple Tribes need to collaborate on a significant goal, they form Alliances, which consist of multiple Tribe Trios.

![Screenshot 2023-10-07 at 17 46 31](https://github.com/nkhanh44/notes/assets/25881847/11d0e830-fca3-4ab9-b524-1823e52d74c8)

=>
Benefits of the Spotify model:

-   The Spotify model emphasizes flexibility over formal processes and ceremonies, allowing teams (Squads) to work in ways that suit their goals while aligning with each other.
-   It promotes self-management and autonomy, giving Squads the freedom to make decisions about their work and direction. This decentralized approach fosters engagement and innovation.
-   Increased transparency and experimentation in a high-trust environment can lead to better products, happier customers, and more engaged employees.

Challenges of the Spotify model:

-   While many organizations desire the benefits of the Spotify model, emulating it can be challenging due to differences in organizational culture and structure.
-   The model may look simple on the surface, but it relies on key cultural elements like trust and autonomy, which require a shift in behaviors and culture. Simply renaming teams as Squads without addressing these cultural aspects won't lead to the same benefits.

![Screenshot 2023-10-07 at 17 59 17](https://github.com/nkhanh44/notes/assets/25881847/035a7d72-8d1d-4092-95a2-e0f2d9c2b491)

**LeSS versus scrum**

Key points about LeSS (Large Scale Scrum):

1.  Extension, Not Competition: LeSS doesn't compete with traditional Scrum; instead, it extends Scrum principles for effective use in larger organizations.

2.  Basic LeSS Resembles Single Team: In Basic LeSS, it's similar to a single Scrum team with one product backlog, product owner, and definition of done.

3.  Collaborative Teams: Multiple teams in LeSS collaborate as if they were one Scrum team to deliver a common product at the end of each sprint.

4.  Role Expansion in LeSS Huge: In LeSS Huge, the product owner role expands to include area product owners who coordinate across multiple teams.

5.  Two-Part Sprint Planning: Sprint planning in LeSS involves two parts: dividing product backlog items collectively and individual teams planning sprints while coordinating with each other.

6.  Adapted Scrum Ceremonies: Scrum ceremonies like the daily scrum, sprint review, and retrospective have specific adaptations in LeSS.

7.  Scaling Effectively: The primary goal of LeSS is to scale Scrum effectively in larger organizational contexts, rather than competing with traditional Scrum.

**Anti-Patterns**

- What are Scrum Anti-Patterns?

- Any common reinvented but bad solution to a problem.

**Anti-Pattern: Velocity as a Target**

- "Velocity of 25 means we'll never get done"

- "Increased Velocity means quicker delivery"

- "If we increase Velocity by 3, we'll get that feature delivered next Sprint"

**Anti-Pattern: Team Formation**

- "How do we deal with third parties?"

- "It takes longer than a Sprint for the testers to complete testing"

- "We can't get 'Done' because we don't have a <rare skill role>"

**Anti-Patterns and the Sprint Retrospective**

<img width="1036" alt="Screenshot 2023-10-07 at 18 29 06" src="https://github.com/nkhanh44/notes/assets/25881847/f297dea4-4782-4f58-83f9-641f7d2e623b">

**Anti-Pattern: The Hero Developer**

- Heroes not required

- Heroes almost always ignore quality

- Hero culture = broken culture

- Heroes crave attention

**Anti-Pattern: Absent Product Owner**

- Very common and very destructive

- Increase wait time and create waste

- Feature decisions are often decided by those least appropriate to do so

**Working Scrum Master Advice:**

Don't just identify anti-patterns, fix them.

-   Assume nothing
-   Ask questions
-   Highlight the truth where you find it
