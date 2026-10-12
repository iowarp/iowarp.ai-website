---
title: "CLIO documentation | IOWarp"
description: "CLIO Agent, Coder, Kit, and Core documentation sites, first commands, tested dependencies, platform requirements, and common questions."
url: https://iowarp.ai/docs/
---

> CLIO Agent, Coder, Kit, and Core documentation sites, first commands, tested dependencies, platform requirements, and common questions.

# Documentation lives with the code.

For developers and scientists installing a CLIO product. The Agent, Coder, Kit, and Core sites carry their product guides. This page points to the right place and gives the first command for each, with release-tag sources for compatibility.

01 Documentation sites 02 Get started 03 CLIO Core guides 04 Concepts 05 Common questions

01 / Documentation sites

## Four places, one platform.

CLIO Agent**clio.iowarp.ai**

Install the scientific data agent, connect a model, work with files and sessions, and add marketplace blueprints and MCP tools.

Open clio.iowarp.ai ↗

<https://clio.iowarp.ai/docs/>

CLIO Coder**coder.iowarp.ai**

Guides for the coding agent: installation, model connections, repository context, checks, worker fleets, run receipts, and context continuity.

Open coder.iowarp.ai ↗

<https://coder.iowarp.ai/docs.html>

CLIO Kit**toolkit.iowarp.ai**

Choose scientific MCP servers and skills, install workflow plugins into a supported client, and check component dependencies and client-specific limits.

Open toolkit.iowarp.ai ↗

<https://toolkit.iowarp.ai/docs/intro>

CLIO Core**core.iowarp.ai**

Install the context runtime, use its Python APIs, compose storage tiers and data operators, mount the filesystem, and explore the runtime dashboard.

Open core.iowarp.ai ↗

<https://core.iowarp.ai/docs/index.html>

02 / Get started

## Get started with one command.

Choose the product for your task, then follow its guide for platform requirements and model setup. These commands use the public release paths. The [current Kit release](https://github.com/iowarp/clio-kit/releases/tag/v2.11.0) adds selective components and workflow plugins; Agent’s installer keeps its own tested Kit pin.

- CLIO Agent
  ```sh
  curl -fsSL https://raw.githubusercontent.com/iowarp/clio-agent/v0.9.4.24/install/install.sh | bash
  ```
  [Guide for CLIO Agent](https://clio.iowarp.ai/docs/install/)
- CLIO Coder
  ```sh
  curl -fsSL https://coder.iowarp.ai/install.sh | sh
  ```
  [Guide for CLIO Coder](https://coder.iowarp.ai/docs.html)
- CLIO Kit
  ```sh
  uv tool install clio-kit
  ```
  [Guide for CLIO Kit](https://toolkit.iowarp.ai/docs/installation)
- CLIO Core
  ```sh
  pip install iowarp-core
  ```
  [Guide for CLIO Core](https://core.iowarp.ai/docs/installation.html)
- CLIO Relay
  ```sh
  uv tool install --python 3.12 --no-config clio-relay
  ```
  [README for CLIO Relay](https://github.com/iowarp/clio-relay#readme)
- CLIO Schemas
  ```sh
  pip install clio-schemas
  ```
  [README for CLIO Schemas](https://github.com/iowarp/clio-schemas#readme)

03 / CLIO Core guides

## The context runtime, in depth.

The Core portal covers installation, Python APIs, storage composition, and data operators. The [stable release notes](https://github.com/iowarp/clio-core/releases/tag/v2.3.1) and [tagged runtime configuration](https://github.com/iowarp/clio-core/blob/v2.3.1/context-runtime/config/clio_default.yaml) establish released behavior; check the [published files](https://pypi.org/project/iowarp-core/2.3.1/#files) for wheel compatibility. Agent retains its own tested Core dependency. The [platform page](https://iowarp.ai/platform/#core) explains the runtime’s role.

- 01
  ### [Install CLIO Core ↗](https://core.iowarp.ai/docs/installation.html)
  Published wheels, the conda channel, native packages, and source-build prerequisites. Check PyPI files for current wheel compatibility.
- 02
  ### [Components and modules ↗](https://github.com/iowarp/clio-core/blob/v2.3.1/README.md#components)
  Transport primitives, the modular runtime, and the assimilation, transfer, and exploration engines in the stable source.
- 03
  ### [Python API ↗](https://core.iowarp.ai/docs/python-api.html)
  Bundle, query, and retrieve context with clio_cee, or work with tags, blobs, and search through clio_cte_core_ext.
- 04
  ### [Runtime configuration ↗](https://core.iowarp.ai/tutorials/compose.html)
  Compose local storage tiers and the filesystem chain. The tagged configuration documents defaults for the stable runtime.

04 / Concepts

## Concepts in short.

Short explainers on context management for AI agents, scientific AI agents, MCP servers for science, HPC I/O, and agentic workflows. Each defines the topic, explains how IOWarp approaches it, and links to the papers, software, and applications that ground it.

T1**Context management for AI agents**

Context management is the work of deciding what an AI agent sees, when, and with what authority: which data, which tool results, which prior decisions, and which limits.

Read the explainer →

<https://iowarp.ai/topics/context-management/>

T2**Scientific AI agents**

A scientific agent is a language-model-driven program that carries out steps of a research workflow by calling tools: reading datasets, submitting jobs, running analyses, and producing figures.

Read the explainer →

<https://iowarp.ai/topics/scientific-agents/>

T3**MCP servers for scientific computing**

The Model Context Protocol is an open standard through which AI applications call external tools and read external resources.

Read the explainer →

<https://iowarp.ai/topics/mcp-for-science/>

T4**HPC I/O and storage hierarchies**

HPC I/O research studies how applications read and write data on supercomputers: through memory, burst buffers, node-local flash, parallel file systems, and archives.

Read the explainer →

<https://iowarp.ai/topics/hpc-io/>

T5**Data movement for AI-infused workflows**

Scientific data rarely starts where it will be used.

Read the explainer →

<https://iowarp.ai/topics/data-movement/>

T6**Scientific workflows and reproducible deployment**

A scientific workflow chains simulation, analysis, AI, and visualization steps across machines.

Read the explainer →

<https://iowarp.ai/topics/scientific-workflows/>

T7**Evidence-based autonomous research**

Autonomous research systems propose changes and test them.

Read the explainer →

<https://iowarp.ai/topics/evidence-based-research/>

05 / Common questions

## Common questions.

Questions that cross component boundaries. Version-specific answers live in each component’s documentation.

**What is the difference between IOWarp and CLIO?**

IOWarp is the team at the Gnosis Research Center that builds CLIO. CLIO, the Context Layer for I/O, is the open platform it builds: two agentic frameworks, CLIO Agent and CLIO Coder, the CLIO Kit tools they share, the CLIO Core context runtime, and the GPU, storage, application, and research components around them.

**Which component should I install first?**

Choose the task first. Install CLIO Agent to work with scientific data, or CLIO Coder to work on scientific software; they are different products for different audiences. Install CLIO Kit to give any MCP-compatible agent scientific tools, and CLIO Core for the context runtime and its APIs. Each installs on its own and has its own prerequisites.

**How do I install CLIO Core?**

Install the standalone runtime with pip install iowarp-core. Check the PyPI files for current CPython versions, operating systems, and architectures. GPU, MPI, and some format adapters need a source build. Linux wheels need libfuse3 to mount, Windows needs WinFsp, and macOS mounting requires a source build with macFUSE. Keep Agent’s tested Core dependency when installing Agent. [Published wheel compatibility on PyPI ↗](https://pypi.org/project/iowarp-core/2.3.1/#files) [Mount on macOS ↗](https://core.iowarp.ai/tutorials/fuse-macos.html)

**How do I install CLIO Agent on my system?**

Use the tagged Bash installer shown above on Linux or macOS. On Windows, run irm https://raw.githubusercontent.com/iowarp/clio-agent/v0.9.4.24/install/install.ps1 | iex in PowerShell. The installer sets up the backend, matching terminal UI, and clio launcher, and prepares the web UI when its bundle can be unpacked. Use Python 3.12 or Python 3.13 for the tested dependency set. Agent keeps its tested Core and Kit dependencies. [Stable Agent installer notes ↗](https://github.com/iowarp/clio-agent/blob/v0.9.4.24/install/README.md) [Agent installation and desktop downloads ↗](https://clio.iowarp.ai/docs/install/) [Connect a model ↗](https://clio.iowarp.ai/docs/connect-a-model/)

**How do I install CLIO Coder on my system?**

The shell installer supplies its own Node.js runtime on Linux and macOS. PowerShell and CMD installers are available for Windows, where native interactive use remains best effort. An npm install uses your own supported Node.js runtime. Connect a model that supports tool calling, then run clio-coder doctor to check the installation and connections. [Coder documentation and installation ↗](https://coder.iowarp.ai/docs.html)

**How do I install the scientific MCP servers?**

Install the standalone CLIO Kit launcher with uv tool install clio-kit. Run clio-kit mcp-servers to list its servers, then clio-kit mcp-server hdf5 to fetch and start the HDF5 component. Components download on demand, and server dependencies stay isolated and locked. Follow the client guide to register a server or install a workflow plugin. [Selective installation ↗](https://toolkit.iowarp.ai/docs/installation) [Client setup and component support ↗](https://toolkit.iowarp.ai/docs/clients#component-support)

**Should I upgrade the Core or Kit installed by CLIO Agent?**

Agent keeps Core in its tested compatible release family and pins Kit for its marketplace packs. Keep that combination when installing Agent. Standalone Core and Kit have separate release and upgrade paths; a newer standalone package does not establish Agent compatibility. [Agent’s tested dependency declarations ↗](https://github.com/iowarp/clio-agent/blob/v0.9.4.24/pyproject.toml) [Agent installer and its Kit pin ↗](https://github.com/iowarp/clio-agent/blob/v0.9.4.24/install/install.sh) [Standalone Kit installation ↗](https://toolkit.iowarp.ai/docs/installation)

**Which scientific formats are supported?**

It depends on the component. CLIO Kit has tools for formats such as HDF5, Parquet, ADIOS2, SAC, and geospatial data. CLIO Core has its own assimilation adapters, including HDF5 in source builds. Check the specific server or adapter before relying on a format in a workflow.

**Is there a Python API?**

Yes. CLIO Core ships clio_cee for bundling, querying, retrieving, and destroying contexts, and clio_cte_core_ext for tags, blobs, and search. Its Python guide explains runtime attachment and indexing requirements. [Core Python API ↗](https://core.iowarp.ai/docs/python-api.html)

**What can I add to CLIO Coder?**

Content plugins provide reusable instructions and procedures. Sandboxed extensions load after approval of their declared capabilities, and playbooks describe fleet contracts. A semantic context index is optional; background indexing is off by default, and scanned PDF recognition and raw video embedding are unsupported. The desktop app remains alpha and SSH workers remain experimental. [Current Coder documentation ↗](https://coder.iowarp.ai/docs.html) [Released behavior and limits ↗](https://github.com/iowarp/clio-coder/releases/tag/v0.6.2)

**Is every CLIO component available now?**

The current flagships, scientific context runtime, and supporting tools are open source. GPU and operating-system backends have build and hardware prerequisites. Archived BaM and GPU–NVMe bridge prototypes remain in older tagged source and are absent from the current Core release. [Current Core release ↗](https://github.com/iowarp/clio-core/releases/tag/v2.3.1) [Archived prototypes ↗](https://github.com/iowarp/clio-core/tree/v2.2.1/external/bam)

**Where should I report a problem or propose an integration?**

Open an issue in the repository of the component you used, with the version, environment, input format, expected and observed results, and a small reproducible example if you can share one. Zulip is open for discussion.

Next step

## Not sure where to start?

[Compare the flagships](https://iowarp.ai/platform/#flagships) [Talk to the team](https://iowarp.ai/community/#contact)

CLIO Agent works with scientific data and CLIO Coder works on scientific software. Both can use scientific tools from CLIO Kit.
