# Changelog

This changelog records substantive changes to the reusable instructions and custom prompt for evidence-informed environmental policy and operational decision support.

The project follows Semantic Versioning. Versions below 1.0.0 are developmental and may introduce substantial changes to structure or expected behaviour.

## [Unreleased]

### Planned

- Test the instructions against representative UK and European environmental policy and operational decision-making tasks.
- Assess consistency across Microsoft Copilot and other supported AI systems.
- Refine the balance between concise synthesis and supporting evidence.
- Add worked examples or test cases covering water resources, biodiversity, land use and climate adaptation.
- Consider separating the current material into core instructions, a research playbook and task-specific prompt templates.

## [0.2.0] - 2026-11-09

### Summary

Substantially revised the initial instructions and prompt following iterative critical review across Microsoft Copilot and an external model.

This version strengthens evidence appraisal, environmental applicability, operational decision support, AI evaluation, source verification, governance and user control over the analytical scope.

### Added

#### Evidence and decision framework

- Added an explicit evidence-to-decision lifecycle covering data, information, evidence synthesis, interpretation, decisions, implementation, monitoring, evaluation and learning.
- Expanded the definition of relevant evidence to include research, monitoring, administrative and operational data, models, evaluations, practitioner experience, stakeholder knowledge, local and Indigenous knowledge, legal duties, public values and distributional effects.
- Added a requirement to distinguish evidence-informed analysis from advocacy.

#### Evidence appraisal

- Added claim-specific evidence appraisal rather than relying on a universal source hierarchy.
- Added distinctions between established findings, emerging evidence, documented but unevaluated practice, interpretation, projections and speculation.
- Added explicit treatment of conflicting evidence, uncertainty, transferability and evidence gaps.
- Added a requirement to distinguish:
    1. technical performance;
    2. workflow performance;
    3. user and organisational outcomes;
    4. decision quality;
    5. environmental and societal outcomes.
- Added consideration of human baselines, including disagreement among human analysts, expertise and workload.

#### Research and source verification

- Added separate searches for materially different research questions.
- Added a requirement to inspect primary sources behind important figures, evaluation results and consequential claims where available.
- Added explicit handling of sources available only through snippets, abstracts, press releases, aggregators or vendor material.
- Added citation chaining and targeted follow-up searches for claims central to the conclusion.
- Added visible annotated source-list requirements, including source type, date, primary or secondary status, supported claim and important limitation.
- Added a prohibition on presenting a secondary account as though the original source had been examined.
- Added an explicit distinction between targeted rapid reviews and systematic or comprehensive reviews.

#### AI taxonomy and maturity

- Added distinctions between generative AI, predictive machine learning, information extraction, retrieval-augmented generation, semantic search, knowledge graphs, digital twins, deterministic models, orchestrated workflows and agentic systems.
- Clarified that an API, tool interface or MCP server is not itself an agent.
- Added an AI maturity classification:
    - proposal;
    - prototype;
    - pilot or trial;
    - limited operational deployment;
    - established operational use.
- Added distinctions between independently measured, internally evaluated, estimated, projected and unsupported results.
- Added an agentic-system assessment covering autonomy, permissions, available tools, executable actions, approval points, stopping rules, fallback mechanisms, logging and accountability.
- Added a requirement to consider whether a simpler non-AI approach would be more reliable, transparent, maintainable or cost-effective.

#### AI-specific risks

- Added fabricated citations, unsupported statements, prompt sensitivity, non-determinism and model-version drift.
- Added retrieval failure, automation bias, data leakage, cybersecurity and prompt-injection risks.
- Added loss of provenance, weak reproducibility and optimisation of measurable proxies rather than intended outcomes.
- Added risks arising from exclusion of local, experiential and non-digitised knowledge.

#### Environmental evidence

- Added explicit checks for spatial and temporal autocorrelation, non-stationarity, changing baselines, rare events and ecological thresholds.
- Added monitoring sparsity, geographic and taxonomic bias, changing measurement methods, detection limits and quality-control flags.
- Added checks for scale mismatch, cumulative effects and multiple forms of uncertainty.

#### Operational decision-making

- Added a separate operational track for flood warnings, drought triggers, abstraction control, pollution response and land-management interventions.
- Added assessment of latency, decision frequency, false-positive and false-negative costs, uncertainty thresholds and error tolerance.
- Added human-in-the-loop and human-on-the-loop supervision, override, escalation, degraded operation, fallback, incident response and recovery.
- Required evaluation criteria to reflect the consequences of the specific decision rather than generic model-accuracy thresholds.

#### AI-ready data and knowledge

- Clarified that open, FAIR or API-accessible data is not automatically AI-ready.
- Added machine-readable structure, semantics, provenance, versioning, processing history, uncertainty, representativeness and data drift.
- Added licensing, intellectual property, secure access, permitted uses, stewardship, correction mechanisms and sustainable maintenance.
- Extended AI readiness beyond datasets to documents, models, ontologies, software and guidance.
- Made AI readiness dependent on fitness and validation for a defined use.

#### Jurisdiction and governance

- Added explicit consideration of England, Scotland, Wales, Northern Ireland and European contexts.
- Added checks for potentially applicable requirements, including:
    - the UK Algorithmic Transparency Recording Standard;
    - UK GDPR;
    - Environmental Information Regulations;
    - the Aarhus Convention;
    - public-law and consultation obligations;
    - the EU AI Act;
    - EU open-data and high-value dataset requirements;
    - intellectual-property, procurement, security, records-management and audit obligations.
- Added a requirement to establish applicability rather than assuming that every listed regime applies.
- Added a distinction between legislation, mandatory duties, standards, guidance and good practice.

#### Organisational and environmental sustainability

- Added procurement, interoperability, portability, vendor lock-in and digital sovereignty.
- Added organisational skills, supplier dependence, automation bias and professional deskilling.
- Added total operating costs, long-term funding and stewardship.
- Added consideration of AI-related energy, carbon and water use.

#### Recommendations and confidence

- Required recommendations to be labelled as analytical judgement rather than presented as established fact.
- Added requirements to connect recommendations to evidence, assumptions and trade-offs.
- Added a requirement to explain what evidence or circumstances could change an important recommendation.
- Added confidence statements for headline conclusions.
- Added explicit review limitations and evidence-gap reporting.

### Changed

#### Scope control

- Replaced the previous instruction to adopt sensible defaults automatically.
- Made the following required user-controlled scope parameters:
    - decision, policy problem or research question;
    - intended users and audience;
    - jurisdiction;
    - timeframe and evidence cut-off;
    - domains, interventions and outcomes;
    - type of review or analysis.
- Required substantive work to pause when a required parameter is missing or materially ambiguous.
- Allowed sensible defaults or analyst-defined assumptions only when explicitly authorised by the user.
- Required user-specified scope and analyst-assumed scope to be distinguished.
- Added a short scope restatement before substantive research begins.

#### Length and proportionality

- Replaced a fixed one-page default with proportionate, audience-sensitive length.
- Separated the full working appraisal from the smaller set of attributes that should appear in a concise output.
- Required concise outputs to prioritise maturity, comparator, measured or projected result, principal limitation and decision relevance.
- Added a rule for handling conflict between length and coverage.
- Recommended supporting tables or annexes only where they add material value.

#### Recency

- Replaced an unconditional preference for recent sources with a balanced rule: prioritise recent evidence for changing technologies, policy and practice, while retaining older authoritative or foundational sources where relevant.

#### Exemplars

- Replaced the requirement to provide an example for every domain regardless of evidence quality.
- Required deliberate searching across all requested domains while permitting the response to state that no credible or adequately evaluated exemplar was found.
- Required examples to demonstrate an analytical point rather than form a catalogue of projects.

#### Cross-domain learning

- Strengthened the use of health and other comparator domains by requiring an explicit transferability assessment.
- Added decision type, causal structure, reference standards, data-generating process, spatial and temporal scale, reversibility of errors, and institutional and legal context as transferability criteria.

### Removed

- Removed silent adoption of analyst-selected defaults for fundamental scope decisions.
- Removed the implication that source types can always be ranked using a single fixed hierarchy.
- Removed the assumption that technical model performance demonstrates better policy, operational or environmental outcomes.
- Removed the implication that every requested domain must be represented by an exemplar even when credible evidence is unavailable.
- Removed the treatment of interfaces such as APIs or MCP servers as inherently agentic.
- Removed the rigid expectation that the full analytical scope can always be represented responsibly on one page.

## [0.1.0] - 2026-11-09

### Summary

Created the initial coherent draft of reusable instructions and a custom prompt for reviewing the role of generative and agentic AI in environmental policy and operational decision-making.

### Added

- Defined the role of a senior UK and European environmental and public-policy evidence specialist.
- Established an initial evidence hierarchy and preference for authoritative and primary sources.
- Added distinctions between demonstrated practice, emerging evidence, projections and speculation.
- Introduced the evidence-to-decision lifecycle.
- Added initial treatment of generative AI, retrieval-augmented generation, knowledge graphs, predictive models, digital twins and agentic systems.
- Added initial AI-ready data criteria extending beyond FAIR principles and basic API access.
- Added environmental considerations covering spatial and temporal effects, monitoring gaps, changing baselines and uncertainty.
- Added human oversight, accountability, transparency and contestability.
- Added an initial custom prompt covering water resources, biodiversity, land use, climate adaptation and lessons from health.
- Required concise, evidence-led writing with practical exemplars, citations and a review-limitations statement.
