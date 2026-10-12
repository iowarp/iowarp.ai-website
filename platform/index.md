---
title: "The CLIO platform | IOWarp"
description: "The CLIO platform: CLIO Agent and CLIO Coder, the CLIO Kit tools they share, and the CLIO Core runtime, from GPU kernels to scientific agents."
url: https://iowarp.ai/platform/
---

> The CLIO platform: CLIO Agent and CLIO Coder, the CLIO Kit tools they share, and the CLIO Core runtime, from GPU kernels to scientific agents.

# From GPU kernels to scientific agents.

For developers, researchers, and facility staff deciding where to start. The IOWarp team builds CLIO as one platform: two agentic frameworks on top, the tools they share, and a context runtime underneath. Each piece installs on its own and is built to work with the rest.

Built by

The IOWarp team, [Gnosis Research Center](https://grc.iit.edu/research/projects/iowarp/)

Software

Open source under BSD-3-Clause, Apache-2.0, and MIT licenses

Source

[github.com/iowarp](https://github.com/iowarp)

01 / Principles

## Context, memory, and scale.

Context

### The right data, with its meaning attached.

For decades, scientific I/O research asked how to move bytes faster. AI-driven work asks a harder question: which data, with which provenance, tools, system state, and permissions, does the next step need? Context has a location, a size, a cost, and a lifetime, so IOWarp treats it as a system resource: assimilated with its meaning, placed near the computation, exposed through well-defined tools, and retired when it is no longer needed.

Carried by CLIO Core CLIO Kit CLIO Coder CLIO Agent

Memory

### What an agent learns outlasts the session.

An agent that forgets everything between sessions repeats work and loses the trail. IOWarp keeps memory in the system rather than in a prompt: it persists across sessions, it can be inspected, and it is tied to the evidence that produced it, so people can check what an agent knows and why.

Carried by CLIO Agent CLIO Coder CLIO Core

Scale

### From a laptop to a national system.

The same software has to work on one machine and on a facility. Workers take sub-tasks in parallel, fleets run across nodes, tools reach schedulers and storage, and the runtime spans GPU memory, NVMe, parallel file systems, and object stores. Each piece installs on its own, so a team adds scale one component at a time.

Carried by CLIO Coder CLIO Core CLIO Agent CLIO Kit

**EVIDENCE CLOSES THE LOOP** An agent’s step is only useful to science if someone can inspect it later. CLIO records what was given, what was done, and what was measured, and leaves conclusions to people who can check them.

02 / The flagships

## Two agents, one toolkit.

CLIO Agent and CLIO Coder are different products for different audiences and different jobs. Choose the one that matches your work. Both can use scientific tools from CLIO Kit. CLIO Agent uses CLIO Core for its context runtime.

Flagship Scientific data agent Beta

### CLIO Agent

For scientists, data managers, and facility teams who want an agent to inspect, analyze, and visualize scientific data.

An autonomous agent for scientific data management. It works directly with workspace tools, and installable packs add an orchestrator, domain experts for data, analysis, and visualization, and short-lived workers for parallel sub-tasks. It runs from a terminal, a desktop app, or a browser.

Context

Packs route each task to the domain expert with the matching capability, and data is read through typed tools.

Memory

ARC, a local-first memory layer that every tier reads and writes, keeps what the agent learned across sessions. It stores its records in CLIO Core by default, with a local file backend as the alternative.

Scale

Packs can spawn short-lived workers for parallel sub-tasks, and the agent runs on local models, cloud providers, or an institutional inference gateway.

**What else it does**

- Packs with an orchestrator, domain experts, and capability-based routing
- A tool gateway that mounts CLIO Kit servers such as HDF5 and Parquet through agent packs
- Per-turn invocation records kept as a corpus for future optimizer research
- A runtime doctor that checks the model, gateway, and file-policy health
- Works with LM Studio, Ollama, OpenAI, Anthropic, Codex, Claude Code, OpenRouter, subscription sign-in, and the Argonne ALCF inference gateway
- Stable installers for Linux, macOS, and Windows, with tested Core and Kit dependencies

```sh
curl -fsSL https://raw.githubusercontent.com/iowarp/clio-agent/v0.9.4.24/install/install.sh | bash
```

[CLIO Agent site](https://clio.iowarp.ai/) [Documentation for CLIO Agent](https://clio.iowarp.ai/docs/) [Source for CLIO Agent](https://github.com/iowarp/clio-agent)

Flagship Coding agent Beta

### CLIO Coder

For developers and research software engineers working on simulation kernels, numerical libraries, data pipelines, and mixed-language builds.

A coding agent that connects your own models to repository tools, project context, verification, and worker delegation, and leaves work you can inspect. Understand a codebase, investigate a failing check, implement a change, or coordinate a workflow across local workers, with experimental support for SSH workers.

Context

A project handbook, layered rules, and a code map give the model bounded orientation. The checks you declare decide whether a change holds.

Memory

The session ledger stays whole while working-set selection keeps the model inside its budget. Branch, resume, or hand off a session, and review the memory the agent proposes against recorded evidence.

Scale

Workers and fleets run across worktrees, and experimentally across SSH nodes. Compiled fleet plans are reviewed before anything runs.

**What else it does**

- Declared tests, builds, numerical comparisons, and performance checks, tied to repository quality policies
- Tool activity, diffs, traces, cost accounting, and sealed run records you can review
- MCP servers, including CLIO Kit Slurm workflows, and a headless mode plus an Agent Client Protocol server for editors
- Skills, agents, prompts, and content plugins, with sandboxed extensions that load after capability approval
- Playbooks for reviewable fleet contracts
- An optional semantic context index for code, approved memory, and evidence. Background indexing is off by default; scanned PDF recognition and raw video embedding are unsupported
- A desktop app (alpha) with a setup wizard
- Installs with its own Node.js, or with npm on a supported Node.js release. Native Windows is best effort
- Your models: local servers such as Ollama, LM Studio, llama.cpp, and vLLM, cloud APIs, and the Argonne ALCF inference service

```sh
curl -fsSL https://coder.iowarp.ai/install.sh | sh
```

[CLIO Coder site](https://coder.iowarp.ai/) [Documentation for CLIO Coder](https://coder.iowarp.ai/docs.html) [Source for CLIO Coder](https://github.com/iowarp/clio-coder)

Flagship Scientific tools and workflows

### CLIO Kit

For anyone who wants an agent, CLIO Agent and CLIO Coder included, to work with real scientific data and systems.

A meta-marketplace for scientific computing: Model Context Protocol servers, workflow skills, agents, hooks, and plugins. Choose a component for a task or install a workflow that brings its tools and guidance together. CLIO Agent’s marketplace packs and CLIO Coder use its scientific servers.

Context

Typed operations with declared inputs and visible outputs give an agent the data and system state a step needs.

Scale

A small launcher downloads only the selected components, with isolated, locked server dependencies. Slurm, Spack, and Darshan tools reach real machines.

**What else it does**

- Servers for data formats, HPC operations, visualization, earth science, discovery, and systems
- Select individual servers and skills, or install workflow plugins into a supported client’s project
- Project installers for Codex, Claude Code, OpenCode, Cursor, Antigravity, and VS Code, with client-specific limits for agents and hooks
- Verified component downloads, separately versioned server contracts, and community marketplace discovery

```sh
uv tool install clio-kit
```

[CLIO Kit hub](https://iowarp.ai/clio-kit/) [CLIO Kit guides](https://toolkit.iowarp.ai/docs/intro) [Source for CLIO Kit](https://github.com/iowarp/clio-kit)

Infrastructure Context runtime

### CLIO Core

For facility teams, HPC developers, and researchers who need data kept with its meaning across every tier.

The runtime underneath. Assimilation brings data in with its metadata, transfer places it across memory and storage tiers, and exploration lets people and agents bundle, query, and retrieve it.

Context

Data is assimilated with its metadata and stays addressable by name wherever it is placed.

Memory

Tiers reach from GPU memory through NVMe and parallel file systems to object stores, so context outlives any one process.

Scale

GPU runtimes, and ports to ALCF Aurora and DeltaAI, take it from a laptop to national systems.

**What else it does**

- Python and C++ APIs, with an MCP path for agents
- Wheels on PyPI and a conda channel
- Optional GPU, MPI, and format adapters in source builds, and a FUSE mount in Linux and Windows wheels or macOS source builds

```sh
pip install iowarp-core
```

[CLIO Core site](https://core.iowarp.ai/) [Documentation for CLIO Core](https://core.iowarp.ai/docs/index.html) [Source for CLIO Core](https://github.com/iowarp/clio-core) [Deployment record for CLIO Core](https://grc.iit.edu/research/projects/iowarp/) [Releases for CLIO Core](https://github.com/iowarp/clio-core/releases)

03 / The layers

## Seven layers, one system.

At the bottom, **accelerator and operating-system work** lets GPU kernels reach storage: CUDA, ROCm, and SYCL code in CLIO Core, compression on the GPU, and direct I/O adapters. Archived research prototypes explored GPU-owned NVMe queues.

**Storage systems** span GPU memory, DRAM, NVMe, parallel file systems, object stores, and remote collections, with adapters that let existing applications use them unchanged.

**CLIO Core** is the context runtime. It assimilates data with its metadata, places it across tiers, and lets people and agents query and retrieve it.

**Agents and tools** use that context. CLIO Agent and CLIO Coder are the two agentic frameworks. CLIO Kit supplies scientific MCP tools and reusable workflow components, and CLIO Relay and GACT connect CLIO Agent to clusters and to people.

**Applications** such as Materio and the materials, geoscience, and DOE Genesis workflows test the whole platform, and **research tooling** for writing, benchmarking, and measured experimentation keeps the results checkable.

1. 07 **Research tooling** Tools for writing, measuring, and testing research claims.
    - [CLIO Author](https://iowarp.ai/platform/#author)
    - [CLIO Researcher](https://iowarp.ai/platform/#researcher)
    - [CLIO Bench](https://iowarp.ai/platform/#bench)
2. 06 **Applications** Science workflows and domain packages built on the stack.
    - [Materio and wtf-MS](https://iowarp.ai/platform/#materio)
    - [Science workflows](https://iowarp.ai/platform/#workflows)
3. 05 **Agents and tools** Agent runtimes, scientific tools, and the contracts between them.
    - [CLIO Agent](https://iowarp.ai/platform/#agent)
    - [CLIO Coder](https://iowarp.ai/platform/#coder)
    - [CLIO Kit](https://iowarp.ai/platform/#kit)
    - [CLIO Relay](https://iowarp.ai/platform/#relay)
    - [GACT and Agent Workspace](https://iowarp.ai/platform/#gact)
    - [Agent marketplace](https://iowarp.ai/platform/#marketplace)
    - [CLIO Web Search](https://iowarp.ai/platform/#web-search)
    - [CLIO Schemas](https://iowarp.ai/platform/#schemas)
4. 04 **Context runtime** CLIO Core: data assimilated, placed, and explored with its meaning attached.
    - [CLIO Core](https://iowarp.ai/platform/#core)
    - [Jarvis](https://iowarp.ai/platform/#jarvis)
5. 03 **Storage systems** Tiered devices, I/O adapters, compression, and data connectors.
    - [Tiered block devices](https://iowarp.ai/platform/#tiers)
    - [I/O adapters and connectors](https://iowarp.ai/platform/#adapters)
6. 02 **Operating system** The Linux I/O path, from asynchronous I/O to kernel modules.
    - [GPU–NVMe bridge](https://iowarp.ai/platform/#gnb)
    - [Linux I/O backends](https://iowarp.ai/platform/#os-io)
7. 01 **Accelerators** GPU code that reaches the storage hierarchy directly.
    - [CLIO Core GPU runtime](https://iowarp.ai/platform/#gpu-runtime)
    - [GPU compression](https://iowarp.ai/platform/#gpu-compression)
    - [Direct GPU I/O research](https://iowarp.ai/platform/#gpu-direct)

The flagships are outlined in cyan. Select a component to jump to its entry.

04 / Everything else

## The rest of the platform.

These components support the flagships and the science, each with its own repository and release.

LAYER 01

### Accelerators

GPU code that reaches the storage hierarchy directly.

Scientific AI computes on GPUs. If data can only reach them through the host, every read and write waits on the CPU.

#### CLIO Core GPU runtime

GPU kernels read and write IOWarp.

CUDA, ROCm, and SYCL builds of CLIO Core let GPU kernels submit work to the runtime and keep GPU-resident data backed by transfer-engine storage, spilling payloads to host memory and NVMe and bringing them back on demand.

**What is inside**

- GPU-to-runtime task queues on NVIDIA, AMD, and Intel GPUs
- GPU-resident vectors with a GPU and host-memory page cache
- An HDF5-style dataset interface callable from GPU kernels
- GPU memory and pinned host memory as storage tiers

```sh
cmake --preset=cuda-release
```

Used in [CLIO on national research systems](https://iowarp.ai/applications/national-infrastructure/) [GPU direct I/O and compression](https://iowarp.ai/applications/gpu-data-movement/)

[Source code for CLIO Core GPU runtime](https://github.com/iowarp/clio-core)

#### GPU compression

Compress on the device, before data moves.

nvCOMP, cuSZ, cuSZp, ndzip, and ZFP for SYCL plug into the CLIO compression layer beside CPU codecs, with learned predictors that choose a codec for the data at hand instead of guessing.

Used in [GPU direct I/O and compression](https://iowarp.ai/applications/gpu-data-movement/)

[Source code for GPU compression](https://github.com/iowarp/clio-core) [NVIDIA nvCOMP](https://developer.nvidia.com/nvcomp)

#### Direct GPU I/O research

Take the CPU out of the GPU’s data path.

The cuFile adapter and NIXL transport support are source-build options, alongside published characterization of GPUDirect transfers through NIXL. Earlier BaM-style GPU page-cache work remains in archived prototype sources and is absent from the current release.

Gnosis Research Center, Illinois Tech

Used in [GPU direct I/O and compression](https://iowarp.ai/applications/gpu-data-movement/)

[NVIDIA NIXL](https://github.com/ai-dynamo/nixl) [Archived BaM prototype](https://github.com/iowarp/clio-core/tree/v2.2.1/external/bam)

LAYER 02

### Operating system

The Linux I/O path, from asynchronous I/O to kernel modules.

The operating system decides how fast any byte can move. IOWarp uses what the kernel offers and prototypes what it does not.

#### GPU–NVMe bridge

An archived Linux kernel-module prototype for GPU I/O.

The bridge prototype created NVMe queue pairs alongside the stock Linux driver so a GPU or a user-space process could submit storage commands without the CPU in the data path. It remains in an earlier release’s source archive and is absent from the current release.

Used in [GPU direct I/O and compression](https://iowarp.ai/applications/gpu-data-movement/)

[Guide to GPU–NVMe bridge](https://github.com/iowarp/clio-core/blob/v2.2.1/external/bam/gnb/DESIGN.md) [Source code for GPU–NVMe bridge](https://github.com/iowarp/clio-core) [Archived bridge design](https://github.com/iowarp/clio-core/blob/v2.2.1/external/bam/gnb/DESIGN.md)

#### Linux I/O backends

Asynchronous I/O and user-space file systems.

io_uring, libaio, and POSIX AIO backends drive direct file I/O under the block-device layer, and a FUSE adapter mounts IOWarp as a file system on Linux and Windows, with the Linux adapter tested with xfstests. The layer descends from LabStor (SC 2022), a platform for building customized I/O stacks in user space, which evolved into the CLIO runtime.

Used in [GPU direct I/O and compression](https://iowarp.ai/applications/gpu-data-movement/)

[Source code for Linux I/O backends](https://github.com/iowarp/clio-core)

LAYER 03

### Storage systems

Tiered devices, I/O adapters, compression, and data connectors.

Science data lives in memory, on NVMe, on parallel file systems, in object stores, and at remote facilities. Storage has to span all of them.

#### Tiered block devices

One hierarchy from GPU memory to object storage.

RAM, file and NVMe, GPU memory, and pinned host-memory devices, cloud object stores, and a Reed–Solomon erasure-coded array for resilience. The transfer engine places data across them by policy.

**What is inside**

- Compression with zstd, LZ4, Blosc2, SZ3, ZFP, and more in source builds
- Transports over shared memory, ZeroMQ, Thallium, and NIXL

Used in [GPU direct I/O and compression](https://iowarp.ai/applications/gpu-data-movement/)

[Source code for Tiered block devices](https://github.com/iowarp/clio-core)

#### I/O adapters and connectors

Meet applications and data where they are.

In source builds, POSIX, STDIO, and HDF5 VOL and VFD adapters, with an optional MPI-IO adapter, let existing applications use IOWarp without code changes. The assimilation engine brings data in from local file systems, S3, Globus, and Google Cloud, described by OMNI files.

Used in [Agents in the materials workflow](https://iowarp.ai/applications/materials-science/) [CLIO on national research systems](https://iowarp.ai/applications/national-infrastructure/)

[Source code for I/O adapters and connectors](https://github.com/iowarp/clio-core) [HDF5](https://www.hdfgroup.org/solutions/hdf5/) [Globus](https://www.globus.org/)

LAYER 04

### Context runtime

CLIO Core: data assimilated, placed, and explored with its meaning attached.

This is where bytes become context: data kept together with its metadata and location, and served to whatever needs it next.

#### Jarvis

Reproducible deployment on real machines.

Pipeline descriptions record the scheduler, modules, network, and storage choices of each system. Public CLIO Core recipes cover local machines, the Ares cluster, Delta, and ALCF Aurora. The Jarvis package catalog covers simulations such as LAMMPS, WarpX, and OpenFOAM, storage services, and measurement tools such as IOR and Darshan.

Used in [CLIO on national research systems](https://iowarp.ai/applications/national-infrastructure/)

[Source code for Jarvis](https://github.com/grc-iit/jarvis-cd)

LAYER 05

### Agents and tools

Agent runtimes, scientific tools, and the contracts between them.

Agents are new clients of scientific systems. They need real instruments to operate, memory that lasts, and limits that can be inspected.

MIT license

#### CLIO Relay

Send work to a cluster and follow it home.

Submit work to a remote machine, follow it while it runs, and collect logs, artifacts, and provenance, from a CLI, an HTTP API, or MCP tools. Part of the federation layer for CLIO Agent, and usable on its own.

**What is inside**

```sh
uv tool install --python 3.12 --no-config clio-relay
```

[Source code for CLIO Relay](https://github.com/iowarp/clio-relay)

MIT license

#### GACT and Agent Workspace

One contract, any agent, one workspace.

GACT is an open wire contract for agent front ends. Agent Workspace, a React and Tauri application, renders any agent that speaks it; CLIO Agent is the reference implementation.

[Source code for GACT and Agent Workspace](https://github.com/iowarp/gact-tui)

#### Agent marketplace

Installable agent packs for real tasks.

Packs that give CLIO Agent a ready team for a job: cluster operations, data semantics, deep research, EarthScope analysis, and provenance investigation for the DOE SPOTTER-AI project.

Used in [Agents on the National Data Platform](https://iowarp.ai/applications/national-data-platform/) [Provenance and integrity for AI-driven science](https://iowarp.ai/applications/genesis-spotter/)

[Source code for Agent marketplace](https://github.com/iowarp/clio-agent-marketplace)

MIT license

#### CLIO Web Search

Self-hosted search and document understanding.

Web search, document conversion, and scholarly metadata extraction for agents in one container, built on SearXNG, Docling, and GROBID, so every claim can point to its source.

[Source code for CLIO Web Search](https://github.com/iowarp/clio-web-search)

#### CLIO Schemas

Shared record shapes across the stack.

Canonical definitions of artifacts, provenance records, and messages shared by CLIO Agent, Relay, and Agent Workspace, published as Python models and JSON Schema.

**What is inside**

```sh
pip install clio-schemas
```

[Source code for CLIO Schemas](https://github.com/iowarp/clio-schemas)

LAYER 06

### Applications

Science workflows and domain packages built on the stack.

Every layer below is tested against real science: materials, geoscience, and DOE laboratory workflows.

MIT license

#### Materio and wtf-MS

A materials research workflow for agents.

Turns a materials question into a synthesis of the supplied literature, a map of the laboratory actually available, and an assumption-checked research plan with a reviewed paper handoff. wtf-MS runs in Claude Code; Materio is its port for CLIO Coder.

Used in [Agents in the materials workflow](https://iowarp.ai/applications/materials-science/)

[Source code for Materio and wtf-MS](https://github.com/iowarp/wtf-ms)

#### Science workflows

Where the stack meets the science.

Materials characterization, EarthScope data through the National Data Platform, NeuroH5 through its HDF5 connector, and DOE Genesis Mission projects with Argonne and PNNL.

[Science workflows page](https://iowarp.ai/applications/) [National Data Platform](https://nationaldataplatform.org/) [DOE Genesis Mission](https://genesis.energy.gov/)

LAYER 07

### Research tooling

Tools for writing, measuring, and testing research claims.

Scientific results must be checkable. These tools keep the evidence attached from experiment to paper.

More research tools are on the way, together with a CLIO SDK that packages tested combinations of the components on this page.

BSD-3-Clause license

#### CLIO Author

From source material to a reviewable paper.

A multi-agent harness for the paper lifecycle: ingest sources, check citations, plan, draft, review, and export, driven from MCP clients or CLIO Coder.

Apache-2.0 license

#### CLIO Researcher

Let hypotheses compete against measurements.

A local-first research loop for I/O systems: it proposes a change to code or configuration, measures it against a baseline, checks confidence and a holdout, and stages only supported improvements for review.

MIT license

#### CLIO Bench

Make every run inspectable.

A run recorder and live dashboard for benchmarks and model comparisons. Producers send measurements; Bench stores, streams, and compares them without issuing verdicts of its own.

05 / What exists today

## What runs today, what comes next.

- 01
  ### Released and installable
  CLIO Agent in beta, CLIO Coder, CLIO Kit with its scientific tools and workflow plugins, and CLIO Core, plus CLIO Relay and the supporting tools around them, all open source and released on their own schedules.
- 02
  ### [Running on national systems](https://iowarp.ai/applications/national-infrastructure/)
  CLIO Core was ported to ALCF Aurora, where it runs benchmark pipelines, and it builds and runs on DeltaAI and the Ares cluster.
- 03
  ### [In the science](https://iowarp.ai/applications/)
  Materials science, agents on the National Data Platform, NeuroH5 through its HDF5 connector, and, since August 2026, the DOE Genesis Mission projects SPOTTER-AI and PORTUS.
- 04
  ### [Published](https://iowarp.ai/research/)
  Papers and posters at IEEE eScience, ICS, and HPDC, with new 2026 work accepted at eScience and SC on agent data staging, semantic search for HPC, and agents that monitor simulations.
- 05
  ### [Coming next](https://iowarp.ai/progress/)
  The soft launch at SC26 in Chicago, November 15–20, 2026, the Technical Advisory Board at the end of November, end-to-end runs of the materials workflow, and a stable platform release after that.

[Results and milestones, with sources and conditions →](https://iowarp.ai/progress/)

Next step

## See the platform in the science.

[Read the applications](https://iowarp.ai/applications/) [Source on GitHub](https://github.com/iowarp)
