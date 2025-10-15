**THIS IS AN EXAMPLE. DO NOT REUSE VERBATIM. TAILOR CONTENT & MESSAGING APPROPRIATLEY TO AUDIENCE** 

![alt text](image location "Stella logo")

# Agile Process

## Table of Contents
- [Overview](#overview)
  * [Agile Ceremonies](#agile-ceremonies)
  * [Agile Tooling](#agile-tooling)

# Overview
<p align="left">
<img src="https://playbook.cio.gov/assets/images/usds-logo-seal.png" align="middle"  title="USDS logo" width=50 height =50>
 <strong>Applying <a href="https://playbook.cio.gov/#play4">Play 4</a></strong>
</p>

We use our scalable Agile process to deploy cross functional teams aligned to products and project requirements. Our process includes a strong emphasis on how we achieve the Product Owner and end user engagement required to deliver solutions that are readily adopted with a mission impact. Our teams use Scrum for software development or project-based work, and Kanban for operations and ongoing monitoring. We use our Agile approach to deliver the transparency, predictability, and flexibility that our customers need to observe progress, track metrics, and deliver value to their customers.

Team Stella’s Agile teams kickoff our **Appreciate Phase** by conducting our Discovery activity to understand the requirements, detailed product needs and what constitutes value for the Product Owner, stakeholders and users. We work with the Product Owner, stakeholders, users, and other product teams that might integrate with our teams to understand the requirements and ensure they are represented in the user stories using our UCD methods.

The Scrum Master, Lead Designer, and Technical Lead for each team works closely with the Government Product Owner to evaluate user stories, technical tasks, prioritization, acceptance criteria, and all things related to the backlog. Backlog grooming ensures all user stories are well-defined, decomposed to a level the team can accomplish within a sprint, and prioritized appropriately. Our team works collaboratively with the Product Owner to validate, prioritize, refine, and tighten the product, release, and sprint backlogs.

Following Discovery, the team conducts a Sprint Zero activity where they use their development workstations, development tools, code and binary repositories, frameworks, libraries, and development assets to push initial test code to source control and perform a build using the CI/CD pipeline. This establishes the baseline to start developing against user stories using a DevSecOps-focused approach. During Sprint Zero, we are not only establishing a code baseline, we are also  establishing and refining our CI/CD pipeline to ensure the technology is in place to enable our teams’ capabilities around build management, comprehensive automated testing, static code analysis, and containerization and deployment services. Once we push code and show initial user story success, we move into Sprint One and the **Innovate Phase**.

With the team assembled, the product planning is kicked off, the CI/CD pipeline and process tested, the Agile backlog prioritized and designers able to work with the team and users/stakeholders - the team is ready to begin sprinting in earnest. At this stage, our teams begin conducting our Agile ceremonies – release and sprint planning, planning poker, user story estimation, technical task development, defining acceptance criteria and definition of done for each story, daily scrums, sprint reviews, sprint demonstrations, and sprint retrospectives on a once-a-sprint basis - alongside our Product Owner and stakeholders.

As the teams begin sprinting, they enter the **Iterate Phase**. The team is developing software, configuring infrastructure and platforms through infrastructure as code, developing test plans, conducting comprehensive testing using automation techniques, coding automated acceptance testing for user stories that include acceptance criteria, and delivering regular sprint demonstrations to the team and stakeholders. In the **Activate Phase**, our teams conduct sprint demonstrations and sprint reviews at the end of each sprint to brief Product Owners, stakeholders, and users on the work completed during the sprint. Team Steampunk focuses on validating that each user story completed satisfies the definition of done, documented acceptance criteria, and meets the business value requirements identified in the story.

<p align="center">
 <img src="Agile Process image location " title="Agile Process">
</p>

## Agile Ceremonies

Agile Ceremony | Recurrence	| Goals & Benefits
----- | ----- | ------
Discovery | Sprint Zero	Once at beginning of new product/project cycle | Establish initial product backlog and technical ability for team to conduct development activities. Issue GFE, access to systems, Rally, repos, pipeline, initial build script established, initial code committed, built, tested, deployed to test environment. Understand requirements and establish strong rapport with stakeholder/user community. Establish definition of done.
PI Planning | Every three months, at the beginning of the program increment	| Assess, evaluate, understand, document, estimate, prioritize epics, features, and functions planned for development and deployment over the coming program increment. Program leadership, stakeholders, the Product Owner, users, and team members participate to promote shared understanding and alignment to feature/function schedule, and to create a common accountability to the goals of the program and the release. Team establishes, documents, estimates, prioritizes, and refines product and/or release backlogs with user stories.
Sprint Planning | Every two weeks, at the beginning of the sprint	| Product Owner, Scrum Master, and team conduct Sprint Planning at the beginning of each sprint to establish the prioritized set of user stories to be completed throughout the sprint based on the team’s velocity. The team establishes user story estimates along with technical tasks and acceptance criteria for each user story.
Daily Stand Up	| Daily	| Stakeholders, Product Owner, and users attend daily scrums to review progress in the current sprint. Team shares what’s been accomplished, plans for the day’s work, and identifies blockers at the daily scrums to time-box the meeting for efficiency. Scrum Masters work through inhibitors to let team members to focus on work. Scrums are typically limited to 15 minutes. Issues or challenges presented in the daily scrum are deferred to one-on-one meetings following the daily scrum.
Sprint Review	| Every two weeks, at the end of the sprint |	Sprint reviews are on the last day of the sprint to communicate with the Product Owner, leaders, stakeholders, and users about sprint performance. Team reviews completed user stories, velocity, issues and progress inhibitors, and future work. Team does a Sprint Demonstration of features/functions developed during the sprint. The Product Owner accepts or rejects user stories to validate completion.
Sprint Retrospective | Every two weeks, at the sprint end |	Sprint Retro serves as a way to perform continuous improvement. The teams discuss good behaviors that should continue, poor behaviors that should stop, and ideas for improvement in upcoming sprints.
PI Review |	Every three months, at the end of the program increment |	At the end of each program increment, leaders, stakeholders, users, the Product Owner, and the development team review production features that were deployed for the current program increment. The team reviews deployment activities, communications plans, change management activities, training plans and schedules for awareness, acceptance and understanding as to how product features have been or will be deployed to user. For teams performing continuous delivery or release on demand, PI reviews serve as an opportunity to share user feedback, KPI and MPI analysis/trends, and feedback on PI features/functions released.

### Notes and References
##### [Click here for more information](./agile)

## Agile Tooling
We utilize JIRA for documenting user stories, building a backlog, sprint planning, and tracking development of features and tests within a sprint. Each user story includes a brief description in the form "AS A [USER], I WANT [A FEATURE] SO THAT I [VALUE STATEMENT]", Acceptance Criteria written in Gherkin syntax, a link to an epic with wireframes and additional technical context or assumptions as appropriate.

### Sample User Story
<p align="center">
 <img src="Example image location title="Agile User Story">
</p>

### User Story Workflow
<p align="center">
 <img src="Workflow Image title="User Story Workflow">
</p>
