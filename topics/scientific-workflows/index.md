---
title: "Scientific workflows and reproducible deployment | IOWarp"
description: "Agentic scientific workflows that stay reproducible: Jarvis deployment pipelines, simulation integrations, and agent steps with recorded provenance."
url: https://iowarp.ai/topics/scientific-workflows/
---

> Agentic scientific workflows that stay reproducible: Jarvis deployment pipelines, simulation integrations, and agent steps with recorded provenance.

# Agentic workflows you can run again.

A scientific workflow chains simulation, analysis, AI, and visualization steps across machines. It is only useful as evidence if another person can run it again and get an explainable result.

01 Deployment as a record 02 Integrations 03 Agent-operated steps 04 How IOWarp approaches it 05 Common questions

01

## Deployment as a record

Jarvis describes a software stack and its resources as a pipeline that can be deployed, monitored, and torn down. CLIO Core ships pipelines for Aurora, Delta, local machines, and other targets, so a run records its own configuration.

02

## Integrations

The workflow integration catalog covers simulations such as LAMMPS and Gray-Scott, storage services, and I/O benchmarks such as IOR and FIO.

03

## Agent-operated steps

When an agent performs a step, the tool calls and their results become part of the workflow record. The IOR deployment evaluation in the eScience 2025 poster measured agents configuring the benchmark across several agent and model combinations and prompt variations.

How IOWarp approaches it

## Where to go deeper.

01**Jarvis**

Deployment pipelines and packages for simulations, services, and benchmarks.

Continue →

<https://iowarp.ai/platform/#jarvis>

02**Application stories**

Materials science, the National Data Platform, DOE Genesis Mission projects, and national systems.

Continue →

<https://iowarp.ai/applications/>

03**CLIO Kit**

Slurm, Spack, and Jarvis servers that let an agent operate the workflow’s schedulers and deployments.

Continue →

<https://iowarp.ai/clio-kit/>

Applications that use it

- A1
  ### [Agents in the materials workflow](https://iowarp.ai/applications/materials-science/)
  Design on HPC, additive manufacturing, X-ray tomography, and fatigue testing: the Utah team’s reference workflow, and the agent tools built for it.
  Active collaboration
- A4
  ### [Agentic workflows across HPC and cloud](https://iowarp.ai/applications/genesis-portus/)
  A DOE Genesis Mission project at PNNL on performance-aware agentic workflows for the Genesis Mission Platform. The IOWarp team works on workflow motifs and performance models.
  Project began August 2026
- A5
  ### [CLIO on national research systems](https://iowarp.ai/applications/national-infrastructure/)
  Where CLIO Core has been built and run: ALCF Aurora, DeltaAI, and the Ares cluster.
  Built and run on national systems

Common questions

## Common questions.

**What is Jarvis?**

A deployment framework from the Gnosis Research Center that describes software stacks as pipelines over a resource graph. CLIO Core uses it for per-machine deployment.

Related

## Research and demos on this topic.

- [Research direction **Authority that travels with work** What can a delegated agent actually do?](https://iowarp.ai/research/directions/#authority)
- [Demo **CLIO on DeltaAI and Aurora** Planned for 2026](https://iowarp.ai/research/demos/#demo-clio-on-deltaai-and-aurora)
- [Demo **Materio for materials research** Planned for 2026](https://iowarp.ai/research/demos/#demo-materio-for-materials-research)
- [Demo **DOE Genesis: SPOTTER-AI and PORTUS** Planned for 2026](https://iowarp.ai/research/demos/#demo-doe-genesis-spotter-ai-and-portus)

## References

1. Cernuda et al., Jarvis: Towards a shared, user-friendly, and reproducible I/O infrastructure, PDSW 2024 work-in-progress session
2. [CLIO Core Jarvis deployment pipelines for Aurora, Delta, and other systems](https://github.com/iowarp/clio-core/tree/v2.2.1/jarvis_clio_core/pipelines)
3. [eScience 2025 poster PDF: EarthScope, LAMMPS, ParaView, and IOR agent workflows](http://cs.iit.edu/~scs/assets/files/islam2025aidriven_poster.pdf)
4. [Tang, Guo, Kougkas, Sun, Tallent. Characterizing dataflow for I/O-aware scheduling in HPC workflows. IPDPS 2026](https://doi.org/10.1109/IPDPS65963.2026.00076)
5. [WfCommons: open workflow instances and tools](https://wfcommons.org/)

## Other concepts

- [T1 Context management for AI agents](https://iowarp.ai/topics/context-management/)
- [T2 Scientific AI agents](https://iowarp.ai/topics/scientific-agents/)
- [T3 MCP servers for scientific computing](https://iowarp.ai/topics/mcp-for-science/)
- [T4 HPC I/O and storage hierarchies](https://iowarp.ai/topics/hpc-io/)
- [T5 Data movement for AI-infused workflows](https://iowarp.ai/topics/data-movement/)
- [T7 Evidence-based autonomous research](https://iowarp.ai/topics/evidence-based-research/)

Next step

## See this topic at work.

[Agents in the materials workflow](https://iowarp.ai/applications/materials-science/) [All concepts](https://iowarp.ai/docs/#concepts)
