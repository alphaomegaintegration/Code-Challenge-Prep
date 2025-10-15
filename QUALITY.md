**THIS IS AN EXAMPLE. DO NOT REUSE VERBATIM. TAILOR CONTENT & MESSAGING APPROPRIATLEY TO AUDIENCE** 

![alt text](Image location "Stella logo")

# Quality

## Table of Contents

- [Application Quality](#application-quality)
  * [Continuous Testing and Shifting Left](#continuous-testing-and-shifting-left)
  * [Quality Profile](#quality-profile)
  * [Behavior Driven Development](#behavior-driven-development)
  * [Test Driven Development](#test-driven-development)
  * [Developer Testing](#developer-testing)
  * [Code Quality](#code-quality)
  * [Code Review](#code-review)
  * [Functional Testing](#functional-testing)
  * [Non-Functional Testing](#non-functional-testing)
- [Scalability](#scalability)
- [Application Security](#application-security)
  * [Binary Analysis](#binary-analysis)
  * [SCA](#sca)
  * [Security Remediation Process](#security-remediation-process)

## Application Quality

Team Stella focuses on quality at all levels of the applications we build,
enabled through test automation and test driven development, which
are integrated features of the DevSecOps and CI/CD methodologies.
This ensures we are releasing our application with predictable quality
and integrity, versus simply releasing code rapidly.

To this effect, we employ a Continuous Testing approach, testing at all
levels of application development, and throughout the entire release cycle.
This includes relying heavily on a shift left approach to get testing performed
early and often, and building out feedback cycles throughout the process to
provide information to the entire team on the quality of the application at
each stage.

### Continuous Testing and Shifting Left

Team Stella adheres to the concept of shifting testing left during
planning of quality and security tests. This means performing testing as early
in the development lifecycle as possible, without slowing down the feedback and
release process. Continuous Testing takes the standard 'Shift Left' approach
and expands on it, ensuring that not only is testing done early and often, but
throughout the entire testing process, expanding right to test as late into the
release process as needed and possible.

<p align="center">
 <img src= Image location title="Shift Left">
</p>

By adhering to this process, our team not only ensures they have a known
[Quality Profile](#quality-profile) created, but also that they will get feedback
on the application state rapidly. Developer level testing such as unit tests,
code coverage and static analysis is performed rapidly, and run frequently
and early, providing insight into low level application correctness. Once this
is determined to be acceptable, the next stage of application is tested, looking
at integration between components. This builds on top of the unit level testing by
ensuring each application can talk to the other, and might include things like
integration and API testing. As these tests are dependent on the individual
code components being correct and take longer to execute, they run next, and
provide the next feedback cycle. Finally, once all of the parts appear to be
playing nicely together, only then do we look at the higher level operation
of the application, namely, does the application do what the end user wants.

This process is aligned with our typical Quality Assurance (QA) functionality. To truly
adhere to Continuous Testing, our team pushes testing further right,
encompassing the full release process. This means including longer running
security and performance testing next, pulling in, and sanitizing data from
production, to ensure accurate and useful tests that best mimic our production
environment(s).

### Quality Profile

By collecting information from testing done throughout the entire development
and release process, our team can build a quality profile for each release
candidate. This means that when it comes time to release the software, we can
make quantitative and qualitative assessments of each release candidate, and
decide what to release. This becomes extremely important within the DevSecOps
processes to ensure that we are releasing high quality software iteratively.

Our Quality Profile incorporates many components, including:
- Unit Test Results
- Branch Code Coverage
- Issues from Static Code Analysis
- Technical Debt
- Integration Test Results
- API Test Results
- Functional Test Results
- User Story/Feature Coverage
- Security Test Results
- Performance Test Results
- Data Migration Compatibility Information

### Behavior Driven Development

<p align="left">
<img src="https://playbook.cio.gov/assets/images/usds-logo-seal.png" align="middle" title="USDS Logo" width=50 height =50>
<strong>Applying <a href="https://playbook.cio.gov/#play1">Play 1</a>, <a href="https://playbook.cio.gov/#play2">Play 2</a> and <a href="https://playbook.cio.gov/#play10">Play 10</a></strong>
</p>

Behavior Driven Development (BDD) is all about fostering collaboration between the
product owner, developer and tester, often referred to as the 'three amigos.'
At Stella, we pride ourselves on building the correct solution for our
customers, the right way, and we default to BDD to ensure we design, develop, and
test the prioritized features that align to the desired user experience. This collaboration occurs throughout the entire
development process. One of the resulting documents produced during planning
are user stories with test scenarios defined that the entire team agrees upon
so that everyone understands how the end result will operate. These are referred to as
features, and have two main parts: User Story and Scenarios.

The User Story takes the form of `As a ...` `I want to...` `So that...`. This
provides context to everyone working on the application, to keep the development
and testing focused on the end user desires. The Scenarios are written in human
friendly `Given` `When` `Then` (GWT) syntax, with the Givens setting up the system, the Whens performing
some action, and the thens asserting the desired reaction occurred. These GWTs reference business operations 
to describe how each feature will operate in greater detail. 

While Stella chose the BDD techniques for the strength of its collaboration
first approach, we also make heavy use of the resulting ability to easily automate the
creation of the feature file documentation. We take these resulting documents, and
write Cucumber automated tests utilizing these statements, to ensure the desired
outcome of each new feature is achieved.

### Test Driven Development

<p align="left">
<img src="https://playbook.cio.gov/assets/images/usds-logo-seal.png" align="middle" title="USDS Logo" width=50 height =50>
<strong>Applying <a href="https://playbook.cio.gov/#play4">Play 4</a> and <a href="https://playbook.cio.gov/#play10">Play 10</a></strong>
</p>

Our development teams use Test-Driven Development (TDD) to ensure all code written
is properly instrumented with unit tests that are meaningful and relevant.
Unit tests, integration tests, and functional tests are all written alongside
the code being developed to meet user story requirements and acceptance
criteria.  We require all tests to be run on each developed feature through
the CI/CD pipeline to ensure no code is released unless it is tested for
quality and security. This provides quick feedback
loops to developers when bugs are identified, decreases debugging time, reduces the number
of defects identified in production, and encourages a team culture that values the
positive impact of thorough testing in application development.

### Developer Testing

Developers are taught to test at
the lowest unit possible to achieve confidence in the success or failure
of any given feature. This naturally leads to testing that focuses first on unit
tests over integration, or API tests over GUI tests, as seen in the Agile
Testing Pyramid. This approach reduces the burden on test maintenance while
significantly lowering test-run time and false-positive/false-negative rates.

<p align="center">
 <img src="Image location title="Agile Test Pyramid">
</p>

To this end, our developers are expected to follow TDD when writing application code. 
Each developer is expected to write good tests at the unit level
that will help guide the application code. By focusing on testing in this fashion
not only will our application code be more complete and thought out, it will result in higher code coverage, 
with effective, accurate tests. Our developers are responsible for writing
unit and integration tests for each piece of code checked in, to help build the
quality profile.

### Code Quality

<p align="left">
<img src="https://playbook.cio.gov/assets/images/usds-logo-seal.png" align="middle" title="USDS Logo" width=50 height =50>
<strong>Applying <a href="https://playbook.cio.gov/#play12">Play 12</a></strong>
</p>
Team Stella uses static code analysis to measure code quality. Tools, 
like SonarQube, are used to scan source code to identify code duplication, 
security defects, implementation bugs, and code smells (that 
indicate something might not be implemented well and might be difficult to 
maintain). Using these automated tools, we detect issues early in the 
DevSecOps Pipeline and provide quick feedback to the Developers to address 
issues with code quality. These tools also provide Developers with a 
dashboard to easily gain in-depth insights into the code quality early and often.

### Code Review

Code Review is an important component of our Agile process in which our code is assessed by one or more people on the team. A skilled reviewer
looks for inconsistencies, errors, potential bugs, problems in
design and architecture, and issues of performance and security. Although
not all software companies implement this practice, in our experience we are able to
identify vulnerabilities and security defects earlier and produce better
software through frequent code reviews. We do this through pull requests in
GitHub for consistency and efficiency.

### Functional Testing

While Steampunk focuses heavily on low level developer testing to promote
stability, maintainability, and rapid execution pace, we do fill out the
testing pyramid with a variety of functional tests. These take the form of
both automated and manual tests. We automate as many tests as reasonable,
following the MoSCoW method to alleviate repetitive, error prone, or unfeasible
manual tests. Steampunk is not an 'automate everything' shop, but rather, we
analyze our ROI for automation, and automate as much as makes sense,
sometimes 50%, sometimes 99%, depending on the nature of a given application.

<p align="center">
 <img src="Image location title="MOSCOW">
</p>

Our functional testing simulates the same actions as a user, and typically
occurs at the UI level, but might dive deeper depending on the actions trying
to be verified. These tests might be scripted, automated, exploratory, or even
ad-hoc, but are performed to provide as much coverage to the user stories.
We focus on happy path, negative path, and even malicious path testing, to
ensure all options and possibilities are covered.

### Non-Functional Testing

We extend our quality checks beyond simple functionality, to ensure the
application is setup to handle all sorts of possibilities. Our non-functional
testing capabilities often vary depending on the application, but typically
include:
- Performance Testing
- Security Testing
- Accessibility Testing
- Compatibility Testing
- Usability Testing

## Scalability

Our team takes our functional and non-functional testing beyond simple feature
and performance testing, and focuses on reliability of the application. This
means examining up-times, failover capabilities, and disaster recovery metrics.
We use modeling and measurements from our quality analysis and improvement benchmarks
to determine our reliability. To achieve this, our team follows a standard
procedure of:
- Establishing reliability goals
- Developing am (or many) operational profile(s)
- Planning and executing tests
- Using the test results to drive decisions

We follow the three segment approach of:
- Model
- Measure
- Improve

For modeling, we have experts on staff to help build both prediction and estimation
models, taking into account data reference, development cycle timelines, and
application time frames. For measuring, our teams look at 4 key metrics: product
(such as size, complexity, and coverage), project management (such as key Agile
metrics), process, and fault and failure (such as MTTF and MTTR). For improvement,
we roll our plans into our backlog, prioritizing them as needed and pulling them
into sprints as potential technical debt.

## Application Security

<p align="left">
<img src="https://playbook.cio.gov/assets/images/usds-logo-seal.png" align="middle" title="USDS Logo" width=50 height =50>
<strong>Applying <a href="https://playbook.cio.gov/#play11">Play 11</a></strong>
</p>
Team Stella believes that security is paramount when working with USCIS and 
ensures that the most up-to-date practices are incorporated and designed from each
project’s inception and throughout the design, development and deployment phases. We
strongly commit to the incorporation of security within code reviews, security 
testing, binary analysis, SCA, and security remediation process. In an effort to
reduce the attack surface of applications and their infrastructure, we provide a 
variety of security testing throughout the CI/CD pipeline. As much as feasible, we 
shift security left and attempt to (where appropriate) run security testing as 
early as possible to detect and resolve the vulnerabilities while they are being
developed. Code reviews provide an opprtunity to identify issues in the architecture of the system that may present vulnerabilities not identified in automated tooling.

### Binary Analysis

Binary analysis is used to determine the origins of all components and libraries
that are used within the software to identify any vulnerabilities that are
found in popular and commonly used components. These open-source components and
libraries are compared to a list of recently and updated documented vulnerabilities
that will advise any potential issues or out of date warnings and if any patches
are available. We leverage
[OWASP Dependency-Check](https://owasp.org/www-project-dependency-check/) to
identify vulnerable libraries at compile time, allowing us to make early changes
or patch vulnerable libraries with the "next release" or as a hotfix.

### SCA

SCA tools are run on compiled code to detect defects such as input validation,
pointers and references, numerical errors and path traversals that may be exploited
by potential vulnerabilities. Reasoning for implementing a binary analysis include
discovering vulnerabilities through decomposition and disassembly of the binary in
order to recognize vulnerability patterns. Discovering these weakness furthers the
commitment to security that is expected from our high standards. We leverage
security plugins within [SonarQube](https://www.sonarqube.org/) to identify
vulnerabilities in our software.

## Security Remediation Process

Critical and high defects discovered in the development process should be identified, break the build, and resolved prior to release. Defects originating from architecture decisions or those involving zero-day defects should be triaged and added as a bug and prioritized with user stories for remediation.
