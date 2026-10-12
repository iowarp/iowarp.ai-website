---
title: "Community and IOWarp at SC26 | IOWarp"
description: "IOWarp at SC26 in Chicago, the user group, the Technical Advisory Board forming at the end of November 2026, and ways to contribute to the CLIO stack."
url: https://iowarp.ai/community/
---

> IOWarp at SC26 in Chicago, the user group, the Technical Advisory Board forming at the end of November 2026, and ways to contribute to the CLIO stack.

# Build where science meets systems.

For scientists, facility staff, tool builders, and students who use CLIO or want to shape it. IOWarp and the CLIO platform soft launch at SC26 in Chicago. This page lists the confirmed sessions, how the user group and the advisory board come together, and concrete ways to contribute.

SC26

November 15–20, 2026 · McCormick Place, Chicago

Talk to us

[Zulip ↗](https://iowarp.zulipchat.com/) · [Email the team](https://iowarp.ai/community/#contact)

On this page

SC26 · User group · Advisory board · Ways in · Contact

01 / IOWarp at SC26

## The soft launch at SC26.

IOWarp and the CLIO platform soft launch at SC26 in Chicago. The team presents work on simulation monitoring, GPU I/O, storage observability, compressed training data, and agent fleets through workshop presentations, research posters, a conference paper, and an HDF5 birds-of-a-feather session. The conference runs November 15–20, 2026 at McCormick Place, Chicago, Illinois. It is not a single meeting: the user group gathers around these sessions, and advisory board invitations follow the conference.

- Workshops
- Posters
- Papers
- Birds of a feather

[SC26 conference site ↗](https://sc26.supercomputing.org/)

- 01
  ### Workshop [GPUH5: A GPU-first I/O Library for Scientific Data](https://sc26.conference-program.com/presentation/?id=ws_pdsw111&sess=sess129)
  Monday, November 16, 2026, 10:50–11:10 am CST · Room W175bc PDSW’26: The 11th International Parallel Data Systems Workshop GPU-initiated writes for persistent kernels, with hierarchical paths and chunked arrays backed by a key-value store.
- 02
  ### Workshop [GDSight: Per-Operation Cross-Layer Attribution for GPUDirect Storage](https://sc26.conference-program.com/presentation/?id=ws_pdsw125&sess=sess129)
  Monday, November 16, 2026, 11:30–11:50 am CST · Room W175bc PDSW’26: The 11th International Parallel Data Systems Workshop eBPF tracing that attributes NVMe device commands to the cuFile or POSIX operation that caused them.
- 03
  ### Workshop [Trigger-Gated Multimodal LLM Agents for In-situ Scientific Simulation Monitoring](https://sc26.conference-program.com/presentation/?id=ws_pdswwip113&sess=sess129)
  Monday, November 16, 2026, 12:15–12:20 pm CST · Room W175bc PDSW’26: The 11th International Parallel Data Systems Workshop Work-in-progress presentation on Vigil: deterministic triggers, in-transit rendering, and agent-driven ParaView inspection on the simulation I/O path.
- 04
  ### Poster [Extending I/O Observability to Explainability for Targeted Optimization](https://sc26.conference-program.com/presentation/?id=rpost229&sess=sess313)
  Tuesday, November 17, 2026, 10:00 am–5:00 pm CST · Skyline Ballroom North Pre-Function Research posters display · Poster Blitz PEARL, an eBPF tracing plugin for DataCrumbs, follows requests from system calls to disk completion to explain the causes of I/O bottlenecks.
- 05
  ### Poster [GNNs Beyond HBM: Compressed, Bit-Exact Feature Streaming for Out-of-Core Training](https://sc26.conference-program.com/presentation/?id=rpost258&sess=sess313)
  Tuesday, November 17, 2026, 10:00 am–5:00 pm CST · Skyline Ballroom North Pre-Function Research posters display · Poster Blitz GnnPress streams compressed node features through a bounded GPU memory window for graph neural network training, with a lossless path that preserves exact values.
- 06
  ### Poster [StageOnce: Speculative Cross-Job Data Staging for LLM Agent Fleets](https://sc26.conference-program.com/presentation/?id=rpost305&sess=sess313)
  Tuesday, November 17, 2026, 10:00 am–5:00 pm CST · Skyline Ballroom North Pre-Function Research posters display · Poster Blitz A node-local daemon coordinates speculative input staging across agent jobs, sharing immutable dataset copies while preserving versions and private outputs.
- 07
  ### Poster [ToolFuse: Provenance-Aware In-Flight Coalescing of Redundant Agent Tool Calls](https://sc26.conference-program.com/presentation/?id=rpost306&sess=sess313)
  Tuesday, November 17, 2026, 10:00 am–5:00 pm CST · Skyline Ballroom North Pre-Function Research posters display · Poster Blitz A provenance-aware gateway coalesces equivalent read-only tool calls while they are running, using versioned dependencies and execution context to establish equivalence.
- 08
  ### Paper [Trigger, Render, Reason: Multimodal LLM Agents for Science-Aware Scientific Simulation Monitoring](https://sc26.conference-program.com/presentation/?id=pap1039&sess=sess236)
  Wednesday, November 18, 2026, 4:30–5:00 pm CST · Room W181abc Papers in Conversation: Scientific AI at Extreme Scale Vigil combines science-aware triggers with rendering and multimodal reasoning to check running simulations for invalid scientific states.
- 09
  ### Birds of a feather [Trustworthy Data at Scale: HDF5 in the Age of AI-Driven Science](https://sc26.conference-program.com/presentation/?id=bof168&sess=sess428)
  Thursday, November 19, 2026, 12:15–1:15 pm CST · Room W185d An HDF5 community discussion on provenance, concurrent I/O, and cloud interoperability, with an opt-in agentic survey of attendee priorities and pain points.

All times are Central Standard Time in Chicago. Poster times cover the display session; the posters are also marked for Poster Blitz in the conference program. Follow each program entry for updates.

02 / The user group

## The IOWarp user group.

A working community for people who use, operate, or build on CLIO. The team plans user group meetings where upcoming releases are discussed and feedback from users shapes what comes next. The user group first gathers around IOWarp’s events at SC26.

How to take part

1. Tell the team you are interested in
  [Zulip](https://iowarp.zulipchat.com/)
  or by
  [email](https://iowarp.ai/community/#contact)
  .
2. Name the component you use and the workflow you would bring.
3. The team sends details before each gathering and follows up on what you raise in the public issue trackers.
- 01
  ### The stack, layer by layer
  What changed across CLIO Core, Kit, Agent, CLIO Coder, and the research tools since the last release, and what is planned on the path to a stable platform release.
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

Invitations follow SC26, starting with the research collaborators who have worked with the project since its beginning. The board forms at the end of November 2026, after SC26, and members will be listed on this page once they accept.

- 01 / Role
  ### Align with real needs
  Keep CLIO aligned with how scientific data is actually managed, moved, and analyzed today.
- 02 / Role
  ### Carry user feedback
  Bring the experience of facilities, application teams, and tool builders into release planning.
- 03 / Role
  ### Set priorities
  Advise on development priorities across the stack as the project moves toward a stable platform release.

04 / Ways in

## More than one entry point.

- 01 / Contribution path
  ### Research partnership
  Define a scientific workload, a research question, an evaluation plan, and a shared publication path with the team.
  Discuss a collaboration →
  <https://iowarp.ai/community/#contact>
- 02 / Contribution path
  ### Compute and infrastructure
  Provide machines, storage, instruments, or test environments where context systems have to work for real.
  Discuss resources →
  <https://iowarp.ai/community/#contact>
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

For institutional sponsorship terms or a formal research agreement, write to the Gnosis Research Center by [email](https://iowarp.ai/community/#contact). The team and its support are described on the [About page](https://iowarp.ai/about/#team).

05 / A good first exchange

## Make the problem reproducible.

1. 01
  Choose the repository for the component you used. The [platform page](https://iowarp.ai/platform/) lists every component and where its source lives.
2. 02
  Open an issue with the version, environment, input format, expected behavior, observed behavior, and the smallest safe example you can share.
3. 03
  Bring a proposed fix or a benchmark when possible. Tests and documentation that make a scientific workflow repeatable are valuable contributions.
4. 04
  Continue the conversation in [Zulip](https://iowarp.zulipchat.com/) or write to the Gnosis Research Center [by email](https://iowarp.ai/community/#contact) about a collaboration.

06 / Gatherings

## Meet the people behind it.

- 01
  ### Coding sessions
  Weekly CLIO coding sessions on the Illinois Tech campus bring students and researchers together to build and debug the stack. Ask in Zulip if you would like to join one.
- 02
  ### Talks and tutorials
  Team members present IOWarp at research conferences and community meetings, including SC, a research cyberinfrastructure meeting in Denver, IEEE eScience, and The HDF Group’s HDF Clinic. The [news page](https://iowarp.ai/news/) lists dated items with sources.
- 03
  ### Hackathons
  The [Gnosis project record](https://grc.iit.edu/research/projects/iowarp/) reports that the team ported CLIO Core to Aurora at the INCITE GPU hackathon and ran scientific workloads. Public [Aurora deployment recipes](https://github.com/iowarp/clio-core/tree/v2.2.1/jarvis_clio_core/pipelines/aurora) provide implementation context.

07 / Contact

## Write to the team.

The contact form is for collaboration proposals, questions about using CLIO, and press requests. Formal sponsorship terms and research agreements start here too. For quick questions from users and contributors, [Zulip](https://iowarp.zulipchat.com/) is faster, and the answers help others.

Next step

## Bring the hard problem.

[Join the conversation on Zulip](https://iowarp.zulipchat.com/) [Write to the team](https://iowarp.ai/community/#contact)
