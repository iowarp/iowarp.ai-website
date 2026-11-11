---
title: "IOWarp: an open stack for AI-driven science"
description: "IOWarp builds CLIO, the open-source stack that puts AI agents to work on scientific data. The full stack will launch at SC26 in Chicago."
url: https://iowarp.ai/
---

> IOWarp builds CLIO, the open-source stack that puts AI agents to work on scientific data. The full stack will launch at SC26 in Chicago.

# AI for science you can check.

IOWarp builds **CLIO**, open-source software that puts AI agents to work on your scientific data and leaves a record your people can check. It runs on the systems you already operate, from a workstation to a national facility. In AI-driven science, **context is part of the system.**

Explore CLIO [Find us at SC26](https://iowarp.ai/community/#sc26)

THE CLIO SUITE

## Start anywhere. Each piece stands alone.

Choose the product closest to your work. CLIO Agent and CLIO Coder serve people working on scientific data and scientific software; CLIO Kit supplies the scientific tools both share, and CLIO Core runs the context hierarchy underneath.

[Compare on the platform](https://iowarp.ai/platform/#flagships) [All documentation](https://iowarp.ai/docs/)

Flagship Scientific data workspace

### [CLIO Agent](https://clio.iowarp.ai/)

For scientists, lab teams, and facility data managers.

Work with files, live streams, visualizations, shared web pages, and LaTeX papers in the desktop app or a browser, on local, cloud, or lab models.

```sh
curl -fsSL https://clio.iowarp.ai/install.sh | bash
```

[Open clio.iowarp.ai](https://clio.iowarp.ai/) [Desktop & install guide for CLIO Agent](https://clio.iowarp.ai/docs/install/) [In the stack for CLIO Agent](https://iowarp.ai/platform/#agent)

Flagship Meta-harness for scientific software

### [CLIO Coder](https://coder.iowarp.ai/)

For developers, computational scientists, and research software engineers.

Bring every model you have behind shared project guidance, inspectable checks, measured research campaigns, and a blind model arena.

```sh
curl -fsSL https://coder.iowarp.ai/install.sh | sh
```

[Open coder.iowarp.ai](https://coder.iowarp.ai/) [Documentation for CLIO Coder](https://coder.iowarp.ai/docs.html) [In the stack for CLIO Coder](https://iowarp.ai/platform/#coder)

Flagship Scientific tools and workflows

### [CLIO Kit](https://toolkit.iowarp.ai/)

For any MCP client: CLIO Agent, CLIO Coder, Claude Code, Codex, Cursor, and VS Code.

Select scientific MCP servers, skills, and workflow plugins for HDF5, Parquet, ADIOS2, Slurm, ParaView, the National Data Platform, and more.

```sh
uv tool install clio-kit
```

[Open toolkit.iowarp.ai](https://toolkit.iowarp.ai/) [Server catalog for CLIO Kit](https://iowarp.ai/clio-kit/) [Install guide for CLIO Kit](https://toolkit.iowarp.ai/docs/installation)

Infrastructure Tiered context runtime

### [CLIO Core](https://core.iowarp.ai/)

For HPC developers, facilities, and pipelines spanning memory and storage tiers.

Assimilate scientific data with its metadata, place it across GPU memory, DRAM, NVMe, and parallel storage, and query it from Python or C++.

```sh
pip install iowarp-core
```

[Open core.iowarp.ai](https://core.iowarp.ai/) [Install guide for CLIO Core](https://core.iowarp.ai/docs/installation.html) [In the stack for CLIO Core](https://iowarp.ai/platform/#core)

**FIG S.1** · HOW THE CLIO PRODUCTS CONNECT PEOPLE · AGENTS · TOOLS · RUNTIME · DATA

CLIO Agent serves scientific data and papers; CLIO Coder serves scientific software. Both use the models you choose and call tools in CLIO Kit, while CLIO Core stores durable memory and moves context across memory and storage tiers.

[CONTEXT **The right data, with its meaning attached.**](https://iowarp.ai/platform/#principle-context)

[MEMORY **What an agent learns outlasts the session.**](https://iowarp.ai/platform/#principle-memory)

[SCALE **From a laptop to a national system.**](https://iowarp.ai/platform/#principle-scale)

IOWarp will launch the full CLIO stack at SC26 in Chicago, November 15–20, 2026. [IOWarp at SC26 →](https://iowarp.ai/community/#sc26)

WHAT IS THIS?

## The whole stack, from GPU to agent.

IOWarp is the research and engineering team at the Gnosis Research Center, Illinois Tech, that builds CLIO. CLIO, the Context Layer for I/O, is an open-source software stack that connects AI agents to scientific data and the systems that hold it.

It matters because scientific data is only useful with its meaning attached. Point an agent at an HDF5 file or a Slurm queue and it needs the right data, memory that outlasts the session, and a path from a laptop to a national system. CLIO supplies each of those, so an organization can bring AI into its science and hold every change to its own checks.

Adoption is incremental. CLIO Agent, CLIO Coder, CLIO Kit, and CLIO Core each install on their own.

[See how the platform fits together](https://iowarp.ai/platform/)

1. 07 **Research tooling**
  From sources and results to a paper someone can check.
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

ACROSS DISCIPLINES

## One agentic framework. Ready for your science.

CLIO began in materials science, expanded to mechanical engineering simulations when neighboring groups saw it run, and now reaches analytical chemistry, federated earth-science catalogs, and DOE Genesis Mission workflows at Argonne and PNNL. Each discipline keeps the same CLIO backbone while swapping in the tools, domain skills, and checks its workflow demands.

**FIG W.1** · Where CLIO fits in a research group’s workflow CLOSED-LOOP SCIENTIFIC WORKFLOW

CLIO handles the reading, data plumbing, code verification, and study records around an experiment; the scientists and their instruments keep the scientific judgment.

**DOMAIN PROGRESSION** · How one discipline unlocks the next SELECT A FIELD TO INSPECT THE PATTERN

01 · Where CLIO started

### Materials science

Additive manufacturing, X-ray computed tomography, segmentation, and next-experiment planning across instruments and clusters.

THE LAB’S WORKFLOW

Printed specimens move from design to tomography scans and fatigue testing, where process history and volumes have to stay linked.

SWAPPED DOMAIN LAYER · KIT & PLUGINS

wtf-MS and Materio study-planning plugins, HDF5 and Parquet tools, ParaView rendering, and Globus data assimilation.

CONSTANT CLIO BACKBONE

CLIO Agent keeps study questions and observations tied to tool calls; CLIO Core holds the shared part record across stages.

[Read the materials story](https://iowarp.ai/applications/materials-science/)

02 · Adopted for simulation

### Mechanical engineering

Structural and topology-optimization campaigns where engineers saw the materials agents and adapted them to finite-element models.

THE LAB’S WORKFLOW

Engineers configure Abaqus and Tosca input decks, sweep parameters on cluster queues, inspect stress fields, and compare simulation runs.

SWAPPED DOMAIN LAYER · KIT & PLUGINS

Abaqus model-interpretation skills, Slurm and Lmod cluster servers, ParaView field inspection, and numerical check gates.

CONSTANT CLIO BACKBONE

CLIO Coder verifies code and configuration edits against declared checks; CLIO Agent records parameter choices and figures.

[Explore simulation tools in CLIO Kit](https://iowarp.ai/clio-kit/)

03 · Adopted at the bench

### Chemistry & bench labs

Experimental labs working from bench instruments, assay tables, and small-data machine learning without needing a supercomputer.

THE LAB’S WORKFLOW

Measurements stay at the bench while students and researchers organize instrument exports, train and validate predictive models, and preserve continuity when cohorts rotate.

SWAPPED DOMAIN LAYER · KIT & PLUGINS

Pandas and Parquet profiling, scripted matplotlib figures, marimo notebooks, and method-validation checks on held-out samples.

CONSTANT CLIO BACKBONE

CLIO Agent keeps computational steps as auditable as a validated lab method, and CLIO Coder reruns model pipelines from pinned inputs.

[Try CLIO Agent on your workstation](https://clio.iowarp.ai/)

04 · Scaled to facilities

### Earth & DOE facilities

Federated geoscience catalogs, simulation monitoring, workflow provenance security, and cross-facility HPC and cloud orchestration.

THE LAB’S WORKFLOW

Agents discover EarthScope stations through the National Data Platform, trace workflow integrity in SPOTTER-AI, and adapt multi-site runs in PORTUS.

SWAPPED DOMAIN LAYER · KIT & PLUGINS

NDP, Geo, and Seismology tools, the SPOTTER provenance investigator and watcher, and PORTUS surrogate performance models.

CONSTANT CLIO BACKBONE

The same MCP tool contracts, bounded agent permissions, sealed run receipts, and tiered CLIO Core placement underneath.

[See SPOTTER-AI and PORTUS](https://iowarp.ai/applications/genesis-spotter/)

05 · Bring your domain

### Your lab’s workflow

Any scientific group whose day crosses literature, messy data files, analysis scripts, predictive models, and manuscripts.

THE LAB’S WORKFLOW

Keep physical instruments and scientific judgment with your people, and hand the repetitive reading, data plumbing, code verification, and record-keeping to CLIO.

SWAPPED DOMAIN LAYER · KIT & PLUGINS

Pick existing servers from CLIO Kit or add a focused MCP server, a plain-Markdown domain skill, and your project’s own validation checks.

CONSTANT CLIO BACKBONE

CLIO Agent, CLIO Coder, CLIO Kit, and CLIO Core run on the models and machines your organization already approves.

[Bring a workflow to the team](mailto:partnerships@iowarp.ai?subject=%5BIOWarp-website%5D%20Collaboration%3A%20Adapting%20CLIO%20to%20our%20scientific%20workflow)

IN THE FIELD

### Project stories and collaborations.

Select a collaboration to preview its workflow and inspect how CLIO operates alongside working scientists and facilities.

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

[How CLIO adapts & all stories](https://iowarp.ai/applications/) [See the demos](https://iowarp.ai/research/demos/) [Releases and news](https://iowarp.ai/news/)

THE LAUNCH

## The full stack will launch at SC26.

**IOWarp at SC26** November 15–20, 2026 · McCormick Place, Chicago

[SC26 floor guide](https://iowarp.ai/community/#sc26) [Add to calendar (.ics)](https://iowarp.ai/sc26.ics)

IOWarp will launch the full CLIO stack at SC26 in Chicago. The team will present work on simulation monitoring, GPU I/O, storage observability, compressed training data, and agent fleets through workshop presentations, research posters, a conference paper, and an HDF5 birds-of-a-feather session with The HDF Group. The user group will gather around these events, and the Technical Advisory Board will form at the end of November.

### MON · NOV 16 · PDSW’26 Workshop

Room W179b

- **Workshop** · 10:50–11:10 am CST**[GPUH5: A GPU-first I/O Library for Scientific Data](https://iowarp.ai/community/#sc26-gpuh5)**
- **Workshop** · 11:30–11:50 am CST**[GDSight: Per-Operation Cross-Layer Attribution for GPUDirect Storage](https://iowarp.ai/community/#sc26-gdsight)**
- **Workshop** · 12:15–12:20 pm CST**[Trigger-Gated Multimodal LLM Agents for In-situ Scientific Simulation Monitoring](https://iowarp.ai/community/#sc26-trigger-gated)**

### TUE · NOV 17 · Research Posters · Poster Blitz

Skyline Ballroom North Pre-Function

- **Poster** · 10:00 am–5:00 pm CST**[Extending I/O Observability to Explainability for Targeted Optimization](https://iowarp.ai/community/#sc26-io-explainability)**
- **Poster** · 10:00 am–5:00 pm CST**[GNNs Beyond HBM: Compressed, Bit-Exact Feature Streaming for Out-of-Core Training](https://iowarp.ai/community/#sc26-gnns-beyond-hbm)**
- **Poster** · 10:00 am–5:00 pm CST**[StageOnce: Speculative Cross-Job Data Staging for LLM Agent Fleets](https://iowarp.ai/community/#sc26-stageonce)**
- **Poster** · 10:00 am–5:00 pm CST**[ToolFuse: Provenance-Aware In-Flight Coalescing of Redundant Agent Tool Calls](https://iowarp.ai/community/#sc26-toolfuse)**

### WED · NOV 18 · Papers in Conversation

Room W181abc

- **Paper** · 4:30–5:00 pm CST**[Trigger, Render, Reason: Multimodal LLM Agents for Science-Aware Scientific Simulation Monitoring](https://iowarp.ai/community/#sc26-trigger-render-reason)**

### THU · NOV 19 · Birds of a Feather

Room W185d

- **Birds of a feather** · 12:15–1:15 pm CST**[Trustworthy Data at Scale: HDF5 in the Age of AI-Driven Science](https://iowarp.ai/community/#sc26-hdf5-bof)**

[All SC26 details](https://iowarp.ai/community/#sc26) [The user group](https://iowarp.ai/community/#user-group) [The advisory board](https://iowarp.ai/community/#advisory-board) [Join Zulip](https://iowarp.zulipchat.com/)

Open source

## Read the source. Run the stack.

[Get started](https://iowarp.ai/docs/#install) [Source on GitHub](https://github.com/iowarp)

The IOWarp team at the Gnosis Research Center builds CLIO in the open, alongside the scientific teams and facilities that put it to work.
