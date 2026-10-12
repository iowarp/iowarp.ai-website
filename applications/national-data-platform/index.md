---
title: "Agents on the National Data Platform | IOWarp"
description: "How CLIO Kit exposes the National Data Platform to agents, and what the EarthScope demonstrations showed."
url: https://iowarp.ai/applications/national-data-platform/
---

> How CLIO Kit exposes the National Data Platform to agents, and what the EarthScope demonstrations showed.

# Agents on the National Data Platform.

The National Data Platform federates scientific data catalogs so researchers can find and use data across institutions. IOWarp builds agent tools on top of it.

Partners

National Data Platform · University of Utah · Illinois Tech

Status

Demonstrated on EarthScope data

Stack layers

Agents and tools · Applications

Components

[CLIO Kit](https://iowarp.ai/platform/#kit) · [Agent marketplace](https://iowarp.ai/platform/#marketplace) · [CLIO Agent](https://iowarp.ai/platform/#agent)

On the web

[National Data Platform ↗](https://nationaldataplatform.org/) · [EarthScope Consortium ↗](https://www.earthscope.org/) · [University of Utah ↗](https://www.utah.edu/) · [Illinois Institute of Technology ↗](https://www.iit.edu/) · [Chameleon Cloud ↗](https://www.chameleoncloud.org/) · [Model Context Protocol ↗](https://modelcontextprotocol.io/)

Record

What the work has produced · Sources

01 / The scientific question

## Can an agent go from a plain-language request to a staged, analyzed, and plotted dataset from a federated catalog without a human wiring every step?

Federated catalogs make data findable, but using a dataset still takes a sequence of manual steps: search several catalogs, interpret metadata, download the right resource, check its structure, then analyze and plot it.

Each step depends on context the previous one produced. Without that context an agent either stalls or improvises.

**WHERE CONTEXT BREAKS** The failure mode is not a lack of intelligence. It is missing context: which catalog, which resource, what the columns mean, where the data was staged. CLIO Kit turns each of those into a tool with a defined contract.

02 / Workflow

## The workflow, stage by stage.

**FIG A2.1** · Data infrastructure workflow 4 stages

1. **Locate**
  Geospatial tools narrow the request to candidate stations or sites.
  CLIO Kit · Geo
2. **Search the catalog**
  The NDP server searches datasets across the platform’s catalogs and returns structured metadata.
  CLIO Kit · NDP
3. **Stage and profile**
  The agent retrieves the chosen resource into a controlled staging area and profiles it before analysis.
  CLIO Kit · Pandas
4. **Analyze and plot**
  Plotting and visualization tools produce figures the researcher can check against the source data.
  CLIO Kit · Plot, ParaView

Stages as the project sources describe them. What each stage has produced so far is listed in the record below.

**FIG A2.2** · Reference figure

![Still from a recording of an agent searching the National Data Platform for EarthScope data.](https://iowarp.ai/images/demos/ndp-claude.webp)

Still from the October 2025 recording of the NDP and EarthScope workflow.

03 / The record

## What the work has produced.

1. With IOWarp context, an agent completed EarthScope data retrieval and visualization through NDP; the comparison agent without that context did not complete the workflow. [1] [2]
  CONDITIONS · Agent runs on Chameleon Cloud, reported in an IEEE eScience 2025 poster that states the models and timings
2. A public recording shows an agent examining EarthScope seismograph data found through the National Data Platform. [3]
3. CLIO Kit ships an NDP server with documentation, and callers choose where it stages and writes data. [4] [5]

04 / Software in the loop

## The instruments involved.

01 / Component**CLIO Kit · NDP server**

Dataset search and retrieval across NDP catalogs.

Open source ↗

<https://toolkit.iowarp.ai/docs/mcps/ndp>

02 / Component**CLIO Kit · Pandas, Plot, Geo**

Profiling, plotting, and geospatial filtering.

Read more →

<https://iowarp.ai/clio-kit/>

03 / Component**CLIO Agent packs**

EarthScope agent packs in the CLIO Agent marketplace.

Open source ↗

<https://github.com/iowarp/clio-agent-marketplace>

05 / What comes next

## Next steps.

1. Publish a repeatable NDP workflow with a pinned catalog snapshot, since live catalogs change between runs.
2. Record the 2026 EarthScope demonstration on current releases.
3. Extend beyond EarthScope to other NDP-federated domains.

Who should get in touch

Data platform operators, catalog maintainers, and domain scientists whose data is already findable but still hard to use.

[Propose a collaboration](https://iowarp.ai/community/#contact) [Join the community](https://iowarp.ai/community/)

Related

## Topics, research, and demos.

- [Topic **MCP servers for scientific computing**](https://iowarp.ai/topics/mcp-for-science/)
- [Topic **Scientific AI agents**](https://iowarp.ai/topics/scientific-agents/)
- [Topic **Context management for AI agents**](https://iowarp.ai/topics/context-management/)
- [Demo **EarthScope through the National Data Platform, 2026** Planned for 2026](https://iowarp.ai/research/demos/#demo-earthscope-through-the-national-data-platform-2026)
- [Demo **EarthScope seismograph analysis** Recorded 2025](https://iowarp.ai/research/demos/#demo-earthscope-seismograph-analysis)

06 / Sources

## Sources

1. [Islam, Cernuda, Muradli, Kougkas, Sun. Towards an AI-driven scientific workflow. IEEE eScience 2025 (poster)](https://doi.org/10.1109/eScience65000.2025.00074)
2. [eScience 2025 poster PDF: EarthScope, LAMMPS, ParaView, and IOR agent workflows](http://cs.iit.edu/~scs/assets/files/islam2025aidriven_poster.pdf)
3. [Agent examining EarthScope data through the National Data Platform (video, October 2025)](https://www.youtube.com/watch?v=9NUf76wnHhA)
4. [CLIO Kit NDP MCP server documentation](https://toolkit.iowarp.ai/docs/mcps/ndp)
5. [CLIO Kit source repository](https://github.com/iowarp/clio-kit)

Next application · A3

## Provenance and integrity for AI-driven science.

[Read the next story](https://iowarp.ai/applications/genesis-spotter/) [All applications](https://iowarp.ai/applications/)
