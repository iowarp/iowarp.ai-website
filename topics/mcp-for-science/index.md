---
title: "MCP servers for scientific computing | IOWarp"
description: "MCP servers for science: how the Model Context Protocol connects AI agents to HDF5, Slurm, ParaView, and other scientific tools through CLIO Kit."
url: https://iowarp.ai/topics/mcp-for-science/
---

> MCP servers for science: how the Model Context Protocol connects AI agents to HDF5, Slurm, ParaView, and other scientific tools through CLIO Kit.

# MCP servers for scientific computing.

The Model Context Protocol is an open standard through which AI applications call external tools and read external resources. An MCP server wraps a capability, such as reading an HDF5 dataset or submitting a Slurm job, behind a described interface any compatible client can use.

01 Why science needs its own servers 02 HDF5 with agents 03 What CLIO Kit provides 04 Design choices 05 How IOWarp approaches it 06 Common questions

01

## Why science needs its own servers

General-purpose tools do not understand hierarchical scientific formats, job schedulers, I/O traces, or domain catalogs. A server that knows how to list HDF5 groups or parse a Darshan log gives an agent precise operations instead of guesswork over raw bytes.

02

## HDF5 with agents

HDF5 is a standard format for simulation and experimental data across the sciences. CLIO Kit’s HDF5 server lets an agent list groups, inspect datasets and attributes, and read slices without pulling whole files, and CLIO Core’s HDF5 VOL connector lets existing HDF5 applications place data through the runtime without code changes.

The HDF Group works on agentic HDF5 and agent skills with the IOWarp team, and at SC26 a birds-of-a-feather session covers HDF5 in AI-driven science.

03

## What CLIO Kit provides

CLIO Kit is an open-source meta-marketplace of scientific MCP servers, skills, agents, hooks, and workflow plugins. Its servers cover data formats (HDF5, Parquet, ADIOS, Pandas), HPC operations (Slurm, Spack, Lmod, Jarvis, Darshan, node hardware), visualization (ParaView, Plot), geospatial and seismic data, and discovery (ArXiv, NDP, scientific catalogs, web search).

The launcher installs from PyPI as clio-kit and downloads selected components on demand. Project installers support Codex, Claude Code, OpenCode, Cursor, Antigravity, and VS Code; agents and hooks have client-specific adapters and limits.

04

## Design choices

Each server is separately versioned and testable, so a facility can adopt only the servers it trusts. Component downloads are verified, and server dependencies stay isolated and locked. Tools return structured results, which makes an agent’s steps easier to check afterward.

How IOWarp approaches it

## Where to go deeper.

01**CLIO Kit catalog**

Every server, grouped by capability, with install commands.

Continue →

<https://iowarp.ai/clio-kit/>

02**Connect an MCP client**

Register CLIO Kit servers in Claude Code, Cursor, VS Code, and other clients.

Continue →

<https://iowarp.ai/clio-kit/#connect>

03**CLIO Kit guides**

Component setup, workflow plugins, and client guides.

Open ↗

<https://toolkit.iowarp.ai/docs/intro>

04**Kit client support**

Choose skills, MCP configuration, agents, and hooks that your client supports.

Open ↗

<https://toolkit.iowarp.ai/docs/clients#component-support>

05**Anthropic’s introduction to MCP**

Further reading: Why an open protocol connects AI applications to external data and capabilities.

Open ↗

<https://www.anthropic.com/news/model-context-protocol>

06**Anthropic on designing effective tools**

Further reading: Designing precise tool interfaces and useful results, then evaluating whether agents can operate them.

Open ↗

<https://www.anthropic.com/engineering/writing-tools-for-agents>

Applications that use it

- A2
  ### [Agents on the National Data Platform](https://iowarp.ai/applications/national-data-platform/)
  MCP tools that let an agent search, stage, and analyze datasets federated through the National Data Platform, first shown on EarthScope data.
  Demonstrated on EarthScope data
- A5
  ### [CLIO on national research systems](https://iowarp.ai/applications/national-infrastructure/)
  Where CLIO Core has been built and run: ALCF Aurora, DeltaAI, and the Ares cluster.
  Built and run on national systems

Common questions

## Common questions.

**How do I install a CLIO Kit server?**

Install the launcher with uv tool install clio-kit, then run clio-kit mcp-server followed by the server name. It downloads that component and prepares its isolated runtime. Register the command in your MCP client, or use a workflow plugin to install its MCP configuration and skills together.

**Is CLIO Kit tied to one AI vendor?**

No. It implements the open MCP standard and is documented for several clients.

Related

## Research and demos on this topic.

- [Demo **EarthScope through the National Data Platform, 2026** Planned for 2026](https://iowarp.ai/research/demos/#demo-earthscope-through-the-national-data-platform-2026)
- [Demo **CLIO on DeltaAI and Aurora** Planned for 2026](https://iowarp.ai/research/demos/#demo-clio-on-deltaai-and-aurora)
- [Demo **EarthScope seismograph analysis** Recorded 2025](https://iowarp.ai/research/demos/#demo-earthscope-seismograph-analysis)

## References

1. [CLIO Kit source repository](https://github.com/iowarp/clio-kit)
2. [CLIO Kit NDP MCP server documentation](https://toolkit.iowarp.ai/docs/mcps/ndp)
3. [ParaView MCP server in CLIO Kit, derived from LLNL paraview_mcp](https://github.com/iowarp/clio-kit/tree/v2.11.0/mcp-servers/paraview)
4. [Islam, Cernuda, Muradli, Kougkas, Sun. Towards an AI-driven scientific workflow. IEEE eScience 2025 (poster)](https://doi.org/10.1109/eScience65000.2025.00074)
5. [Model Context Protocol specification and documentation](https://modelcontextprotocol.io/)
6. [HDF5, The HDF Group](https://www.hdfgroup.org/solutions/hdf5/)
7. [Anthropic’s introduction to MCP](https://www.anthropic.com/news/model-context-protocol)
8. [Anthropic on designing effective tools](https://www.anthropic.com/engineering/writing-tools-for-agents)

## Other concepts

- [T1 Context management for AI agents](https://iowarp.ai/topics/context-management/)
- [T2 Scientific AI agents](https://iowarp.ai/topics/scientific-agents/)
- [T4 HPC I/O and storage hierarchies](https://iowarp.ai/topics/hpc-io/)
- [T5 Data movement for AI-infused workflows](https://iowarp.ai/topics/data-movement/)
- [T6 Scientific workflows and reproducible deployment](https://iowarp.ai/topics/scientific-workflows/)
- [T7 Evidence-based autonomous research](https://iowarp.ai/topics/evidence-based-research/)

Next step

## See this topic at work.

[Agents on the National Data Platform](https://iowarp.ai/applications/national-data-platform/) [All concepts](https://iowarp.ai/docs/#concepts)
