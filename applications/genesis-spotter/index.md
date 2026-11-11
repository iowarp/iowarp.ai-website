---
title: "Provenance and integrity for AI-driven science | IOWarp"
description: "SPOTTER-AI, a DOE Genesis Mission project at Argonne National Laboratory, on provenance for AI science workflows, and the role of CLIO Agent in it."
url: https://iowarp.ai/applications/genesis-spotter/
---

> SPOTTER-AI, a DOE Genesis Mission project at Argonne National Laboratory, on provenance for AI science workflows, and the role of CLIO Agent in it.

# Provenance and integrity for AI-driven science.

SPOTTER-AI is a DOE Genesis Mission project. Argonne National Laboratory leads it, with Oak Ridge National Laboratory, Illinois Tech, and Hewlett Packard Enterprise as partners. It addresses cybersecurity for AI-driven science through data provenance and integrity verification. The project began in August 2026. The IOWarp team builds the agents that investigate what the provenance shows.

Partners

Argonne National Laboratory · Oak Ridge National Laboratory · Illinois Tech · Hewlett Packard Enterprise

Status

Project began August 2026

Stack layers

Agents and tools · Applications

Components

[CLIO Agent](https://iowarp.ai/platform/#agent) · [Agent marketplace](https://iowarp.ai/platform/#marketplace) · [CLIO Kit](https://iowarp.ai/platform/#kit)

On the web

[Argonne National Laboratory ↗](https://www.anl.gov/) · [Oak Ridge National Laboratory ↗](https://www.ornl.gov/) · [Illinois Institute of Technology ↗](https://www.iit.edu/) · [Hewlett Packard Enterprise ↗](https://www.hpe.com/) · [U.S. Department of Energy Genesis Mission ↗](https://genesis.energy.gov/) · [SPOTTER-AI on GitHub ↗](https://github.com/spotter-ai-genesis) · [Flowcept ↗](https://flowcept.readthedocs.io/) · [CMF ↗](https://github.com/HewlettPackard/cmf)

01 / The scientific question

## When a scientific AI workflow produces a wrong answer, can we tell whether it was tampered with, and trace the cause to its source?

AI models, datasets, and workflows are increasingly shared across facilities. A poisoned passage in a retrieval corpus or a manipulated tool call can quietly change what a model concludes, and every result built on that conclusion inherits the damage.

SPOTTER-AI captures detailed provenance of workflows and of the models inside them, learns how much influence each input should have on an outcome, and treats departures from that expectation as a signal worth investigating.

**WHERE CONTEXT BREAKS** Provenance helps only if someone can question it. The records span workflow events, artifact lineage, and signals from inside the model, across systems never designed to be read together. An investigating agent needs bounded, read-only access to all of it, and its own actions must meet the same standard of evidence.

02 / Workflow

## The workflow, stage by stage.

**FIG A3.1** · DOE Genesis · SPOTTER-AI workflow 4 stages

1. **Capture**
  Workflow and model provenance, including token-importance signals from inference, is recorded by provenance systems such as Flowcept.
  Partner systems
2. **Expose**
  A read-only provenance server gives an investigating agent tools for correlation, artifact lineage, and timelines across providers.
  Agent marketplace · MCP
3. **Watch**
  A standing watcher agent observes a session, treats instructions inside files or pages as evidence rather than orders, and quarantines the session on a danger finding while destructive calls wait for clearance.
  CLIO Agent · Spotter mode
4. **Attribute**
  Agentic forensic analysis works backward from an anomaly to its likely root cause and reports it to the people responsible.
  CLIO Agent

Stages as the project describes them.

03 / Software in the loop

## The instruments involved.

01 / Component**CLIO Agent**

The Spotter approval mode and the investigating agents.

Open source ↗

<https://github.com/iowarp/clio-agent>

02 / Component**Agent marketplace**

The SPOTTER provenance investigator plugin and its read-only provenance MCP server.

Open source ↗

<https://github.com/iowarp/clio-agent-marketplace/tree/main/plugins/spotter>

03 / Component**CLIO Kit**

Scientific tools that the investigated workflows may use.

Read more →

<https://iowarp.ai/clio-kit/>

04 / What comes next

## Next steps.

1. Connect the investigation layer to the project’s scientific testbed workflows.
2. Instruction-tune a foundation model for provenance analysis.
3. Record a demonstration of CLIO Agent working with SPOTTER-AI.

Who should get in touch

Facility security teams, provenance-system developers, and owners of AI workflows who need to know when a result can be trusted.

[Propose a collaboration](mailto:partnerships@iowarp.ai?subject=%5BIOWarp-website%5D%20Collaboration%3A%20Provenance%20and%20integrity%20for%20AI-driven%20science) [Join the community](https://iowarp.ai/community/)

Related

## Topics, research, and demos.

- [Topic **Scientific AI agents**](https://iowarp.ai/topics/scientific-agents/)
- [Topic **Evidence-based autonomous research**](https://iowarp.ai/topics/evidence-based-research/)
- [Research direction **Provenance an agent can question** When a result is wrong, can we find out why?](https://iowarp.ai/research/directions/#provenance)
- [Demo **DOE Genesis: SPOTTER-AI and PORTUS** Planned for 2026](https://iowarp.ai/research/demos/#demo-doe-genesis-spotter-ai-and-portus)

Next application · A4

## Agentic workflows across HPC and cloud.

[Read the next story](https://iowarp.ai/applications/genesis-portus/) [All applications](https://iowarp.ai/applications/)
