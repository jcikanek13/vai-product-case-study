# VAi: From Business Questions to Reviewed Action

**A product case study by Jim Cikanek**  
**Product leadership and AI-assisted development**

VAi is Venntier's internal conversational work platform for research, company knowledge, business analysis, and team workflows. It brings those capabilities into one interface with text and voice interaction.

This case study shows how I translated business needs into product boundaries, workflows, acceptance criteria, and iterative AI-assisted development. The internal application's source code and business data are excluded.

## The problem

A useful answer is often only the beginning of a business task. Teams still need to check sources, distinguish facts from interpretation, run repeatable calculations, prepare a proposal, and move it through review and follow-up.

VAi was designed for employees in product, sales, strategy, leadership, and operations who perform that work. The product connects conversation to structured workflows while preserving the authority of evidence, business rules, permissions, and human approvals.

## My role

I led product definition and the iterative development process: framing user problems, designing workflows, sequencing milestones, defining acceptance criteria, reviewing behavior, and deciding when work required remediation or should be deferred.

AI development tools supported implementation, testing, and documentation. My focus was on directing that work and evaluating it against explicit product requirements.

## What VAi includes

The local project record documents these capabilities. Their presence in the internal implementation does not imply that every live integration has completed acceptance.

| Capability | Purpose |
| --- | --- |
| Conversational workspace | Persistent conversations with typed and voice interaction |
| Market research | Company research, comparisons, provenance, and separation of facts from inference |
| Signals | Monitoring and review of findings for potential knowledge capture or follow-up |
| ROI/TCO analysis | Repeatable calculations using a deterministic engine and structured assumptions |
| Company knowledge | Review and use of approved internal context |
| Commercial work | Draft outputs connected to research and approved context |
| Team workflows | Assignments, reviews, handoffs, notifications, and a consolidated My Work view |
| Connected tools | Google Workspace-oriented actions governed by configuration, permissions, and confirmation |

## Five decisions that shaped the product

**1. Keep calculations authoritative.** The assistant interprets requests and helps users navigate an analysis. A deterministic ROI/TCO engine calculates the financial results from validated inputs.

**2. Separate evidence from interpretation.** External facts, approved company knowledge, assumptions, calculated results, and AI inference have different meanings. Preserving those distinctions makes the answer easier to evaluate.

**3. Build approvals into the workflow.** Preparing an action and authorizing its execution are separate steps. Identity, permissions, evidence, and approval rules control protected actions.

**4. Give employees one assistant interface.** Specialized capabilities operate behind VAi, allowing users to work through a consistent interface without choosing among multiple assistant identities.

**5. Treat operational readiness as part of delivery.** Implemented code, simulated-provider tests, live integration acceptance, and production readiness require different evidence. Milestone decisions account for those differences.

See [Product decisions](PRODUCT_DECISIONS.md) for supporting evidence and tradeoffs.

## How I worked with AI

I used bounded build instructions with explicit requirements, constraints, acceptance criteria, and stopping conditions. Development proceeded through milestones, with targeted verification and remediation when observed behavior did not meet the requirement.

Product leadership remained responsible for choosing the problems, defining business rules, setting approval boundaries, interpreting failures, and accepting or deferring work. The case study illustrates that process; it does not claim measured development-speed or cost improvements.

## Evidence and current status

| Evidence level | Status described in the October 2026 local project record |
| --- | --- |
| Implemented locally | Core workflows, persistence, permissions, collaboration, and operational controls |
| Tested using isolated fixtures | Substantial historical evidence for browser workflows, provider behavior, identity, connectors, and recovery paths |
| Dependent on live services | AI responses, research, Google integrations, and enterprise identity require configuration and live acceptance |
| Deferred or unfinished | Selected live acceptance, final production cutover, and remaining operational work |

The internal readiness assessment describes VAi as **ready with conditions for an initial single-host internal deployment**. Production cutover remains paused pending suitable dedicated storage and the remaining deployment work.

The case-study preparation did not rerun the application tests. Historical reports establish prior results, not a fresh passing build. There is no public runnable demonstration at this stage, and no adoption, time-savings, or business-outcome metrics are claimed.

VAi is an internal business system. Protected health information is outside its scope. This case study makes no claim of HIPAA readiness, enterprise certification, or high availability.

## Planned demonstration

A proposed three-to-five-minute walkthrough uses fictional organizations and synthetic information to show research, inspection of facts and inference, a deterministic ROI/TCO scenario, and a review or assignment workflow.

The [Demo plan](DEMO.md) describes the sequence. The [Screenshot plan](SCREENSHOT_PLAN.md) describes the proposed visuals. These documents are plans; screenshots and a recording have not yet been produced.

## About this case study

This is a documentation-based portfolio case study. No internal source code, operational runbooks, provider configuration, user records, or proprietary research are included.
