**THIS IS AN EXAMPLE. DO NOT REUSE VERBATIM. TAILOR CONTENT & MESSAGING APPROPRIATLEY TO AUDIENCE** 

![alt text](image location "Stella logo")

# CI/CD (Continuous Integration/Continuous Delivery)

## Table of Contents

- [Our DevSecOps Practices](#our-devsecops-practices)
  * [Alignment on Outcomes](#alignment-on-outcomes)
  * [Design with Flexibility and Scalability](#design-with-flexibility-and-scalability)
  * [Measuring Progress using Quantitative Measures](#measuring-progress-using-quantitative-measures)
  * [Adopted DevSecOps Processes](#adopted-devsecops-processes)
- [Our Pipeline](#our-pipeline)

## Our DevSecOps Practices

<p align="left">
<img src="https://playbook.cio.gov/assets/images/usds-logo-seal.png" align="middle" title="USDS logo" width=50 height =50>
<strong>Applying <a href="https://playbook.cio.gov/#play8">Play 8</a>, <a href="https://playbook.cio.gov/#play9">Play 9</a>, <a href="https://playbook.cio.gov/#play10">Play 10</a>, <a href="https://playbook.cio.gov/#play11">Play 11</a>, and <a href="https://playbook.cio.gov/#play12">Play 12</a></strong>
</p>
At Stella, we take a different approach to DevSecOps that focuses not only 
on the latest technology capabilities in the DevSecOps ecosystem, but equally 
on the human resources, organizational, and culture change required to enable 
the people, the processes and the technology to get aligned on a common outcome
– the mission of their organization. We believe DevSecOps has something to offer
to every mission. While DevSecOps does provide technical excellence – continuous
improvement in areas like continuous integration, continuous delivery, continuous
deployment, infrastructure as code, automated testing, and the like – its primary
outcome is providing communication and collaboration between all aspects of the
organization (infrastructure, quality, security, etc.) to meet the shared mission.

### Alignment on Outcomes

Our teams begin each engagement by understanding the constraints in your current
software delivery process (from development to operations) to identify short- and
long-term outcomes. This assessment in the Discovery Phase identifies a
long-term strategy, definition of done, and outlining short-term outcomes to meet
the long-term strategy. Stella then builds a backlog of capabilities and
features for the team. Using our Design Intelligence Framework, a CMMI-Level 3 certified
approach that integrates HCD, Agile and DevSecOps, we empower teams to
collaborate with stakeholders (across the business, development, security and IT Operations) to
accomplish those outcomes using service design techniques, as experts in their
work and context. We find that by focusing on designing and executing short-term
outcomes that support a long-term strategy, teams will adjust to emergent needs.
While there is no “one size fits all” approach to DevSecOps for every program,
our experience has taught us that by building DevSecOps capabilities using an
iterative approach leads to greater adoption and fosters a culture of continuous
improvement.

### Design with Flexibility and Scalability

Stella uses a microservice-based development approach and containerized
deployment infrastructure to maximize flexibility, reuse, quality, performance,
and maintainability of our product development. Our delivery and deployment
approach provide programs with a flexible deployment architecture that allows the
USCIS to respond to changes in immigration policy, reduce the
reintroduction of flaws, and provides maximum interoperability and reuse by other
products and teams.

Our focus on building reusable artifacts such as infrastructure as code
images/scripts, microservices, and pre-accredited components of the architecture
provides fully tested, secure, scalable, quality reusable services that can be
rolled back to a previous state for any number of reasons from backing out
production changes to disaster recovery. These reusable components also maximize
efficiency in the risk management process through NIST control inheritance of
common control providers and ensure platform and networks are compliant with
USCIS guidance for security, reliability, and availability. This speeds delivery
to the mission while maximizing reuse and minimizing rework.

### Measuring Progress using Quantitative Measures

Stella captures the effectiveness of the development and delivery process
by measuring four key metrics of availability, cycle-time, deployment frequency, and quality aligned with
the DORA State of DevOps Report. We measure the throughput of the software
delivery process using **lead time** of code changes from check-in to release
along with **deployment frequency**. Stability is measured using
**time to restore** — the time it takes from detecting a user impacting incident
to having it remediated — and **change fail rate**, a measure of the quality
of the release process. Our teams identify additional program specific metrics
as defined by short- and long-term outcomes and integrate those quantitative
measures from automated processes in the CI/CD pipeline to provide metrics that
measure mission success for each program’s unique requirements.

### Adopted DevSecOps Processes

Stella’s DevSecOps approach uses the following tools and techniques, listed
in the table below. Although we might use tools listed in an initial transition-in,
our philosophy is to use the best of breed tools for any given situation. That
simply means, while we might utilize Jenkins or even a language like Ruby today,
we should always be looking for ways to improve and leverage new tools to
provide better value to our customers.

DevSecOps Activities and Techniques |	Goals, Benefits | Tools
----- | ----- | -----
Pipeline Orchestration |	Automates collection, compilation, build, deployment of software. Affords the team comprehensive automation. Significantly reduces or eliminates human error while increasing speed and efficiency in the build and deployment process. We use these tools and principles throughout development, test, and production deployments. | **Jenkins**
Source Code Control Repository	| Version control, single source of truth for code, scripts, configuration files, templates. Promotes reuse, guards against human error in code changes, etc. | **GitHub**
Artifact Repository |	Version control of libraries, promotes reuse and continuity of library and framework use across the organization, protects the organization from sprawl and security risks of open source or external dependencies, improves performance of resulting code deliverables. | **Nexus**
Automated Testing Framework |	Automated testing promotes clean coding principles, code modularity and isolation, and reliable code behavior. This increases the confidence in the code developers create, reduces risk when code is refactored, and significantly increases the ability to easily identify and track down bugs introduced into code over its life. | **Junit, Nunit, Selenium**
Code Coverage Testing| 	Validating that at least 75% of code is covered by automated unit/regression tests that run on every automated build. Failure to meet code coverage thresholds results in failed builds, which stops development until the test coverage can be met. | **Jacoco, Sonar**
Security Testing |	A subset of automated tests, focused on secure coding by ensuring dependencies are valid and secure, code meets quality and security standards, and both the code and running application have been scanned properly for potential security vulnerabilities. | **OWASP Dependency Check, OWASP ZAP, Findbugs, PMD, Checkstyle**
Performance Testing Framework |	These tests profile code performance and indicate where issues exist in code that could cause scale and/or performance problems when deployed to larger user base with greater concurrency and load. | **JMeter**
Containerization, Virtualization	| Development teams deploy software to containers for deployment across all environments. Containers and other virtualization techniques abstract physical server resources and allow teams to automate provisioning, orchestration and management of workloads running in the wide variety of deployment architectures. | **OpenShift, Docker**
Provisioning, Configuration Management, and Deployment	| Development teams use infrastructure as code to automate the provisioning and configuration management of both infrastructure and platform resources. This provides rapid deployment through automation, reduces human error, and allows security teams to accredit infrastructure and platform environments for accelerated ATOs for subsequent workloads that inherit common controls provided by automated infrastructure.  | **Terraform, Ansible**
Automated Deployment	| Deployment of software is fully automated, such that once the organization has approved workload development for production deployment, teams can use tooling to “push button deploy” vs. having to manually move workloads onto production environments. These tools and principles are used throughout development, test, and production deployments for continuity and resilience. | **Jenkins, Openshift**

## Our Pipeline

As discussed in the [Quality](./QUALITY.md) documentation, Stella has built
out a full DevSecOps pipeline, going through multiple stages, and providing feedback
at each stage. Our pipeline hits six distinct phases, balancing the impact and
celerity of the results. Each phase is composed of one or more stages, with each
one gated based on the results produced.

<p align="center">
 <img src="Iamge location title="CI/CD Pipeline Overview">
</p>

Phase | Actions | Gates | Frequency | Results
----- | ----- | ----- | ----- | -----
**Local Development** | Write Tests; Write Code; Execute Tests (locally) | Code Review (in Pull Request) |  Feature Branch  | Initatite pull request and code review
**Development** | Code Compilation and Build; Unit Testing; Code Coverage; Static Analysis | No build errors; All tests pass; 90% branch coverage; No [quality profile errors](QUALITY.md#code-quality) | Every commit and PR | Failures prevent merge, developer notified
**Integration** | Build Container; Deployment to ephemeral Integration Environment, Integration Testing; API Testing; Application Security Scan; API Tests; Feature Testing; SonarQube Quality Scan | All tests pass; 90% branch coveragel; No High or Medium severity issues, other issues have remediation plan | Every PR | Failures prevent merge, team notified
**QA** | Deployment to QA; Usability Testing; Traffic Monitoring Security Analysis; Exploratory Testing; 508 Testing | All tests pass; No High or Medium severity issues, other issues have remediation plan | Develop & Master | Failures notify team and release management
**Staging** | Deployment to Staging; Load Testing; Stress Testing; Fuzz Testing; Compatibility Testing | p>99% succeed rate at load thresholds; p>95% succeed rate at +50% load thresholds; No High or Medium severity issues, other issues have remediation plan; All tests pass | Develop & Master | Failures notify team and release management
**Production** | Deployment to Production |  | Develop & Master | Failures notify team, product owner, and release management


As a result of our usage of containerization, each time code is merged into
Develop, a docker container is built for the microservice, which is promoted
through different phases. This singular container provides confidence that the
same application and code that was tested at the Integration phase, is the same
application and code that is being promoted into production. This limits issues
from configuration, manual installation and changes, and other common deployment
problems.

<p align="center">
 <strong>Example Pull Request Pipeline Run</strong>
 <img src=image location title="CI/CD Completed PR"/>
</p>

<p align="center">
 <strong>Example Slackbot Notifications</strong>
 <img src="Iamge location title="CI/CD Slack Notifications"/>
</p>

<p align="center">
 <strong>Example Develop Pipeline Failure on Manual Testing</strong>
 <img src=Image location title="CI/CD Manual Test Failure"/>
</p>

<p align="center">
 <strong>Example Develop Pipeline Success Run</strong>
 <img src=Image location title="CI/CD Completed Develop"/>
</p>

As mentioned in our description of [quality profiles](QUALITY.md#quality-profile),
a quality profile is built for each code change, providing insight into the code
and all metrics against it. SonarQube provides a developer dashboard for deep
insight into any coding issues, including tests run, coverage obtained, security
issues, and technical debt tracking. Jenkins holds a team level dashboard providing
insight into each microservice, including tests run, stages executed, and feedback
obtained.

By virtue of building out the pipeline in this fashion, any code that makes it
through the Staging phase is clearly of high quality. Our dashboarding and
reporting makes it easy to determine what (if any) issues might exist, so our
team can make an easy go/no-go decision on the release of the software.

<p align="center">
 <strong>Example use of go/no-go approval process built into Jenkins</strong> 
 <img src=Image location title="CI/CD Reporting Regression Test">
</p>

### GitFlow and Container Promotion

As the above illustrates, we are using an industry standard GitFlow pattern to promote our
code, but we have expanded on the GitFlow model to better apply it for handling
containers. Because we are not really promoting code through our process, but
rather containers, each branch type (see frequency in the above table) performs
different actions, sometimes at the code level, and sometimes at the container
level. This modernized look at the GitFlow process was arrived at through looking
at a value stream mapping of our activities, and removing repetitive steps.

This means activities such as unit and integration tests are not run after the
code is compiled and put into a container. Our containers are not ever rebuilt,
but promoted through our artifact repository system (Nexus). This provides
confidence that only code that has been thoroughly tested can make its way into
Production, while still streamlining the process.

From all of this, different activities get kicked off from different branches, following
your typical GitFlow activities.
* Feature Branch - Development Phase
* PRs - Development and Integration Phases
* Develop - Quality, Staging and Production Phases

No actions occur on merging to release, as this is automatically handled by the
Production phase.

In the event code needs to be deployed rapidly to Production (e.g. a critical product 
bug is identified), rather than merging to develop, a hotfix pipeline is available. 
Creating a branch named `hotfix` off of the
feature branch and merging into it will trigger a more rapid hotfix workflow, going
through only the Quality and Production phases, skipping the Staging stage. This allows
for a rapid deployment, while still providing the Quality phase for more in-depth
manual examination of the changes and impacts as needed.
