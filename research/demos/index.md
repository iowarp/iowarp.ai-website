---
title: "Demonstrations of the CLIO stack | IOWarp"
description: "IOWarp demonstrations: the 2026 series planned across the CLIO stack and the 2025 archive of agents on scientific data and HPC tools."
url: https://iowarp.ai/research/demos/
---

> IOWarp demonstrations: the 2026 series planned across the CLIO stack and the 2025 archive of agents on scientific data and HPC tools.

# See the stack at work.

For anyone who wants to see the software run: recordings of CLIO software on real scientific data and systems, made by the IOWarp team. The 2026 series follows the full stack, from CUDA kernels to DOE laboratory workflows; each entry states what its recording will show. The 2025 archive holds the first agent workflows on EarthScope, LAMMPS, ParaView, ADIOS2, and Slurm.

2026 series

Planned recordings across the stack

2025 archive

Recorded agent workflows

Research

[The questions behind the demos](https://iowarp.ai/research/directions/)

01 / Latest · 2026

## The 2026 series.

These entries are placeholders, not previews. Each video appears here when it is published.

1. 01 · To be recorded
  ### Zero to agent with CLIO Kit
  A clean machine to a working scientific agent: install CLIO Kit, connect an MCP client, and open a real HDF5 dataset.
  [CLIO Kit](https://iowarp.ai/platform/#kit)
2. 02 · To be recorded
  ### EarthScope through the National Data Platform, 2026
  The NDP workflow rebuilt on the current releases: catalog search, staging, profiling, and plotting of GNSS data.
  [Agents on the National Data Platform](https://iowarp.ai/applications/national-data-platform/) [CLIO Kit](https://iowarp.ai/platform/#kit) [CLIO Coder](https://iowarp.ai/platform/#coder)
3. 03 · To be recorded
  ### The HPC operator
  An agent submits and watches Slurm jobs, then reads the Darshan I/O profile to explain what the job did to the file system.
  [CLIO Kit](https://iowarp.ai/platform/#kit) [CLIO Agent](https://iowarp.ai/platform/#agent)
4. 04 · To be recorded
  ### GPU payload offload
  CUDA kernels in CLIO Core write GPU-resident data into IOWarp and stage it through host memory and NVMe.
  [GPU direct I/O and compression](https://iowarp.ai/applications/gpu-data-movement/) [CLIO Core GPU runtime](https://iowarp.ai/platform/#gpu-runtime) [CLIO Core](https://iowarp.ai/platform/#core)
5. 05 · To be recorded
  ### CLIO on DeltaAI and Aurora
  One Jarvis pipeline description deploys the same CLIO Core configuration on DeltaAI at NCSA and Aurora at Argonne.
  [CLIO on national research systems](https://iowarp.ai/applications/national-infrastructure/) [CLIO Core](https://iowarp.ai/platform/#core) [Jarvis](https://iowarp.ai/platform/#jarvis)
6. 06 · To be recorded
  ### Materio for materials research
  A materials question becomes a synthesis of the supplied literature, a map of the available lab, and a reviewed research plan.
  [Agents in the materials workflow](https://iowarp.ai/applications/materials-science/) [CLIO Coder](https://iowarp.ai/platform/#coder) [Materio and wtf-MS](https://iowarp.ai/platform/#materio)
7. 07 · To be recorded
  ### Memory across sessions
  CLIO Agent resumes a data investigation days later and recalls what it learned and where the data lives.
  [CLIO Agent](https://iowarp.ai/platform/#agent) [CLIO Core](https://iowarp.ai/platform/#core)
8. 08 · To be recorded
  ### DOE Genesis: SPOTTER-AI and PORTUS
  CLIO Agent investigating provenance with the SPOTTER-AI team at Argonne, and CLIO Coder fleets working with the PORTUS team at PNNL.
  [Provenance and integrity for AI-driven science](https://iowarp.ai/applications/genesis-spotter/) [Agentic workflows across HPC and cloud](https://iowarp.ai/applications/genesis-portus/) [CLIO Agent](https://iowarp.ai/platform/#agent) [CLIO Coder](https://iowarp.ai/platform/#coder)
9. 09 · To be recorded
  ### Fleet dispatch on a cluster
  CLIO Coder spreads bounded engineering tasks across workers on cluster nodes and returns reviewable run receipts.
  [Agentic workflows across HPC and cloud](https://iowarp.ai/applications/genesis-portus/) [CLIO Coder](https://iowarp.ai/platform/#coder)

02 / Archive · 2025

## The 2025 archive.

Recorded between September and November 2025. Select a preview to load the video player.

OCT 20, 2025 / TOOL ORCHESTRATION

### HPC workflow automation

An agent connects Slurm, ADIOS2, Jarvis, and a Gray–Scott simulation into one automated HPC workflow.

AI4HPC · CLIO Kit, Jarvis [Open on YouTube: HPC workflow automation ↗](https://www.youtube.com/watch?v=ogUpMwEU-SU)

OCT 20, 2025 / SCIENTIFIC DATA

### EarthScope seismograph analysis

An agent examines EarthScope seismograph data found through the National Data Platform.

AI4HPC · CLIO Kit [Open on YouTube: EarthScope seismograph analysis ↗](https://www.youtube.com/watch?v=9NUf76wnHhA)

OCT 20, 2025 / SIMULATION

### LAMMPS simulation data

An agent answers questions about data produced by a LAMMPS molecular dynamics simulation.

AI4HPC · CLIO Kit [Open on YouTube: LAMMPS simulation data ↗](https://www.youtube.com/watch?v=_Pd1SClE1Hc)

NOV 18, 2025 / VISUALIZATION

### ParaView as an agent tool

ParaView exposed through an MCP server so an agent can build and adjust a scientific visualization.

Shazzadul Islam · CLIO Kit [Open on YouTube: ParaView as an agent tool ↗](https://www.youtube.com/watch?v=IkcJnbFfpW0)

SEP 29, 2025 / AGENT WORKFLOW

### An IOWarp workflow end to end

An agent works through a scientific analysis with the IOWarp MCP servers, from data access to a finished plot.

Jaime Cernuda · CLIO Kit [Open on YouTube: An IOWarp workflow end to end ↗](https://www.youtube.com/watch?v=bjQ8uks4b5s)

SEP 29, 2025 / SCIENTIFIC FORMATS

### ADIOS2 data through MCP

An agent reads and inspects ADIOS2 simulation output through the IOWarp MCP servers.

Jaime Cernuda · CLIO Kit [Open on YouTube: ADIOS2 data through MCP ↗](https://www.youtube.com/watch?v=2x6yAcCPJFc)

SEP 29, 2025 / DEPLOYMENT

### Reproducible deployment

A workflow deployed reproducibly, with the agent’s activity streamed to a dashboard for inspection.

Jaime Cernuda · Jarvis, CLIO Kit [Open on YouTube: Reproducible deployment ↗](https://www.youtube.com/watch?v=AfS7xrYIRwc)

![Diagram of a six-stage materials science workflow: download a tomography dataset, reconstruct and segment the image stack, convert and store the volume, then visualize the result](https://iowarp.ai/images/demos/material_science.png)

2025 demo work / Materials workflow

### Follow the data.

The six-stage materials workflow that the demonstrations aim to cover: from a tomography dataset to reconstruction, segmentation, storage, and visualization. Every handoff between tools is part of the scientific work.

[The materials science story](https://iowarp.ai/applications/materials-science/)

What changed since

### From tools to a stack.

The 2025 recordings show agents calling individual MCP tools. The 2026 series shows the layers underneath and around them: GPU offload in CLIO Core, deployment on national systems, memory that persists across sessions, and agents working inside DOE laboratory projects.

[See the platform](https://iowarp.ai/platform/)

Try the system

## From a demo to your dataset.

[Install a component](https://iowarp.ai/docs/#install) [Read the applications](https://iowarp.ai/applications/)
