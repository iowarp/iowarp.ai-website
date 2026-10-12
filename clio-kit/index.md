---
title: "CLIO Kit: scientific tools and workflows | IOWarp"
description: "CLIO Kit brings scientific MCP servers, skills, agents, hooks, and workflow plugins to your AI client. Select the components your project needs."
url: https://iowarp.ai/clio-kit/
---

> CLIO Kit brings scientific MCP servers, skills, agents, hooks, and workflow plugins to your AI client. Select the components your project needs.

# Give agents real instruments.

For scientists and developers who want an AI agent to work with real scientific data and systems. CLIO Kit brings together MCP servers, skills, agent definitions, hooks, and workflow plugins. Choose individual components or a bundle for your task. The [released launcher](https://github.com/iowarp/clio-kit/releases/tag/v2.11.0) downloads selected components as needed, with isolated server dependencies installed on first launch.

Browse the servers [Components and workflows](https://toolkit.iowarp.ai/catalogue) [Source](https://github.com/iowarp/clio-kit)

**CLIO Kit** · command line MCP

1. Install the launcher
  ```sh
  uv tool install 'clio-kit>=2.11.0'
  ```
2. Inspect the catalog
  ```sh
  clio-kit mcp-servers
  ```
3. Start a server
  ```sh
  clio-kit mcp-server hdf5
  ```

The interface

MCP servers provide tools. Skills provide procedures. Workflow plugins bundle the components a task needs.

[How MCP works for science](https://iowarp.ai/topics/mcp-for-science/)

01 / The catalog

## Find your tool.

- 01 · Data
  ### [HDF5](https://toolkit.iowarp.ai/docs/mcps/hdf5)
  Inspect and work with scientific datasets and attributes.
- 02 · Data
  ### [Parquet](https://toolkit.iowarp.ai/docs/mcps/parquet)
  Read columnar data and inspect file structure.
- 03 · Data
  ### [Pandas](https://toolkit.iowarp.ai/docs/mcps/pandas)
  Load, filter, and analyze tabular data.
- 04 · Data
  ### [ADIOS](https://toolkit.iowarp.ai/docs/mcps/adios)
  Read data through ADIOS2 engines.
- 05 · HPC
  ### [Slurm](https://toolkit.iowarp.ai/docs/mcps/slurm)
  Submit and manage cluster jobs.
- 06 · HPC
  ### [Spack](https://toolkit.iowarp.ai/docs/mcps/spack)
  Discover, install, and locate scientific packages.
- 07 · HPC
  ### [JARVIS](https://toolkit.iowarp.ai/docs/mcps/jarvis)
  Build and manage scientific pipelines.
- 08 · HPC
  ### [Darshan](https://toolkit.iowarp.ai/docs/mcps/darshan)
  Inspect I/O performance traces.
- 09 · HPC
  ### [Lmod](https://toolkit.iowarp.ai/docs/mcps/lmod)
  Manage environment modules.
- 10 · HPC
  ### [Parallel Sort](https://toolkit.iowarp.ai/docs/mcps/parallel_sort)
  Sort, filter, and summarize large log files in parallel.
- 11 · Visual
  ### [ParaView](https://toolkit.iowarp.ai/docs/mcps/paraview)
  Visualize and render scientific data.
- 12 · Visual
  ### [Plot](https://toolkit.iowarp.ai/docs/mcps/plot)
  Turn tabular results into plots.
- 13 · Earth
  ### [Geo](https://toolkit.iowarp.ai/docs/mcps/geo)
  Inspect, validate, summarize, and map GeoJSON vector layers.
- 14 · Earth
  ### [Terrain](https://toolkit.iowarp.ai/docs/mcps/terrain)
  Analyze elevation models and point clouds.
- 15 · Earth
  ### [Seismology](https://toolkit.iowarp.ai/docs/mcps/seismology)
  Inspect SAC waveform files and archives, compute trace statistics, and analyze earthquake sequences.
- 16 · Discovery
  ### [ArXiv](https://toolkit.iowarp.ai/docs/mcps/arxiv)
  Find and retrieve research papers.
- 17 · Discovery
  ### [Scientific Catalog](https://toolkit.iowarp.ai/docs/mcps/scientific_catalog)
  Discover operator-owned datasets.
- 18 · Discovery
  ### [NDP](https://toolkit.iowarp.ai/docs/mcps/ndp)
  Search datasets across CKAN instances.
- 19 · Discovery
  ### [Web](https://toolkit.iowarp.ai/docs/mcps/web)
  Run search and durable document fetch tasks.
- 20 · Systems
  ### [ChronoLog](https://toolkit.iowarp.ai/docs/mcps/chronolog)
  Log and retrieve data through ChronoLog.
- 21 · Systems
  ### [Compression](https://toolkit.iowarp.ai/docs/mcps/compression)
  Compress and decompress files.
- 22 · Systems
  ### [Node Hardware](https://toolkit.iowarp.ai/docs/mcps/node_hardware)
  Inspect hardware on the local machine or a remote node.

02 / In practice

## Choose components. Install a workflow.

Project installs support Codex, Claude Code, OpenCode, Cursor, Antigravity, and VS Code. Scientific agents and Dataset Report hooks have adapters for Codex, Claude Code, and OpenCode. Other clients can explicitly select `--components-only` for skills and MCP configuration; see [component support](https://toolkit.iowarp.ai/docs/clients#component-support).

```sh
clio-kit plugin install clio-scientific-io --client codex --project /path/to/project
```

Installs the scientific I/O workflow’s skills and MCP configuration into the specified Codex project. Add `--dry-run` to preview changes. The [client setup guides](https://toolkit.iowarp.ai/docs/clients) explain each adapter; the [selective installation guide](https://toolkit.iowarp.ai/docs/installation) covers release downloads and native Claude plugins.

1. 01
  ### Choose
  Browse [MCPs, skills, agents, and hooks](https://toolkit.iowarp.ai/catalogue), or select a [workflow plugin](https://toolkit.iowarp.ai/docs/plugins) for scientific I/O, HPC operations, analysis, or research.
2. 02
  ### Install
  For one skill, use `clio-kit skill install dataset-explore --target.agents/skills` in a project whose client reads that directory. Configure its required MCP servers separately.
3. 03
  ### Verify
  Reload the client and inspect its skills and tools. Run `clio-kit doctor --server hdf5 --connect`, then try a tool call on known data. Scientific backends and cluster access have their own prerequisites.

Related

## Where CLIO Kit is at work.

- [Application **Agents in the materials workflow** Materials science](https://iowarp.ai/applications/materials-science/)
- [Application **Agents on the National Data Platform** Data infrastructure](https://iowarp.ai/applications/national-data-platform/)
- [Application **Provenance and integrity for AI-driven science** DOE Genesis · SPOTTER-AI](https://iowarp.ai/applications/genesis-spotter/)
- [Application **CLIO on national research systems** National infrastructure](https://iowarp.ai/applications/national-infrastructure/)
- [Research direction **Staging data while agents think** Can reasoning time hide I/O time?](https://iowarp.ai/research/directions/#staging)
- [Demo **Zero to agent with CLIO Kit** Planned for 2026](https://iowarp.ai/research/demos/#demo-zero-to-agent-with-clio-kit)
- [Demo **EarthScope through the National Data Platform, 2026** Planned for 2026](https://iowarp.ai/research/demos/#demo-earthscope-through-the-national-data-platform-2026)
- [Demo **The HPC operator** Planned for 2026](https://iowarp.ai/research/demos/#demo-the-hpc-operator)
- [Demo **HPC workflow automation** Recorded 2025](https://iowarp.ai/research/demos/#demo-hpc-workflow-automation)
- [Demo **EarthScope seismograph analysis** Recorded 2025](https://iowarp.ai/research/demos/#demo-earthscope-seismograph-analysis)
- [Demo **LAMMPS simulation data** Recorded 2025](https://iowarp.ai/research/demos/#demo-lammps-simulation-data)
- [Demo **ParaView as an agent tool** Recorded 2025](https://iowarp.ai/research/demos/#demo-paraview-as-an-agent-tool)
- [Demo **An IOWarp workflow end to end** Recorded 2025](https://iowarp.ai/research/demos/#demo-an-iowarp-workflow-end-to-end)
- [Demo **ADIOS2 data through MCP** Recorded 2025](https://iowarp.ai/research/demos/#demo-adios2-data-through-mcp)
- [Demo **Reproducible deployment** Recorded 2025](https://iowarp.ai/research/demos/#demo-reproducible-deployment)

Next step

## Make your workflow an instrument.

[Open the CLIO Kit guides](https://toolkit.iowarp.ai/docs/intro) [CLIO Kit on the platform](https://iowarp.ai/platform/#kit)
