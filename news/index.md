---
title: "IOWarp news | IOWarp"
description: "IOWarp builds CLIO, the open stack for AI-driven science. News with sources: the SC26 launch, DOE Genesis Mission projects, releases, and papers."
url: https://iowarp.ai/news/
---

> IOWarp builds CLIO, the open stack for AI-driven science. News with sources: the SC26 launch, DOE Genesis Mission projects, releases, and papers.

# What IOWarp is shipping.

IOWarp is the team at the Gnosis Research Center that builds CLIO, the open-source stack connecting AI agents to scientific data and systems. It matters because organizations running scientific computing need AI they can check. IOWarp will launch the full stack at SC26 in Chicago, and every entry here links to its original source.

Covers

Selected entries, 2025–2026

Order

Newest first

Live feeds

Release notes for each product

Subscribe

[RSS feed of news and releases](https://iowarp.ai/rss.xml) · [Publications](https://iowarp.ai/research/rss.xml)

Results

[Results and milestones](https://iowarp.ai/progress/)

01 / The ledger

## News, newest first

1. 01 15–20 NOV 2026
  SC26
  ### IOWarp launches the full CLIO stack at SC26 in Chicago
  IOWarp will launch the full CLIO stack at SC26 in Chicago. The team will present work on simulation monitoring, GPU I/O, storage observability, compressed training data, and agent fleets through workshop presentations, research posters, a conference paper, and an HDF5 birds-of-a-feather session with The HDF Group. Workshop presentations will take place on November 16, research posters on November 17, Trigger, Render, Reason on November 18, and the HDF5 birds-of-a-feather session on November 19. The community page lists every title, time, room, and program entry.
  [SC26 conference site](https://sc26.supercomputing.org/) [IOWarp at SC26](https://iowarp.ai/community/#sc26)
2. 02 11 NOV 2026
  RELEASE RECORD
  ### CLIO Agent ships a redesigned workbench, tool scripts, live streams, and a signed macOS app
  The pre-SC26 release lets an agent run Python scripts against its own tools without filling the conversation, follow live data streams in self-updating dashboards, share a browser tab, take anchored comments on figures and PDFs, build LaTeX papers against venue checks, and quarantine a session on a SPOTTER danger finding. Companion updates to GACT, CLIO Kit, and CLIO Core ship alongside it, and clio.iowarp.ai now serves the one-line desktop and service installers.
  [CLIO Agent release notes](https://github.com/iowarp/clio-agent/releases/tag/v0.9.6.1) [CLIO Agent on the platform](https://iowarp.ai/platform/#agent)
3. 03 9 NOV 2026
  RELEASE RECORD
  ### CLIO Coder adds verified research campaigns and a blind model arena
  clio-coder research climbs a project metric on a budget and keeps a change only when repeated measurements show a real gain and every correctness check passes. clio-coder arena runs one prompt on several models side by side and hides which is which until you vote. The release also reads HDF5, NetCDF, and Parquet, reruns computations from pinned inputs against a stated tolerance, and keeps a claims ledger for each project.
  [CLIO Coder release notes](https://github.com/iowarp/clio-coder/releases/tag/v0.7.0) [CLIO Coder on the platform](https://iowarp.ai/platform/#coder)
4. 04 8 NOV 2026
  RELEASE RECORD
  ### CLIO Kit sharpens its tools on planted scientific datasets
  The team ran the scientific servers through CLIO Coder on planted datasets and fixed what the runs exposed. The ADIOS, HDF5, pandas, Parquet, and Slurm servers gained per-step statistics, grouped aggregates, outlier reports, and the scheduler’s own reason for a job’s state.
  [CLIO Kit release notes](https://github.com/iowarp/clio-kit/releases/tag/v2.12.0) [Scientific tools and workflows](https://iowarp.ai/clio-kit/)
5. 05 31 OCT 2026
  RELEASE RECORD
  ### CLIO Coder seals its run records
  Every telemetry record names the acting agent and every journal is hash-chained. A sealed run can be verified on another machine or shared as a redacted archive.
  [CLIO Coder release notes](https://github.com/iowarp/clio-coder/releases/tag/v0.6.6) [CLIO Coder on the platform](https://iowarp.ai/platform/#coder)
6. 06 29 OCT 2026
  RELEASE RECORD
  ### CLIO Agent links studies to recorded work
  Study questions, experiments, observations, and conclusions now link to recorded calls, with live measurements and data export. Desktop and Web become the supported ways to run CLIO Agent. It pins its own tested pairing of CLIO Kit and CLIO Core, separate from their standalone releases.
  [CLIO Agent release notes](https://github.com/iowarp/clio-agent/releases/tag/v0.9.5.1) [CLIO Agent on the platform](https://iowarp.ai/platform/#agent)
7. 07 28 OCT 2026
  RELEASE RECORD
  ### The agent marketplace is rebuilt around per-agent plugins
  Each agent now ships a plugin that says whom it serves and what it does, and programs, formats, and data sources become separate plugins. CLIO Data inspects and converts HDF5, ADIOS, and Parquet files and verifies each conversion by reading it back. The SPOTTER plugin lives at plugins/spotter.
  [Marketplace release notes](https://github.com/iowarp/clio-agent-marketplace/releases/tag/v0.7.0) [The SPOTTER-AI story](https://iowarp.ai/applications/genesis-spotter/)
8. 08 16 OCT 2026
  RELEASE RECORD
  ### CLIO Core recovers from a full storage tier
  Python callers can inspect storage capacity and add a file target while the runtime stays active, so a managed store can recover from a full tier and keep its existing data.
  [CLIO Core release notes](https://github.com/iowarp/clio-core/releases/tag/v2.3.2) [CLIO Core guides](https://iowarp.ai/docs/#core-guides)
9. 09 9 OCT 2026
  RELEASE RECORD
  ### CLIO Coder releases approved extensions and playbooks
  The stable coding agent separates content plugins from sandboxed extensions that load after capability approval. Playbooks describe fleet contracts, and an optional semantic context index searches code, approved memory, and evidence. Background indexing is off by default.
  [CLIO Coder release notes](https://github.com/iowarp/clio-coder/releases/tag/v0.6.2) [CLIO Coder on the platform](https://iowarp.ai/platform/#coder)
10. 10 9 OCT 2026
  RELEASE RECORD
  ### CLIO Core fixes wheel startup and adds a documentation site
  Published wheels now include the indexer required by the default filesystem chain, fixing the earlier mount and runtime-start failures. The Core documentation site covers installation, Python APIs, storage composition, data operators, and the runtime dashboard. CLIO Agent keeps its own tested dependencies.
  [CLIO Core release notes](https://github.com/iowarp/clio-core/releases/tag/v2.3.1) [CLIO Core guides](https://iowarp.ai/docs/#core-guides)
11. 11 8 OCT 2026
  RELEASE RECORD
  ### CLIO Kit adds selective components and workflow plugins
  The published Kit release brings scientific MCP servers, skills, agents, hooks, and workflow plugins into a meta-marketplace. Its small launcher downloads selected components, keeps server dependencies isolated and locked, and installs supported workflows into client projects. The release is available on GitHub and PyPI, with its server contracts published to the MCP Registry.
  [CLIO Kit release record](https://github.com/iowarp/clio-kit/releases/tag/v2.11.0) [Scientific tools and workflows](https://iowarp.ai/clio-kit/)
12. 12 27 SEP 2026
  RELEASE RECORD
  ### CLIO Coder documents context continuity
  The CLIO Coder guides include a context continuity guide that separates working context, handoffs, and durable memory. The latest release, published to npm as @iowarp/clio-coder, keeps it current.
  [CLIO Coder releases](https://github.com/iowarp/clio-coder/releases) [CLIO Coder on the platform](https://iowarp.ai/platform/#coder)
13. 13 22 SEP 2026
  RELEASE RECORD
  ### wtf-MS reaches a stable release
  The University of Utah’s materials research-planning workflow reached its first stable release. Its CLIO Coder port, Materio, shipped earlier in September.
  [wtf-MS repository](https://github.com/iowarp/wtf-ms) [The materials science story](https://iowarp.ai/applications/materials-science/)
14. 14 AUG 2026
  COLLABORATION
  ### IOWarp joins two DOE Genesis Mission projects
  In August 2026 the IOWarp team joined two DOE Genesis Mission projects: SPOTTER-AI at Argonne and PORTUS at PNNL. CLIO Agent supplies the investigating agents for SPOTTER-AI, and the IOWarp team works on workflow motifs and performance models in PORTUS.
  [DOE Genesis Mission](https://genesis.energy.gov/) [The SPOTTER-AI story](https://iowarp.ai/applications/genesis-spotter/)
15. 15 AUG 2026
  RELEASE RECORD
  ### A coordinated CLIO release wave
  CLIO Core, CLIO Kit, CLIO Agent, CLIO Coder, and CLIO Relay all shipped between mid and late August, including the Spotter approval mode in CLIO Agent. Each repository’s release notes carry the details.
  [The repositories](https://github.com/iowarp) [The CLIO platform](https://iowarp.ai/platform/)
16. 16 2026
  PUBLICATIONS
  ### Agents that watch simulations, at SC 2026
  Trigger, Render, Reason, accepted at SC 2026 and scheduled for presentation in Chicago on November 18, pairs science-aware triggers with multimodal model confirmation to stop spending compute on invalid simulation runs.
  [Publication record](https://grc.iit.edu/publications/xu-2026-trigger-render-reason-multimodal-llm-agents-c360/) [Research directions](https://iowarp.ai/research/directions/)
17. 17 2026
  PUBLICATIONS
  ### New IOWarp papers at IEEE eScience 2026
  AgentStage uses an agent’s reasoning time to stage data; Acropolis brings AI-driven semantic search to HPC storage; a multi-institution paper defines I/O-centric derived quantity operators for in situ processing.
  [eScience 2026 program](https://www.escience-conference.org/2026/papers) [Research directions](https://iowarp.ai/research/directions/)
18. 18 27 MAY 2026
  CORE MILESTONE
  ### CLIO Core takes the CLIO name
  A major CLIO Core release renamed the runtime and its engines under the CLIO name, including the Context Transfer Engine and the Context Assimilation Engine.
  [CLIO Core releases](https://github.com/iowarp/clio-core/releases) [CLIO Core on the platform](https://iowarp.ai/platform/#core)
19. 19 APR 2026
  NATIONAL SYSTEMS
  ### CLIO Core on ALCF Aurora
  The Gnosis project record reports that the team ported CLIO Core to Aurora at the INCITE GPU hackathon and ran scientific workloads there. NERSC lists the event as April 28–30, 2026.
  [Gnosis project record](https://grc.iit.edu/research/projects/iowarp/) [CLIO on national research systems](https://iowarp.ai/applications/national-infrastructure/)
20. 20 28 JUL 2025
  COMMUNITY
  ### IOWarp beta presented in Denver
  The team presented the integrated IOWarp beta to fellow research cyberinfrastructure teams in Denver.
  [Poster on figshare](https://doi.org/10.6084/m9.figshare.29647613.v1) [Results and milestones](https://iowarp.ai/progress/)

02 / Live sources

## Follow the releases.

[Scientific data agent **CLIO Agent releases** Open the release notes ↗](https://github.com/iowarp/clio-agent/releases) [Coding agent **CLIO Coder releases** Open the release notes ↗](https://github.com/iowarp/clio-coder/releases) [Scientific tools **CLIO Kit releases** Open the release notes ↗](https://github.com/iowarp/clio-kit/releases) [Context runtime **CLIO Core releases** Open the release notes ↗](https://github.com/iowarp/clio-core/releases)

Next step

## Meet the team at SC26.

[IOWarp at SC26](https://iowarp.ai/community/#sc26) [The CLIO platform](https://iowarp.ai/platform/)
