# VAi Product Decisions

**Product choices, tradeoffs, and supporting evidence**

These decisions summarize choices described in the supplied local project record. The evidence descriptions below refer to internal documentation and historical verification; those materials are not included in this public case study and were not independently revalidated during editorial review.

## 1. Keep calculations authoritative

**Problem:** Financial analysis requires consistent arithmetic, validated assumptions, and repeatable results. A language model's explanation should not become the source of the financial figures.

**Decision:** Route conversational intent into a deterministic ROI/TCO engine. Validate structured inputs and render authoritative figures from the engine's output.

**Tradeoff:** This requires maintaining calculation logic, input schemas, and validation. Users gain results that can be reproduced and reviewed independently of model phrasing.

**Evidence described in the record:** An independent calculation engine; policy boundaries around model-authored figures; structured inputs with units, provenance, validation, and revision history.

## 2. Separate evidence from inference

**Problem:** Research is difficult to assess when external facts, internal definitions, assumptions, and AI interpretation are blended together.

**Decision:** Preserve distinct layers for external source facts, approved company context, and AI inference. Label assumptions and calculated outputs separately, and keep research gaps visible.

**Tradeoff:** The interface and data model require more structure, and an incomplete assessment may remain conditional. Users can inspect the basis of a recommendation and distinguish evidence from interpretation.

**Evidence described in the record:** Research-fit and knowledge-capture policies; explicit treatment of source facts and inference; support for partially completed research.

## 3. Separate proposals from authorization

**Problem:** Generating a recommendation does not establish permission to perform the resulting action.

**Decision:** Let the assistant prepare proposals while the application enforces identity, permissions, approval, and execution boundaries. The model cannot approve its own action.

**Tradeoff:** Some workflows require additional interaction and explicit state management. Actions remain attributable and reviewable, including cancellation and failure history.

**Evidence described in the record:** Distinct proposal, approval, and execution states; tool boundaries that exclude model approval authority; retained action history.

## 4. Present one assistant interface

**Problem:** Employees need a clear place to begin work across research, analysis, knowledge, and coordination.

**Decision:** Present VAi as one conversational identity, with modular tools, calculation engines, and workflows behind the interface.

**Tradeoff:** Intent routing and context handling must cover several kinds of work without obscuring capability boundaries. Users gain a consistent entry point for their work.

**Evidence described in the record:** A single employee-facing identity; separate tool and capability registries; authoritative functions operating behind the conversational interface.

## 5. Require separate deployment evidence

**Problem:** A locally implemented feature does not establish that a system can be operated reliably with live services and real deployment constraints.

**Decision:** Evaluate operational readiness separately from feature completion. Identity, persistence, migrations, scheduling, backup, and recovery receive explicit acceptance work and stopping conditions.

**Tradeoff:** Deployment can be delayed by dependencies that do not prevent local development. The release decision becomes grounded in operational evidence.

**Evidence described in the record:** A conditional readiness assessment; historical isolated recovery and provider-failure exercises; a deployment pause when proposed storage did not meet the intended standard.

## What these decisions demonstrate

The case study connects product requirements to implemented boundaries and acceptance decisions. It does not claim that every alternative was formally evaluated, that all live integrations passed acceptance, or that business impact has been measured.

[Return to the case study](README.md)
