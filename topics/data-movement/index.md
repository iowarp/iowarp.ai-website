---
title: "Data movement for AI-infused workflows | IOWarp"
description: "Data movement for AI-infused science: ingestion, tiered placement, GPU direct I/O, and agent-aware staging across memory, storage, and sites."
url: https://iowarp.ai/topics/data-movement/
---

> Data movement for AI-infused science: ingestion, tiered placement, GPU direct I/O, and agent-aware staging across memory, storage, and sites.

# Move the data before it is needed.

Scientific data rarely starts where it will be used. It moves from instruments and repositories to HPC storage, between memory and storage tiers, and into GPU memory for AI workloads. Each move costs time and loses context unless it is managed.

01 Ingestion with meaning attached 02 Placement and staging 03 Into the GPU 04 How IOWarp approaches it 05 Common questions

01

## Ingestion with meaning attached

The CLIO assimilation engine brings data in from local and parallel file systems and from Globus endpoints, described by OMNI files that record what the data is and how to read it.

02

## Placement and staging

The transfer engine places data across tiers using selectable placement policies. Research in the project goes further: AgentStage at eScience 2026 uses an agent’s own reasoning time as a window to move requested data into place.

03

## Into the GPU

Student work characterizes GPU-direct transfer through NVIDIA NIXL, and the transfer engine includes GPU-aware paths for accelerated workloads.

How IOWarp approaches it

## Where to go deeper.

01**CLIO Core**

Assimilation, transfer, and exploration engines.

Continue →

<https://iowarp.ai/platform/#core>

02**GPU data movement**

NIXL, CUDA integration, and KV-cache research.

Continue →

<https://iowarp.ai/applications/gpu-data-movement/>

03**Install and configure CLIO Core**

Published wheels, the conda channel, source builds, and system prerequisites.

Open ↗

<https://core.iowarp.ai/docs/installation.html>

Applications that use it

- A1
  ### [Agents in the materials workflow](https://iowarp.ai/applications/materials-science/)
  Design on HPC, additive manufacturing, X-ray tomography, and fatigue testing: the Utah team’s reference workflow, and the agent tools built for it.
  Active collaboration
- A5
  ### [CLIO on national research systems](https://iowarp.ai/applications/national-infrastructure/)
  Where CLIO Core has been built and run: ALCF Aurora, DeltaAI, and the Ares cluster.
  Built and run on national systems
- A6
  ### [GPU direct I/O and compression](https://iowarp.ai/applications/gpu-data-movement/)
  CUDA kernels that read and write IOWarp from the GPU, GPU payloads offloaded to host memory and NVMe, and compression on the device. A research thread built on NVIDIA technologies.
  Research thread across the stack

Common questions

## Common questions.

**Can CLIO pull data from Globus?**

Yes, through the assimilation engine’s Globus support in source builds. An end-to-end integration test passes on a public Globus collection.

Related

## Research and demos on this topic.

- [Research direction **The GPU as a storage tier** Can data reach GPU memory without a detour through the CPU?](https://iowarp.ai/research/directions/#gpu-tier)
- [Research direction **Staging data while agents think** Can reasoning time hide I/O time?](https://iowarp.ai/research/directions/#staging)
- [Demo **GPU payload offload** Planned for 2026](https://iowarp.ai/research/demos/#demo-gpu-payload-offload)
- [Demo **CLIO on DeltaAI and Aurora** Planned for 2026](https://iowarp.ai/research/demos/#demo-clio-on-deltaai-and-aurora)
- [Demo **Materio for materials research** Planned for 2026](https://iowarp.ai/research/demos/#demo-materio-for-materials-research)

## References

1. [Muradli, Ye, Logan, Kougkas, Sun. Insights into GPUDirect data transfer through NIXL benchmarking. IEEE eScience 2025 (poster and extended abstract)](https://doi.org/10.1109/eScience65000.2025.00075)
2. [IEEE eScience 2026 accepted papers, including Acropolis and AgentStage](https://www.escience-conference.org/2026/papers)
3. [CLIO Core Globus materials-science assimilation test](https://github.com/iowarp/clio-core/tree/v2.3.1/context-assimilation-engine/test/integration/globus_matsci)

## Other concepts

- [T1 Context management for AI agents](https://iowarp.ai/topics/context-management/)
- [T2 Scientific AI agents](https://iowarp.ai/topics/scientific-agents/)
- [T3 MCP servers for scientific computing](https://iowarp.ai/topics/mcp-for-science/)
- [T4 HPC I/O and storage hierarchies](https://iowarp.ai/topics/hpc-io/)
- [T6 Scientific workflows and reproducible deployment](https://iowarp.ai/topics/scientific-workflows/)
- [T7 Evidence-based autonomous research](https://iowarp.ai/topics/evidence-based-research/)

Next step

## See this topic at work.

[Agents in the materials workflow](https://iowarp.ai/applications/materials-science/) [All concepts](https://iowarp.ai/docs/#concepts)
