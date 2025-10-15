**THIS IS AN EXAMPLE. DO NOT REUSE VERBATIM. TAILOR CONTENT & MESSAGING APPROPRIATLEY TO AUDIENCE** 


![alt text](Image location "Product Vision Cover")

# Product Vision

## Vision Statement
*A **full application lifecycle system** that will **accept and adjucate digital I-131 forms** for **applicants who are lawful permanent residents** or **conditional permanent residents** by **providing an interactive**, **responsive web portal for applications**, **a case management solution for processing benefits**, and a **reporting & dashboarding system to monitor performance and ensure timely processing**.*

## Problem

**Who** (for) | **Why** (need or desire)
---------- | ----------------
Applicant (Lawful Permanent Resident or Conditional Permanent Resident)     |  Need a digital form to apply for a re-entry permit, refugee travel document, or advance parole travel document, including parole into the U.S. for humanitarian reasons.
Adjudicator | Need a simplified system that allows for application form data to flow into a case that can be easily adjudicated with defined business rules and successful security checks.
Business Owner | Need to be able to analyze the I-131 process to identify improvements that can be made to the application business rules, overall processing times, and system bottlenecks.
External System User | Need to have access to query API inspectors such as Swagger to query from our microservice data sources. These microservices contain mock data for reference and transactional data that is collected from the different web applications.

## Solution

**What**  | **How** (differentiated)
---------- | ----------------
Applicant Form I-131 Portal     |  An interactive, responsive, web-based digital form that captures accurate I-131 data for different applicant types (re-entry, refugee, advanced parole) and collects payment information that can be sent to a case adjudicator.
Case Management Portal    |  An interactive, responsive, web-based case management system that allows an adjudicator to 1) Accept an I-131 case 2) Be assigned an I-131 case 3) Validate an I-131 case against multiple security checks such as the existience of the Applicant's A Number and that the Applicant name is a match for that A number 4) Confirm that multiple business rules for adjudication, such security checks, have been validated and the Applicant's fee receipt is attached to the case  5) Reject or Approve a case based on the business rules and security checks.
Security Check Solution   |  A microservice that will take the case and its associated form data and perform a series of security checks on the applicant.
Client Print Application    |  A desktop client that an internal USCIS adjudicator can use to output the I-131 case data to a local printer, including the applicant's Receipt, Fee Acceptance and Approval Notice correspondence.
Correspondence Application    |  A microservice that will generate PDF correspondence to attach to cases, to mail to applicants and to be printed and mailed.
BI Reporting & Dashboarding Tool  |  An interactive, responsive, web-based reporting and dashboarding application that a USCIS I-131 business owner or administrator can use to perform business intelligence operations, such as viewing page and workflow analytics, user metrics, case approval and rejection metrics, processing times, and that provides the ability to create their own ad-hoc reporting capabilities.
External API | Using Swagger, an API inspector tool that allows for the external system user to query data sources that align to the front end web application and the database supporting each microservice.
