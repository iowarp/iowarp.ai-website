---
title: "About IOWarp | IOWarp"
description: "The systems research CLIO grew from, the collaborators the IOWarp team works with, and the team behind the stack."
url: https://iowarp.ai/about/
---

> The systems research CLIO grew from, the collaborators the IOWarp team works with, and the team behind the stack.

# Built by a research community.

IOWarp turns years of systems research into CLIO, an open stack for AI-driven science. This page traces the ideas the stack grew from, the collaborators the IOWarp team works with, and the team itself.

Ideas

Systems lineage

Work with

Collaborators

Team

Team and support

01 / Systems lineage

## One question, asked from many angles.

The systems behind CLIO developed primitives for placement, runtime, intent, order, and task scheduling over years of work at the Gnosis Research Center. Agents made those primitives newly urgent. LabStor’s runtime evolved directly into CLIO Core, and Hermes’s shared-memory library became its transport primitives; the others contributed ideas.

IOWarp builds on Hermes, an earlier system for buffering data across memory and storage tiers. The project set out to bend the I/O fabric for advancing AI-infused scientific workflows. It framed the unit of exchange as Content, data plus a self-description that any workflow stage can read. As AI agents became real clients of scientific systems, that idea widened into context.

1. 01**Hermes**Placement
  Policy-driven buffering across memory and storage tiers. The system IOWarp builds on.
  <https://github.com/HDFGroup/hermes>
2. 02**LabStor**Runtime
  Customized I/O stacks built in user space. Its runtime evolved into the CLIO Core runtime.
  <https://github.com/grc-iit/labstor>
3. 03**LABIOS**Intent
  A label tells the data system what an operation is for.
  <https://github.com/grc-iit/labios>
4. 04**ChronoLog**Order
  A shared log records activity in time for provenance and replay.
  <https://grc.iit.edu/research/projects/chronolog/>
5. 05**DTIO**Task
  Data movement and transformation become schedulable work.
  <https://grc.iit.edu/research/projects/dtio/>
6. 06**CLIO**Context
  The earlier primitives meet a new client: the scientific agent, from the GPU to the paper.
  <https://iowarp.ai/platform/>

02 / Collaborators

## Who the team works with.

- 01
  ### [Argonne National Laboratory](https://iowarp.ai/applications/genesis-spotter/)
  Home of SPOTTER-AI, a DOE Genesis Mission project at Argonne National Laboratory; Aurora at the Argonne Leadership Computing Facility; co-authored KV-cache research. [Official site of Argonne National Laboratory ↗](https://www.anl.gov/) [ALCF ↗](https://www.alcf.anl.gov/)
  DOE Genesis · facility
- 02
  ### [Pacific Northwest National Laboratory](https://iowarp.ai/applications/genesis-portus/)
  Home of PORTUS, a DOE Genesis Mission project the IOWarp team joined in August 2026; co-authored research on dataflow for I/O-aware scheduling. [Official site of Pacific Northwest National Laboratory ↗](https://www.pnnl.gov/)
  DOE Genesis
- 03
  ### [National Data Platform](https://iowarp.ai/applications/national-data-platform/)
  Agent tools for NDP catalogs and the EarthScope demonstrations. [Official site of National Data Platform ↗](https://nationaldataplatform.org/)
  Data platform
- 04
  ### [NCSA](https://iowarp.ai/applications/national-infrastructure/)
  DeltaAI, where CLIO Core builds and runs. [Official site of NCSA ↗](https://www.ncsa.illinois.edu/)
  Facility
- 05
  ### [Oak Ridge National Laboratory](https://iowarp.ai/research/directions/)
  Co-authored research on in situ processing and simulation monitoring; the Flowcept provenance system. [Official site of Oak Ridge National Laboratory ↗](https://www.ornl.gov/)
  Research
- 06
  ### [NVIDIA](https://iowarp.ai/applications/gpu-data-movement/)
  NVIDIA GPU and data-movement technologies in CLIO Core research (CUDA, cuFile, NIXL, nvCOMP).
  Technology
- 07
  ### [Open-source communities](https://iowarp.ai/community/)
  Upstream contributions to external scientific projects, most of them in the HDF5 ecosystem.
  Upstream

03 / Team and support

## Team and support.

Anthony Kougkas created IOWarp and leads it. The IOWarp team works at the Gnosis Research Center at Illinois Tech. The University of Utah team contributes materials science workflows and AI research, and The HDF Group is the community integration partner that co-develops parts of CLIO Core with the Illinois Tech team. Everyone is listed by what they contribute.

Creator and project lead

### [Anthony Kougkas](https://akougkas.io/) [GitHub](https://github.com/akougkas)

Created IOWarp and leads its vision, architecture, and engineering.

### Core development

CLIO Core

- **[Luke Logan](https://grc.iit.edu/members/luke-logan/) Illinois Tech**CLIO Core developer: GPU, transport, and tiering

### Agents and tools

CLIO Agent and CLIO Kit

- **[Jaime Cernuda](https://grc.iit.edu/members/jaime-cernuda/) Illinois Tech**CLIO Agent developer
- **Shazzadul Islam Illinois Tech**Researcher: agentic scientific workflows
- **Aum Sathwara Illinois Tech**Software developer: MCP servers
- **Soham Sonar Illinois Tech**Software developer: MCP servers

### Research

Systems and agent research

- **[Isa Muradli](https://grc.iit.edu/members/isa-muradli/) Illinois Tech**Researcher: GPU compression and direct GPU I/O
- **Izzet Yildirim Illinois Tech**Researcher: agent I/O behavior and data staging
- **Jie Ye Illinois Tech**Researcher: KV-cache-aware inference scheduling
- **Hua Xu Illinois Tech**Researcher: multimodal agents for simulation monitoring
- **Rajni Pawar Illinois Tech**Researcher: semantic search for HPC data
- **Meng Tang Illinois Tech**Researcher: I/O-aware workflow scheduling, through August 2026
- **Keith Bateman Illinois Tech**Researcher: doctoral research
- **Neeraj Rajesh Illinois Tech**Researcher: doctoral research
- **Zia Uddin Chowdhury Illinois Tech**Researcher: doctoral research

### Partners

**The HDF Group** · Community integration

- **[Gerd Heber](https://www.hdfgroup.org/team/gerd-heber/) The HDF Group**HDF Group development
- **Jordan Henderson The HDF Group**Community liaison: technical coordination and outreach
- **Hyo Kyung (Joe) Lee The HDF Group**Software developer: runtime and assimilation engine engineering, release and CI infrastructure
- **Matthew Larson The HDF Group**Agent developer: agentic HDF5, agent skills, and workflow guardrails
- **Larry Knox The HDF Group**Software developer: testing on national research systems
- **M. Scot Breitenfeld The HDF Group**Community liaison: outreach and community engagement

**University of Utah** · Materials science

- **[Jacob Hochhalter](https://www.mech.utah.edu/directory/faculty/jacob-hochhalter/) University of Utah**Researcher: materials science workflows
- **[Vivek Srikumar](https://www.cs.utah.edu/srikumar-vivek/) University of Utah**Researcher: AI and machine learning
- **Daisy Quach University of Utah**Researcher: materials research workflows
- **Oliver Bentham University of Utah**Researcher: the InfiniteScienceGym benchmark

### Advisors

- **[Xian-He Sun](https://www.iit.edu/directory/people/xian-he-sun) Illinois Tech**Senior advisor

Many more people contribute through code, issues, testing, and talks. Every repository’s contributor history is public on [GitHub](https://github.com/iowarp). Summer interns, course projects, and community coding sessions have added to the work since 2025.

**Support.** The U.S. National Science Foundation supports IOWarp through collaborative awards OAC-2411318 and OAC-2411319.

**Computing.** This work used the DeltaAI system at the National Center for Supercomputing Applications [award OAC 2320345] through allocation CIS250329 from the Advanced Cyberinfrastructure Coordination Ecosystem: Services & Support (ACCESS) program, which is supported by National Science Foundation grants #2138259, #2138286, #2138307, #2137603, and #2138296.

**Collaboration.** The DOE Genesis Mission and the American Science Cloud (AmSC) support IOWarp with computing and collaboration.

Next step

## Meet the team in Chicago at SC26.

[IOWarp at SC26](https://iowarp.ai/community/#sc26) [Ways to collaborate](https://iowarp.ai/community/#collaborate)

SC26 runs November 15–20, 2026, at McCormick Place.
