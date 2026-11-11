---
title: "Community and IOWarp at SC26 | IOWarp"
description: "IOWarp builds CLIO, the open stack for AI-driven science. The full stack will launch at SC26 in Chicago. Join the user group or contribute."
url: https://iowarp.ai/community/
---

> IOWarp builds CLIO, the open stack for AI-driven science. The full stack will launch at SC26 in Chicago. Join the user group or contribute.

# Build where science meets systems.

IOWarp is the team at the Gnosis Research Center that builds CLIO, open-source software that connects AI agents to scientific data and the systems that hold it. That connection matters because it lets an organization bring AI into its science and keep the work checkable. IOWarp will launch the full stack at SC26 in Chicago. This page lists the confirmed sessions, how the user group and the advisory board will form, and the ways to join in.

SC26

November 15–20, 2026 · McCormick Place, Chicago

Talk to us

[Zulip ↗](https://iowarp.zulipchat.com/) · [Email the team](mailto:info@iowarp.ai?subject=%5BIOWarp-website%5D%20Contact)

On this page

SC26 · User group · Advisory board · Ways in · Contact

01 / IOWarp at SC26

## The full-stack launch at SC26.

IOWarp will launch the full CLIO stack at SC26 in Chicago. The team will present work on simulation monitoring, GPU I/O, storage observability, compressed training data, and agent fleets through workshop presentations, research posters, a conference paper, and an HDF5 birds-of-a-feather session with The HDF Group. The conference runs November 15–20, 2026 at McCormick Place, Chicago, Illinois. The user group will gather around these sessions, and advisory board invitations will follow the conference.

- Workshops
- Posters
- Papers
- Birds of a feather

[Add sessions to calendar (.ics)](https://iowarp.ai/sc26.ics) [SC26 conference site](https://sc26.supercomputing.org/)

[Explore the CLIO suite →](https://iowarp.ai/#try) · [See how the stack fits together →](https://iowarp.ai/platform/)

### MON · NOV 16 · PDSW’26 Workshop

Room W179b

PDSW’26: The 11th International Parallel Data Systems Workshop

- Workshop · 10:50–11:10 am CST
  #### [GPUH5: A GPU-first I/O Library for Scientific Data](https://sc26.conference-program.com/presentation/?id=ws_pdsw111&sess=sess129)
  GPU-initiated writes for persistent kernels, with hierarchical paths and chunked arrays backed by a key-value store.
- Workshop · 11:30–11:50 am CST
  #### [GDSight: Per-Operation Cross-Layer Attribution for GPUDirect Storage](https://sc26.conference-program.com/presentation/?id=ws_pdsw125&sess=sess129)
  eBPF tracing that attributes NVMe device commands to the cuFile or POSIX operation that caused them.
- Workshop · 12:15–12:20 pm CST
  #### [Trigger-Gated Multimodal LLM Agents for In-situ Scientific Simulation Monitoring](https://sc26.conference-program.com/presentation/?id=ws_pdswwip113&sess=sess129)
  Work-in-progress presentation on Vigil: deterministic triggers, in-transit rendering, and agent-driven ParaView inspection on the simulation I/O path.

### TUE · NOV 17 · Research Posters · Poster Blitz

Skyline Ballroom North Pre-Function

Research posters display · Poster Blitz

- Poster · 10:00 am–5:00 pm CST
  #### [Extending I/O Observability to Explainability for Targeted Optimization](https://sc26.conference-program.com/presentation/?id=rpost229&sess=sess313)
  PEARL, an eBPF tracing plugin for DataCrumbs, follows requests from system calls to disk completion to explain the causes of I/O bottlenecks.
- Poster · 10:00 am–5:00 pm CST
  #### [GNNs Beyond HBM: Compressed, Bit-Exact Feature Streaming for Out-of-Core Training](https://sc26.conference-program.com/presentation/?id=rpost258&sess=sess313)
  GnnPress streams compressed node features through a bounded GPU memory window for graph neural network training, with a lossless path that preserves exact values.
- Poster · 10:00 am–5:00 pm CST
  #### [StageOnce: Speculative Cross-Job Data Staging for LLM Agent Fleets](https://sc26.conference-program.com/presentation/?id=rpost305&sess=sess313)
  A node-local daemon coordinates speculative input staging across agent jobs, sharing immutable dataset copies while preserving versions and private outputs.
- Poster · 10:00 am–5:00 pm CST
  #### [ToolFuse: Provenance-Aware In-Flight Coalescing of Redundant Agent Tool Calls](https://sc26.conference-program.com/presentation/?id=rpost306&sess=sess313)
  A provenance-aware gateway coalesces equivalent read-only tool calls while they are running, using versioned dependencies and execution context to establish equivalence.

### WED · NOV 18 · Papers in Conversation

Room W181abc

Papers in Conversation: Scientific AI at Extreme Scale

- Paper · 4:30–5:00 pm CST
  #### [Trigger, Render, Reason: Multimodal LLM Agents for Science-Aware Scientific Simulation Monitoring](https://sc26.conference-program.com/presentation/?id=pap1039&sess=sess236)
  Vigil combines science-aware triggers with rendering and multimodal reasoning to check running simulations for invalid scientific states.

### THU · NOV 19 · Birds of a Feather

Room W185d

- Birds of a feather · 12:15–1:15 pm CST
  #### [Trustworthy Data at Scale: HDF5 in the Age of AI-Driven Science](https://sc26.conference-program.com/presentation/?id=bof168&sess=sess428)
  An HDF5 community discussion on provenance, concurrent I/O, and cloud interoperability, with an opt-in agentic survey of attendee priorities and pain points.

All times are Central Standard Time in Chicago. Poster times cover the display session; the posters are also marked for Poster Blitz in the conference program. Follow each program entry for updates.

02 / The user group

## The IOWarp user group.

A working community for people who use, operate, or build on CLIO. Its meetings will cover upcoming releases, and what users report will shape what comes next. The group will first gather around IOWarp’s events at SC26.

How to take part

1. Tell the team you are interested in
  [Zulip](https://iowarp.zulipchat.com/)
  or by
  [email](mailto:info@iowarp.ai?subject=%5BIOWarp-website%5D%20User%20group)
  .
2. Name the component you use and the workflow you would bring.
3. The team sends details before each gathering and follows up on what you raise in the public issue trackers.
- 01
  ### The stack, layer by layer
  What changed across CLIO Core, CLIO Kit, CLIO Agent, and CLIO Coder since the last release, and what is planned on the path to a stable platform release.
- 02
  ### Reports from the field
  Application teams show where CLIO helped and where it failed: materials science, the National Data Platform, national research systems, and DOE laboratory projects.
- 03
  ### Your workflow, on the table
  Bring a dataset, a failure, or a missing tool. Requests heard here go into the public issue trackers with owners and follow-up.
- 04
  ### The advisory board
  Hear how the Technical Advisory Board will form after SC26, and suggest the questions it should take up.

Who should come

- Scientists running data-heavy or agent-assisted workflows
- Facility and HPC center staff
- Developers of scientific tools, formats, and MCP servers
- Students and researchers in systems, I/O, and AI for science

03 / Technical Advisory Board

## Advice from outside the team.

IOWarp plans a Technical Advisory Board with members from academia, industry, and government laboratories. The board advises the IOWarp team on technical direction.

Invitations will follow SC26, starting with the research collaborators who have worked with the project since its beginning. The board will form at the end of November 2026, and members will be listed on this page once they accept.

- 01 / Role
  ### Align with real needs
  Keep CLIO aligned with how scientific data is managed, moved, and analyzed.
- 02 / Role
  ### Carry user feedback
  Bring the experience of facilities, application teams, and tool builders into release planning.
- 03 / Role
  ### Set priorities
  Advise on development priorities across the stack as the project moves toward a stable platform release.

04 / Ways in

## Choose your way in.

- 01 / Contribution path
  ### Research partnership
  Define a scientific workload, a research question, an evaluation plan, and a shared publication path with the team.
  Discuss a collaboration →
  <mailto:partnerships@iowarp.ai?subject=%5BIOWarp-website%5D%20Collaboration>
- 02 / Contribution path
  ### Compute and infrastructure
  Provide machines, storage, instruments, or test environments where the stack has to hold up under real workloads.
  Discuss resources →
  <mailto:partnerships@iowarp.ai?subject=%5BIOWarp-website%5D%20Resources>
- 03 / Contribution path
  ### Build a scientific tool
  Connect a format, scheduler, instrument, or analysis library through CLIO Kit. Servers are small, separately versioned, and a good first contribution.
  Explore CLIO Kit →
  <https://iowarp.ai/clio-kit/>
- 04 / Contribution path
  ### Work on the runtime
  CLIO Core spans GPU code, Linux I/O backends, tiered storage, and the context engines. Bring a reproducible workload or a focused issue.
  CLIO Core on GitHub ↗
  <https://github.com/iowarp/clio-core>
- 05 / Contribution path
  ### Test an agent workflow
  Run CLIO Agent or CLIO Coder on your data, report what worked, and share a small, reproducible failure when it did not.
  See the platform →
  <https://iowarp.ai/platform/>
- 06 / Contribution path
  ### Bring an application
  Collaborations begin with a concrete scientific workload: a dataset, a baseline, and a question the current tools cannot answer.
  Read the applications →
  <https://iowarp.ai/applications/>

For institutional sponsorship terms or a formal research agreement, write to the IOWarp team by [email](mailto:partnerships@iowarp.ai?subject=%5BIOWarp-website%5D%20Sponsorship). The team and its support are described on the [About page](https://iowarp.ai/about/#team).

05 / A good first exchange

## Make the problem reproducible.

1. 01
  Choose the repository for the component you used. The [platform page](https://iowarp.ai/platform/) lists every component and where its source lives.
2. 02
  Open an issue with the version, environment, input format, expected behavior, observed behavior, and the smallest safe example you can share.
3. 03
  Bring a proposed fix or a benchmark when possible. Tests and documentation that make a scientific workflow repeatable are valuable contributions.
4. 04
  Continue the conversation in [Zulip](https://iowarp.zulipchat.com/) or write to the IOWarp team [by email](mailto:partnerships@iowarp.ai?subject=%5BIOWarp-website%5D%20Collaboration) about a collaboration.

06 / Gatherings

## Meet the people behind it.

- 01
  ### Coding sessions
  Weekly CLIO coding sessions on the Illinois Tech campus bring students and researchers together to build and debug the stack. Ask in Zulip to join a session.
- 02
  ### Talks and tutorials
  Team members bring IOWarp to research conferences and community meetings, including SC, IEEE eScience, and The HDF Group’s HDF Clinic. The [news page](https://iowarp.ai/news/) lists dated items with sources.
- 03
  ### Hackathons
  The team brings CLIO Core to GPU hackathons such as INCITE. The [Gnosis project record](https://grc.iit.edu/research/projects/iowarp/) describes the project. Public [Aurora deployment recipes](https://github.com/iowarp/clio-core/tree/v2.2.1/jarvis_clio_core/pipelines/aurora) show how CLIO Core deploys on a national system.

07 / Contact

## Write to the team.

Contact IOWarp using the project inbox that matches your question.

[info@iowarp.ai](mailto:info@iowarp.ai) General questions about IOWarp.

[partnerships@iowarp.ai](mailto:partnerships@iowarp.ai) Collaborations, partner institutions, and industry partnerships.

Next step

## Bring the hard problem.

[Join the conversation on Zulip](https://iowarp.zulipchat.com/) [Write to the team](mailto:info@iowarp.ai?subject=%5BIOWarp-website%5D%20Contact)
