---
title: "Scientific AI agents | IOWarp"
description: "How scientific AI agents take part in research workflows by operating real tools, data, and HPC systems, and where human judgment stays in charge."
url: https://iowarp.ai/topics/scientific-agents/
---

> How scientific AI agents take part in research workflows by operating real tools, data, and HPC systems, and where human judgment stays in charge.

# Scientific AI agents that do real work.

A scientific agent is a language-model-driven program that carries out steps of a research workflow by calling tools: reading datasets, submitting jobs, running analyses, and producing figures. Its value depends less on the model than on the tools it can operate and the context it is given.

01 What agents are good for today 02 What stays with scientists 03 Architecture matters 04 How IOWarp approaches it 05 Common questions

01

## What agents are good for today

Agents are effective at the connective work between scientific tools: finding a dataset, checking its structure, configuring a job, turning output into a plot. Demonstrations in the project cover EarthScope data through the National Data Platform, LAMMPS trajectory analysis, ParaView visualization, and IOR deployment.

In the eScience 2025 evaluation, an agent with IOWarp context completed EarthScope retrieval and visualization, while the comparison agent without that context did not complete the workflow.

02

## What stays with scientists

Choosing the question, judging whether a result is meaningful, and deciding what to publish remain human responsibilities. IOWarp designs agents to stage work for review rather than to declare conclusions.

03

## Architecture matters

A single agent with every tool attached becomes slow and error-prone. CLIO Agent packs route work through an orchestrator to domain experts and short-lived workers, each with a narrower tool set and context.

How IOWarp approaches it

## Where to go deeper.

01**CLIO Agent**

Install the scientific data agent, connect a model, and use packs with experts and workers.

Open ↗

<https://clio.iowarp.ai/docs/install/>

02**CLIO Kit**

The scientific tools agents operate, exposed through the Model Context Protocol.

Continue →

<https://iowarp.ai/clio-kit/>

03**Demonstrations**

Public recordings of agent workflows on scientific data and HPC tools.

Continue →

<https://iowarp.ai/research/demos/>

04**Anthropic on building effective agents**

Further reading: Distinguishing workflows from autonomous agents, and choosing simple, composable patterns.

Open ↗

<https://www.anthropic.com/engineering/building-effective-agents>

05**Anthropic’s multi-agent research architecture**

Further reading: An orchestrator and specialized research workers, with lessons about coordination, evaluation, and reliability.

Open ↗

<https://www.anthropic.com/engineering/multi-agent-research-system>

Applications that use it

- A1
  ### [Agents in the materials workflow](https://iowarp.ai/applications/materials-science/)
  Design on HPC, additive manufacturing, X-ray tomography, and fatigue testing: the Utah team’s reference workflow, and the agent tools built for it.
  Active collaboration
- A2
  ### [Agents on the National Data Platform](https://iowarp.ai/applications/national-data-platform/)
  MCP tools that let an agent search, stage, and analyze datasets federated through the National Data Platform, first shown on EarthScope data.
  Demonstrated on EarthScope data
- A3
  ### [Provenance and integrity for AI-driven science](https://iowarp.ai/applications/genesis-spotter/)
  A DOE Genesis Mission project at Argonne National Laboratory that traces integrity attacks on scientific AI workflows to their source. CLIO Agent provides the investigating agents.
  Project began August 2026

Common questions

## Common questions.

**Which models does IOWarp require?**

None in particular. The software is designed to work with institutional, local, and commercial models; demonstrations have used several agent and model combinations.

**Are the agents autonomous?**

Operators set how much runs without approval through approval modes and permission gates. CLIO Researcher is designed to stage changes for human review rather than accepting them automatically.

Related

## Research and demos on this topic.

- [Research direction **Staging data while agents think** Can reasoning time hide I/O time?](https://iowarp.ai/research/directions/#staging)
- [Research direction **Authority that travels with work** What can a delegated agent actually do?](https://iowarp.ai/research/directions/#authority)
- [Research direction **Provenance an agent can question** When a result is wrong, can we find out why?](https://iowarp.ai/research/directions/#provenance)
- [Demo **EarthScope through the National Data Platform, 2026** Planned for 2026](https://iowarp.ai/research/demos/#demo-earthscope-through-the-national-data-platform-2026)
- [Demo **Materio for materials research** Planned for 2026](https://iowarp.ai/research/demos/#demo-materio-for-materials-research)
- [Demo **DOE Genesis: SPOTTER-AI and PORTUS** Planned for 2026](https://iowarp.ai/research/demos/#demo-doe-genesis-spotter-ai-and-portus)

## References

1. [Islam, Cernuda, Muradli, Kougkas, Sun. Towards an AI-driven scientific workflow. IEEE eScience 2025 (poster)](https://doi.org/10.1109/eScience65000.2025.00074)
2. [eScience 2025 poster PDF: EarthScope, LAMMPS, ParaView, and IOR agent workflows](http://cs.iit.edu/~scs/assets/files/islam2025aidriven_poster.pdf)
3. [Agent examining EarthScope data through the National Data Platform (video, October 2025)](https://www.youtube.com/watch?v=9NUf76wnHhA)
4. [Anthropic on building effective agents](https://www.anthropic.com/engineering/building-effective-agents)
5. [Anthropic’s multi-agent research architecture](https://www.anthropic.com/engineering/multi-agent-research-system)

## Other concepts

- [T1 Context management for AI agents](https://iowarp.ai/topics/context-management/)
- [T3 MCP servers for scientific computing](https://iowarp.ai/topics/mcp-for-science/)
- [T4 HPC I/O and storage hierarchies](https://iowarp.ai/topics/hpc-io/)
- [T5 Data movement for AI-infused workflows](https://iowarp.ai/topics/data-movement/)
- [T6 Scientific workflows and reproducible deployment](https://iowarp.ai/topics/scientific-workflows/)
- [T7 Evidence-based autonomous research](https://iowarp.ai/topics/evidence-based-research/)

Next step

## See this topic at work.

[Agents in the materials workflow](https://iowarp.ai/applications/materials-science/) [All concepts](https://iowarp.ai/docs/#concepts)
