---
title: "HPC I/O and storage hierarchies | IOWarp"
description: "HPC I/O and storage hierarchies: multi-tiered buffering, memory and storage convergence, bottleneck detection, and how they shape the CLIO runtime."
url: https://iowarp.ai/topics/hpc-io/
---

> HPC I/O and storage hierarchies: multi-tiered buffering, memory and storage convergence, bottleneck detection, and how they shape the CLIO runtime.

# HPC I/O under scientific AI.

HPC I/O research studies how applications read and write data on supercomputers: through memory, burst buffers, node-local flash, parallel file systems, and archives. The deep memory and storage hierarchy is fast only if data is in the right tier at the right time.

01 Where IOWarp comes from 02 Measured results in the line of work 03 Why it matters for agents 04 How IOWarp approaches it 05 Common questions

01

## Where IOWarp comes from

IOWarp builds on Hermes, an earlier system for multi-tiered distributed I/O buffering, and on a line of Gnosis Research Center systems for labeled I/O, time-ordered logging, and data-task scheduling. The founding aim was stated directly: bending the I/O fabric for AI-infused scientific workflows.

02

## Measured results in the line of work

MegaMmap (SC 2024) manages DRAM and storage as tiered distributed shared memory and lowered peak DRAM use while keeping performance competitive. WisIO (ICS 2025) automates I/O bottleneck detection in HPC workflows. The papers state the workloads and figures.

03

## Why it matters for agents

Agents add a new kind of client to the storage stack: many small, latency-sensitive reads guided by reasoning. The CLIO transfer engine carries the tiering ideas into that setting.

How IOWarp approaches it

## Where to go deeper.

01**Storage and context**

How CLIO Core’s transfer engine places data across tiers.

Continue →

<https://iowarp.ai/platform/#layer-storage>

02**Where results live**

Papers, release notes, and project sites that carry the measurements with their conditions.

Continue →

<https://iowarp.ai/progress/#where-results-live>

03**Research archive**

Publications behind the systems lineage.

Continue →

<https://iowarp.ai/research/>

04**Compose storage tiers**

Configure local tiers and inspect how the Core filesystem uses its storage chain.

Open ↗

<https://core.iowarp.ai/tutorials/compose.html>

Applications that use it

- A4
  ### [Agentic workflows across HPC and cloud](https://iowarp.ai/applications/genesis-portus/)
  A DOE Genesis Mission project at PNNL on performance-aware agentic workflows for the Genesis Mission Platform. The IOWarp team works on workflow motifs and performance models.
  Project began August 2026
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

**Does IOWarp replace the parallel file system?**

No. It sits alongside existing storage and manages data flow across tiers during a workflow.

**Which I/O interfaces does CLIO Core intercept?**

In source builds, the transfer engine has adapters for POSIX, STDIO, HDF5 (VOL and VFD), and FUSE, an optional MPI-IO adapter, and GPU paths.

Related

## Research and demos on this topic.

- [Research direction **The GPU as a storage tier** Can data reach GPU memory without a detour through the CPU?](https://iowarp.ai/research/directions/#gpu-tier)
- [Demo **GPU payload offload** Planned for 2026](https://iowarp.ai/research/demos/#demo-gpu-payload-offload)
- [Demo **CLIO on DeltaAI and Aurora** Planned for 2026](https://iowarp.ai/research/demos/#demo-clio-on-deltaai-and-aurora)
- [Demo **DOE Genesis: SPOTTER-AI and PORTUS** Planned for 2026](https://iowarp.ai/research/demos/#demo-doe-genesis-spotter-ai-and-portus)

## References

1. [Logan et al., MegaMmap: Blurring the boundary between memory and storage for data-intensive workloads, SC 2024](https://doi.org/10.1109/SC41406.2024.00114)
2. [Yildirim et al., WisIO: Automated I/O bottleneck detection with multi-perspective views for HPC workflows, ICS 2025](https://doi.org/10.1145/3721145.3725742)
3. [Tang, Guo, Kougkas, Sun, Tallent. Characterizing dataflow for I/O-aware scheduling in HPC workflows. IPDPS 2026](https://doi.org/10.1109/IPDPS65963.2026.00076)

## Other concepts

- [T1 Context management for AI agents](https://iowarp.ai/topics/context-management/)
- [T2 Scientific AI agents](https://iowarp.ai/topics/scientific-agents/)
- [T3 MCP servers for scientific computing](https://iowarp.ai/topics/mcp-for-science/)
- [T5 Data movement for AI-infused workflows](https://iowarp.ai/topics/data-movement/)
- [T6 Scientific workflows and reproducible deployment](https://iowarp.ai/topics/scientific-workflows/)
- [T7 Evidence-based autonomous research](https://iowarp.ai/topics/evidence-based-research/)

Next step

## See this topic at work.

[Agentic workflows across HPC and cloud](https://iowarp.ai/applications/genesis-portus/) [All concepts](https://iowarp.ai/docs/#concepts)
