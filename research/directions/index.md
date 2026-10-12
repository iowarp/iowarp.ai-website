---
title: "Research directions | IOWarp"
description: "Open research questions behind the CLIO stack: GPU data paths, context lifecycles, agent memory, provenance, and evidence, with the newest results."
url: https://iowarp.ai/research/directions/
---

> Open research questions behind the CLIO stack: GPU data paths, context lifecycles, agent memory, provenance, and evidence, with the newest results.

# The questions behind the stack.

For researchers and collaborators. IOWarp is a research project as much as a software project. Each layer of the CLIO stack exists to test a question about how science should move, keep, and use context. These are the questions the team is working on now, where each is being worked on, and the newest results.

Questions

The GPU as a storage tier · Context with a lifecycle · Memory as a storage hierarchy · Staging data while agents think · Authority that travels with work · Provenance an agent can question · Evidence for agentic science

Archive

[Publications and posters](https://iowarp.ai/research/)

01 / Open questions

## The system is still a question.

1. 01
  Can data reach GPU memory without a detour through the CPU?
  ### The GPU as a storage tier
  GPU kernels that issue their own I/O, payloads that spill to host memory and NVMe, compression on the device, and prototypes that give GPUs direct NVMe queues. The question is how far the storage hierarchy can extend into the accelerator.
  [Worked on in: CLIO Core GPU runtime and direct GPU I/O research →](https://iowarp.ai/applications/gpu-data-movement/)
  Related [CLIO Core GPU runtime](https://iowarp.ai/platform/#gpu-runtime) [GPU compression](https://iowarp.ai/platform/#gpu-compression) [GPU direct I/O and compression](https://iowarp.ai/applications/gpu-data-movement/) [Data movement for AI-infused workflows](https://iowarp.ai/topics/data-movement/) [HPC I/O and storage hierarchies](https://iowarp.ai/topics/hpc-io/)
2. 02
  What should survive a turn, a handoff, or a project?
  ### Context with a lifecycle
  Working context, handoffs, and durable memory have different lifetimes. Agents need explicit staleness and promotion rules so old notes are never mistaken for current authority.
  [Worked on in: CLIO Coder context continuity ↗](https://coder.iowarp.ai/docs/guide/context-continuity.html)
  Related [CLIO Coder](https://iowarp.ai/platform/#coder) [Context management for AI agents](https://iowarp.ai/topics/context-management/)
3. 03
  Which facts belong hot, durable, or replayable?
  ### Memory as a storage hierarchy
  What an agent remembers has different access patterns and lifetimes. The question is how to place, retrieve, and retire it across scientific systems, including the model’s own KV cache.
  [Worked on in: CLIO Agent ARC memory and KV-cache research →](https://iowarp.ai/platform/#agent)
  Related [CLIO Agent](https://iowarp.ai/platform/#agent) [CLIO Core](https://iowarp.ai/platform/#core) [GPU direct I/O and compression](https://iowarp.ai/applications/gpu-data-movement/) [Context management for AI agents](https://iowarp.ai/topics/context-management/)
4. 04
  Can reasoning time hide I/O time?
  ### Staging data while agents think
  An agent spends time planning before it reads data. That window can be used to move the data it is likely to request into a faster tier.
  [Worked on in: AgentStage, IEEE eScience 2026 ↗](https://www.escience-conference.org/2026/papers)
  Related [Tiered block devices](https://iowarp.ai/platform/#tiers) [CLIO Kit](https://iowarp.ai/platform/#kit) [Data movement for AI-infused workflows](https://iowarp.ai/topics/data-movement/) [Scientific AI agents](https://iowarp.ai/topics/scientific-agents/)
5. 05
  What can a delegated agent actually do?
  ### Authority that travels with work
  Distributed agents need typed assignments, bounded read and write scopes, and checks that can be inspected after execution. More workers without those controls is not a systems result.
  [Worked on in: CLIO Coder fleet dispatch, with the PORTUS integration in progress →](https://iowarp.ai/applications/genesis-portus/)
  Related [CLIO Coder](https://iowarp.ai/platform/#coder) [CLIO Relay](https://iowarp.ai/platform/#relay) [Agentic workflows across HPC and cloud](https://iowarp.ai/applications/genesis-portus/) [Scientific workflows and reproducible deployment](https://iowarp.ai/topics/scientific-workflows/) [Scientific AI agents](https://iowarp.ai/topics/scientific-agents/)
6. 06
  When a result is wrong, can we find out why?
  ### Provenance an agent can question
  Provenance spans workflow events, artifact lineage, and signals from inside the model. Investigating agents need read-only access to all of it, and their own actions must be held to the same standard.
  [Worked on in: CLIO Agent provenance investigation, qualified against Flowcept and CMF for SPOTTER-AI →](https://iowarp.ai/applications/genesis-spotter/)
  Related [CLIO Agent](https://iowarp.ai/platform/#agent) [Agent marketplace](https://iowarp.ai/platform/#marketplace) [Provenance and integrity for AI-driven science](https://iowarp.ai/applications/genesis-spotter/) [Evidence-based autonomous research](https://iowarp.ai/topics/evidence-based-research/) [Scientific AI agents](https://iowarp.ai/topics/scientific-agents/)
7. 07
  What would prove an agent made progress?
  ### Evidence for agentic science
  Scientific workflows need baselines, holdouts, provenance, and run records. A persuasive narrative cannot substitute for measurements tied to their producer and conditions.
  [Worked on in: CLIO Researcher and CLIO Bench in the research tooling →](https://iowarp.ai/platform/#layer-research)
  Related [CLIO Researcher](https://iowarp.ai/platform/#researcher) [CLIO Bench](https://iowarp.ai/platform/#bench) [Agents in the materials workflow](https://iowarp.ai/applications/materials-science/) [Evidence-based autonomous research](https://iowarp.ai/topics/evidence-based-research/)

02 / New results

## Accepted this year.

Recent papers from the team and its collaborators that feed these questions. The [research archive](https://iowarp.ai/research/) has the full record.

- **Trigger, Render, Reason: Multimodal LLM agents for science-aware scientific simulation monitoring.** Xu, Cernuda, Gainaru, Klasky, Kougkas, Sun. [SC 2026 (accepted)](https://grc.iit.edu/publications/xu-2026-trigger-render-reason-multimodal-llm-agents-c360/).
- **AgentStage: Exploiting LLM thinking for data staging in scientific agents.** Yildirim, Sun, Kougkas. [IEEE eScience 2026](https://www.escience-conference.org/2026/papers).
- **Acropolis: A portable, AI-driven semantic search system for HPC.** Pawar, Logan, Cernuda, Sun, Kougkas. [IEEE eScience 2026](https://www.escience-conference.org/2026/papers).
- **Rich I/O-centric derived quantity operators for advanced in situ processing.** Multi-institution collaboration including Illinois Tech, Argonne, and Oak Ridge researchers. [IEEE eScience 2026](https://www.escience-conference.org/2026/papers).
- **InfiniteScienceGym: An unbounded, procedurally generated benchmark for scientific analysis.** Bentham, Srikumar (University of Utah). [COLM 2026](https://arxiv.org/abs/2604.13201).
- **PKAS: Predictive KVCache-aware scheduling for faster LLM and transformer inferences.** Ye, Maurya, Chitty-Venkata, Nicolae, Kougkas, Sun. [HPDC 2026](https://doi.org/10.1145/3806645.3807819).

Next step

## Where collaboration moves the work.

[Ways to collaborate](https://iowarp.ai/community/#collaborate) [Results and milestones](https://iowarp.ai/progress/)

These directions need scientific workloads with trusted baselines, time on national systems, and reviewers from outside the team. Research partners and facility staff can each shorten the path from prototype to evidence.
