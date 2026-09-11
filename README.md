# Innovation Agent

The Innovation Agent is a specialist agent designed to support a broader Chief of Staff Agent. It helps leaders identify promising opportunities, evaluate and prioritize them, and design controlled experiments or pilots before broader implementation.

This repository is an early prototype exploring how specialized agents can contribute to executive decision support.

## Role in the Agent System

The Chief of Staff Agent acts as the orchestrator. It assigns innovation-related work to the Innovation Agent and combines its findings with input from other specialist agents.

The Innovation Agent may recommend involvement from:

- Data Analyst Agent for quantitative analysis and measurement
- Compliance Agent for policy, privacy, security, regulatory, and governance review
- Project Management Agent for detailed planning and execution monitoring

The Innovation Agent provides decision support. It does not independently approve funding, authorize implementation, or make executive decisions.

## Core Skills

### 1. Opportunity Discovery

Identifies unmet needs, inefficiencies, relevant trends, and potential innovation opportunities.

[View the Opportunity Discovery skill](.agents/skills/opportunity-discovery/SKILL.md)

### 2. Opportunity Assessment and Prioritization

Evaluates and ranks opportunities based on strategic alignment, stakeholder value, feasibility, evidence, effort, risk, and time to value.

[View the Opportunity Assessment and Prioritization skill](.agents/skills/opportunity-assessment-prioritization/SKILL.md)

### 3. Experimentation and Implementation

Converts an assessed opportunity into a proof of concept, prototype, experiment, pilot, or implementation recommendation with defined measures and decision criteria.

[View the Experimentation and Implementation skill](.agents/skills/experimentation-implementation/SKILL.md)

## Typical Workflow

1. Discover and define potential opportunities.
2. Assess and prioritize the strongest opportunities.
3. Design a controlled experiment or pilot.
4. Return findings, risks, recommendations, and decisions needed to the Chief of Staff Agent.

Not every request requires all three stages. The agent begins at the stage appropriate to the available evidence and prior decisions.

## Example Use Case

**Question:** Should an organization pilot an AI tool that summarizes executive meeting materials?

The Innovation Agent can:

- Define the organizational need and candidate opportunity
- Assess expected value, feasibility, risk, and evidence
- Recommend whether to proceed to a pilot
- Design the pilot hypothesis, scope, success measures, and stop conditions
- Identify where data, compliance, and project-management support is required

## Repository Structure

```text
innovation_agent/
├── AGENTS.md
├── README.md
└── .agents/
    └── skills/
        ├── opportunity-discovery/
        │   └── SKILL.md
        ├── opportunity-assessment-prioritization/
        │   └── SKILL.md
        └── experimentation-implementation/
            └── SKILL.md
```

## Status

Early-stage prototype for professional development and concept validation. The current version establishes the Innovation Agent’s role, routing instructions, core skills, outputs, handoffs, and guardrails.
