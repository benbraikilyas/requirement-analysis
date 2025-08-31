# Requirement Analysis in Software Development 
--------------

# What is Requirement Analysis?

It is the process of understanding what stakeholders (users, customers, business, legislation, etc.) need from a system, then formulating these needs as clear, testable, and consistent requirements that guide design, development, and testing.

Why is it important in the SDLC?

Reducing risk and rework: Most project errors stem from vague or incomplete requirements. Clarifying them early saves time and money.

Foundation of planning and estimating: Teams cannot accurately estimate effort and duration without specific requirements.

Alignment of expectations: Ensures that what is built is what the business and users actually need.

Test and acceptance reference: From which acceptance criteria and validation tests are derived.

Compliance and quality: Highlights legal/security/operational constraints early.

Location within the SDLC (model comparison)

Waterfall: Strong emphasis on comprehensive documentation (SRS) before design. Any subsequent change is costly.

Agile: Iterative and incremental analysis across a backlog (Epics, User Stories), with continuous refinement and acceptance criteria for each story.

Result: In both cases, analysis is ongoing; however, in Agile, it is closer to the user and more flexible.

Types of Requirements

Functional: What the system should do (book a ticket, log in, etc.).

Non-Functional: How it should work (performance, security, scalability, availability, maintainability, usability, etc.).

Constraints: Prescribed technologies, regulations (GDPR, HIPAA), integrations, budget, deadlines.

Business: Project goals, value, and success indicators.

Requirements Analysis Activities (from start to finish)

Elicitation
Interviews, workshops, monitoring, document analysis, surveys, competitor research, prototypes.

Analysis and Classification
Cleaning up duplicates, resolving conflicts, modeling processes and data, and segmenting them into stories/use cases.

Prioritization
MoSCoW (Must/Should/Could/Won’t), Value vs. Risk, WSJF… to ensure the most important things are built first.

Modeling
Use Cases, User Stories, BPMN for processes, UML (sequence/activity) diagrams, ERD for data, scenarios/personas.

Documentation
SRS (Software Requirements Specification) or Product Backlog.

For each requirement: identifier, description, cause/source, priority, status, acceptance criteria, dependencies, and risks.

Validation & Verification
Reviews with stakeholders, testable prototypes, BDD/Gherkin to link requirements to tests.

Traceability & Change Control
A traceability matrix (business objective → requirement → design → test), and processes for approving changes and releasing versions.

Requirements Quality Criteria (short for "good and testable")

Correct, unambiguous, complete, and consistent.

Prioritized, verifiable/measurable, adaptable, and traceable.

Use testable language: clear numbers and thresholds (e.g., "≤ 2 seconds for P95").

Useful Techniques and Tools

Techniques: Structured interviews, brainstorming, user stories + acceptance criteria, graphical prototyping, rapid prototyping, user journey maps.

Tools: Jira/Azure DevOps (backlog), Confluence/Notion (documentation), Draw.io/PlantUML, DOORS/Jama (advanced traceability).

Metrics for Monitoring Health

Requirement volatility (how many changes/releases),

Traceability coverage (how many requirements are associated with a test),

Post-release defects associated with requirements,

Rate of rework due to ambiguity.

Common Mistakes and How to Avoid Them

Vagueness and general language → Use examples, numbers, and acceptance criteria.

Scope creep → Change governance + clear priority.

Jump to technical solutions early → Focus on the problem/value first.

Ignore non-functionality and legal constraints → Early checklists.

Late stakeholder engagement → Stakeholder map + RACI.

Quick application example (e-commerce)

User story:
As a customer, I want to track my order to know when it will be delivered.

Acceptance criteria:

The tracking number appears within ≤ 5 minutes of shipping.

Status update time is no more than 2 seconds (P95).

Tracking is available from web and mobile.

Non-Functional:
99.9% availability per month, scalable to 10k requests/minute, payment data encryption (PCI-DSS).

Traceability: This story is associated with an interface design file, a tracking service, and two test cases.

Expected deliverables (Deliverables)

SRS or Product Requirements Document, or Backlog (Epics/Stories).

BPMN process models, use cases, prototypes, ERD, traceability matrix, glossary.

Quick pre-closure checklist

Is each requirement clear, testable, and sourced?

Have we prioritized and documented constraints?

Have we covered non-functionality?

Do we have corresponding acceptance criteria and tests?

Is the traceability from objectives → requirements → tests complete?
