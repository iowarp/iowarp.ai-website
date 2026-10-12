---
title: "IOWarp: an open stack for AI-driven science"
description: "The IOWarp team at the Gnosis Research Center builds CLIO, an open stack for AI-driven science: CLIO Agent, CLIO Coder, CLIO Kit, and CLIO Core."
url: https://iowarp.ai/
---

> The IOWarp team at the Gnosis Research Center builds CLIO, an open stack for AI-driven science: CLIO Agent, CLIO Coder, CLIO Kit, and CLIO Core.

# An open stack for AI-driven science.

IOWarp builds **CLIO**: open-source software that runs from CUDA kernels and the Linux I/O path, through storage and a context runtime, to scientific agents, applications, and research tools. In AI-driven science, **context is part of the system.**

Get started [See the platform](https://iowarp.ai/platform/)

TRY IT

## Install one piece. It works alone.

Start with the product closest to your work. Every route leads to its own documentation and source code.

[Where the documentation lives](https://iowarp.ai/docs/)

Give scientific data an agent, from a terminal, a desktop app, or a browser.

```sh
curl -fsSL https://raw.githubusercontent.com/iowarp/clio-agent/v0.9.4.24/install/install.sh | bash
```

[CLIO Agent install notes ↗](https://clio.iowarp.ai/docs/install/)

Connect a model to a repository you can inspect.

```sh
curl -fsSL https://coder.iowarp.ai/install.sh | sh
```

[CLIO Coder install notes ↗](https://coder.iowarp.ai/docs.html)

Choose scientific tools and workflow plugins for your client.

```sh
uv tool install clio-kit
```

[CLIO Kit install notes ↗](https://toolkit.iowarp.ai/docs/installation)

Install the context runtime and its Python API.

```sh
pip install iowarp-core
```

[CLIO Core install notes ↗](https://core.iowarp.ai/docs/installation.html)

[CONTEXT **The right data, with its meaning attached.**](https://iowarp.ai/platform/#principle-context)

[MEMORY **What an agent learns outlasts the session.**](https://iowarp.ai/platform/#principle-memory)

[SCALE **From a laptop to a national system.**](https://iowarp.ai/platform/#principle-scale)

IOWarp and the CLIO platform soft launch at SC26 in Chicago, November 15–20, 2026. [IOWarp at SC26 →](https://iowarp.ai/community/#sc26)

WHAT IS THIS?

## One stack, from GPU to agent.

IOWarp is an open-source project at the Gnosis Research Center. It builds CLIO, a software stack for AI-driven science.

An AI agent in science needs more than a model. It needs the right data with its meaning attached, memory that lasts beyond one session, and a way to run on anything from a laptop to a national system. CLIO covers each of those, from GPU kernels and storage up to agents and applications.

You do not need all of it. CLIO Agent, CLIO Coder, CLIO Kit, and CLIO Core each install on their own.

[See how the platform fits together](https://iowarp.ai/platform/)

1. 07 **Research tooling**
  Tools for writing, measuring, and testing research claims.
2. 06 **Applications**
  Science workflows and domain packages built on the stack.
3. 05 **Agents and tools**
    - [CLIO Agent](https://iowarp.ai/platform/#agent)
    - [CLIO Coder](https://iowarp.ai/platform/#coder)
    - [CLIO Kit](https://iowarp.ai/platform/#kit)
4. 04 **Context runtime**
    - [CLIO Core](https://iowarp.ai/platform/#core)
5. 03 **Storage systems**
  Tiered devices, I/O adapters, compression, and data connectors.
6. 02 **Operating system**
  The Linux I/O path, from asynchronous I/O to kernel modules.
7. 01 **Accelerators**
  GPU code that reaches the storage hierarchy directly.

THE SCIENCE

## Built with working scientists.

IOWarp works with scientific teams: materials scientists, the National Data Platform, and DOE Genesis Mission projects at Argonne and PNNL. CLIO Core runs on national research systems.

- [A1 **Agents in the materials workflow** Materials science](https://iowarp.ai/applications/materials-science/)
  Design on HPC, additive manufacturing, X-ray tomography, and fatigue testing: the Utah team’s reference workflow, and the agent tools built for it.
- [A2 **Agents on the National Data Platform** Data infrastructure](https://iowarp.ai/applications/national-data-platform/)
  MCP tools that let an agent search, stage, and analyze datasets federated through the National Data Platform, first shown on EarthScope data.
- [A3 **Provenance and integrity for AI-driven science** DOE Genesis · SPOTTER-AI](https://iowarp.ai/applications/genesis-spotter/)
  A DOE Genesis Mission project at Argonne National Laboratory that traces integrity attacks on scientific AI workflows to their source. CLIO Agent provides the investigating agents.
- [A4 **Agentic workflows across HPC and cloud** DOE Genesis · PORTUS](https://iowarp.ai/applications/genesis-portus/)
  A DOE Genesis Mission project at PNNL on performance-aware agentic workflows for the Genesis Mission Platform. The IOWarp team works on workflow motifs and performance models.
- [A5 **CLIO on national research systems** National infrastructure](https://iowarp.ai/applications/national-infrastructure/)
  Where CLIO Core has been built and run: ALCF Aurora, DeltaAI, and the Ares cluster.
- [A6 **GPU direct I/O and compression** Accelerated computing](https://iowarp.ai/applications/gpu-data-movement/)
  CUDA kernels that read and write IOWarp from the GPU, GPU payloads offloaded to host memory and NVMe, and compression on the device. A research thread built on NVIDIA technologies.

[All applications](https://iowarp.ai/applications/) [See the demos](https://iowarp.ai/research/demos/) [Releases and news](https://iowarp.ai/news/)

MEET US

## Meet the team at SC26.

**IOWarp at SC26** November 15–20, 2026 · McCormick Place, Chicago

IOWarp and the CLIO platform soft launch at SC26 in Chicago. The team presents work on simulation monitoring, GPU I/O, storage observability, compressed training data, and agent fleets through workshop presentations, research posters, a conference paper, and an HDF5 birds-of-a-feather session. The user group gathers around these events, and the Technical Advisory Board forms at the end of November, after SC26.

- Workshop**[GPUH5: A GPU-first I/O Library for Scientific Data](https://iowarp.ai/community/#sc26-gpuh5)**Monday, November 16, 2026, 10:50–11:10 am CST
- Workshop**[GDSight: Per-Operation Cross-Layer Attribution for GPUDirect Storage](https://iowarp.ai/community/#sc26-gdsight)**Monday, November 16, 2026, 11:30–11:50 am CST
- Workshop**[Trigger-Gated Multimodal LLM Agents for In-situ Scientific Simulation Monitoring](https://iowarp.ai/community/#sc26-trigger-gated)**Monday, November 16, 2026, 12:15–12:20 pm CST
- Poster**[Extending I/O Observability to Explainability for Targeted Optimization](https://iowarp.ai/community/#sc26-io-explainability)**Tuesday, November 17, 2026, 10:00 am–5:00 pm CST
- Poster**[GNNs Beyond HBM: Compressed, Bit-Exact Feature Streaming for Out-of-Core Training](https://iowarp.ai/community/#sc26-gnns-beyond-hbm)**Tuesday, November 17, 2026, 10:00 am–5:00 pm CST
- Poster**[StageOnce: Speculative Cross-Job Data Staging for LLM Agent Fleets](https://iowarp.ai/community/#sc26-stageonce)**Tuesday, November 17, 2026, 10:00 am–5:00 pm CST
- Poster**[ToolFuse: Provenance-Aware In-Flight Coalescing of Redundant Agent Tool Calls](https://iowarp.ai/community/#sc26-toolfuse)**Tuesday, November 17, 2026, 10:00 am–5:00 pm CST
- Paper**[Trigger, Render, Reason: Multimodal LLM Agents for Science-Aware Scientific Simulation Monitoring](https://iowarp.ai/community/#sc26-trigger-render-reason)**Wednesday, November 18, 2026, 4:30–5:00 pm CST
- Birds of a feather**[Trustworthy Data at Scale: HDF5 in the Age of AI-Driven Science](https://iowarp.ai/community/#sc26-hdf5-bof)**Thursday, November 19, 2026, 12:15–1:15 pm CST

[IOWarp at SC26](https://iowarp.ai/community/#sc26) [The user group](https://iowarp.ai/community/#user-group) [The advisory board](https://iowarp.ai/community/#advisory-board) [Join Zulip](https://iowarp.zulipchat.com/)

Open source

## Read the source. Run the stack.

[Get started](https://iowarp.ai/docs/#install) [Source on GitHub](https://github.com/iowarp)

CLIO is built and led by the IOWarp team at the Gnosis Research Center, in the open, with the scientists, engineers, and facilities that put it to work.
