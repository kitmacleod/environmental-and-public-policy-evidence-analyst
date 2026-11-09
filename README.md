

# Environmental Evidence and Policy AI Instructions

Reusable instructions and prompt templates for evidence-informed analysis of environmental policy and operational decision-making in the UK and Europe.

**Current version:** v0.2.0

**Status:** Draft for testing

## Purpose

These artefacts help AI assistants work as rigorous environmental and public-policy evidence analysts.

They are designed for questions involving:

- water resources;
- biodiversity;
- land use and management;
- climate adaptation;
- environmental data and research infrastructure;
- generative and agentic AI in evidence and decision workflows.

The instructions emphasise primary-source verification, environmental context, calibrated confidence and clear distinctions between technical performance, workflow improvements, decision quality and environmental outcomes.

## Repository contents

| Artefact | Purpose |
| --- | --- |
| `environmental-policy-evidence-instructions.md` | Reusable core instructions governing research, evidence appraisal, AI assessment and writing |
| `generative-agentic-ai-review-prompt.md` | Custom prompt for reviewing generative and agentic AI in environmental decision-making |
| `CHANGELOG.md` | Record of substantive changes between versions |

Adjust the filenames above if different names are used in the repository.

## Key principles

The instructions require the AI assistant to:

- confirm the question, users, jurisdiction, timeframe, domains, outcomes and review method before starting;
- block substantive work when required scope parameters are missing, unless the user explicitly authorises sensible defaults;
- distinguish targeted rapid reviews from systematic or comprehensive reviews;
- verify important claims against primary sources where available;
- separate proposals, prototypes, pilots and operational deployments;
- distinguish measured results from estimates, projections and unsupported claims;
- assess policy and time-critical operational decisions differently;
- identify uncertainty, conflicting evidence and negative findings;
- consider environmental, legal, institutional and organisational context;
- treat recommendations as evidence-informed analytical judgements;
- produce concise outputs without removing qualifications that could affect a decision.

## Using the artefacts

1. Add the core instructions to the AI system’s persistent instructions, project context, notebook or equivalent configuration.
2. Complete the required fields in the custom prompt.
3. Provide or confirm:
    - the decision or research question;
    - intended users;
    - jurisdiction;
    - timeframe and evidence cut-off;
    - domains, interventions and outcomes;
    - required type of review or analysis.
4. Run the prompt using an AI system with access to current and inspectable sources.
5. Review the output and annotated sources before relying on it for a consequential decision.

The instructions are initially designed for Microsoft Copilot but use platform-neutral language where practical.

## Important limitations

These artefacts improve consistency and transparency but cannot guarantee factual accuracy, complete evidence coverage or sound decisions.

AI-generated analysis should not replace:

- subject-matter expertise;
- formal systematic-review methods where these are required;
- legal, regulatory or statistical review;
- accountable human judgement;
- validation of operational systems under realistic conditions.

Source access, search quality and instruction-following behaviour will vary between AI systems.

## Development status

Version 0.2.0 is suitable for structured testing but is not yet a stable release.

Testing should cover representative cases in water resources, biodiversity, land use and climate adaptation, including both policy analysis and operational decision support.

See CHANGELOG.md for the development history.

## Contributing

Contributions are welcome, particularly:

- worked examples and test cases;
- evidence of failure modes or unintended behaviour;
- improvements to UK, devolved-nation and European coverage;
- experience applying the instructions across different AI systems;
- clearer or more concise wording that preserves analytical rigour.

Please describe the use case, expected behaviour, observed output and proposed change when raising an issue or pull request.

