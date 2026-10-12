---
title: "Agentic workflows across HPC and cloud | IOWarp"
description: "PORTUS, a DOE Genesis Mission project at PNNL: performance models that let agents plan and adapt scientific workflows across HPC and cloud."
url: https://iowarp.ai/applications/genesis-portus/
---

> PORTUS, a DOE Genesis Mission project at PNNL: performance models that let agents plan and adapt scientific workflows across HPC and cloud.

# Agentic workflows across HPC and cloud.

PORTUS is a DOE Genesis Mission project at Pacific Northwest National Laboratory. It asks how agentic scientific workflows on the Genesis Mission Platform can be predicted, planned, and adapted while they run across HPC and cloud resources. The project began in August 2026. The IOWarp team works on workflow motifs and performance models.

Partners

Pacific Northwest National Laboratory · Princeton Plasma Physics Laboratory · Iowa State University · University of Delaware · Illinois Tech · collaborating with Oak Ridge National Laboratory and HPE

Status

Project began August 2026

Stack layers

Agents and tools · Applications

Components

[CLIO Coder](https://iowarp.ai/platform/#coder)

On the web

[Pacific Northwest National Laboratory ↗](https://www.pnnl.gov/) · [Princeton Plasma Physics Laboratory ↗](https://www.pppl.gov/) · [Iowa State University ↗](https://www.iastate.edu/) · [University of Delaware ↗](https://www.udel.edu/) · [Illinois Institute of Technology ↗](https://www.iit.edu/) · [Oak Ridge National Laboratory ↗](https://www.ornl.gov/) · [Hewlett Packard Enterprise ↗](https://www.hpe.com/) · [U.S. Department of Energy Genesis Mission ↗](https://genesis.energy.gov/) · [WfCommons ↗](https://wfcommons.org/)

Record

What the work has produced · Sources

01 / The scientific question

## When an agent rewrites a scientific workflow as it runs, can it know what the new version will cost, and choose a better one, before it runs?

Agentic scientific workflows do not hold still. Agents change execution paths, generate new subgraphs at runtime, and run on a shifting mix of HPC and cloud resources that contend, fail, and reconfigure. Orchestrators that assume a static graph and fixed resources cannot predict these workflows, plan for contingencies, or rewrite fragments of them.

PORTUS starts from an observation: agentic workflows are built from a small vocabulary of recurring motifs, such as producer and consumer pipelines, fan-out and fan-in, staging loops, and handoffs from HPC simulation to AI inference. Performance models built over those motifs can transfer from one workflow to the next.

**WHERE CONTEXT BREAKS** A coding agent that generates a new workflow fragment needs to know what the fragment will cost on the resources available now: how much data moves between stages, where it waits, and which realization would run better. Surrogate performance models, grounded in memory- and data-centric performance foundations and refined by active learning on live telemetry, give the agent that context. With it the agent can reason about bottlenecks, rank alternatives, and retarget the fragment to the machine, and a domain scientist can describe a workflow in natural language and get a port that performs.

02 / Workflow

## The workflow, stage by stage.

**FIG A4.1** · DOE Genesis · PORTUS workflow 5 stages

1. **Characterize**
  Workflows and the HPC and cloud resources they run on are characterized, drawing on WfCommons workflows and agent-based proxies for Genesis projects.
  PPPL · ORNL · HPE
2. **Model the motifs**
  Compositional, graph-based surrogate models predict how recurring motifs perform. Illinois Tech extends the AMAT matching methodology from memory and storage to workflow dataflow.
  Illinois Tech
3. **Represent and generate**
  Workflows are represented across modalities for graph neural network reasoning, and new workflow instances are generated to train and test the models.
  Iowa State · University of Delaware
4. **Adapt as it runs**
  Telemetry from live runs feeds an adaptation and active-learning loop that refines the models and re-plans the workflow, building on PNNL’s DataFlowDrs tools.
  PNNL
5. **Run as a fleet**
  CLIO Coder fleets carry the measure, model, and re-plan loop as bounded, reviewable agent tasks. The integration is in progress.
  CLIO Coder

Stages as the project sources describe them. What each stage has produced so far is listed in the record below.

03 / The record

## What the work has produced.

1. PORTUS began in August 2026 as a DOE Genesis Mission project at PNNL, with Princeton Plasma Physics Laboratory, Iowa State University, the University of Delaware, and Illinois Tech as partners, and Oak Ridge National Laboratory and HPE collaborating. [1] [2]
2. The IOWarp team works on workflow motifs and performance models, extending the AMAT matching methodology from memory and storage to workflow dataflow. [1]
3. The PORTUS orchestrator is public: an agentic orchestration framework for scientific Slurm workflows that re-plans execution without rewriting task code. [3]
4. The Dataflow Performance Matcher from Illinois Tech predicts the I/O cost of workflow stages on candidate storage tiers and node counts. It builds on published research by Illinois Tech and PNNL on characterizing dataflow for I/O-aware scheduling. [4] [5]
5. CLIO Coder dispatches bounded engineering tasks to fleets of workers and returns reviewable run receipts. Connecting fleets to the PORTUS loop is in progress. [6]

04 / Software in the loop

## The instruments involved.

01 / Component**PORTUS orchestrator**

The project’s public agentic orchestration framework for scientific Slurm workflows, from PNNL.

Open source ↗

<https://gitlab.com/perflab-exact/portus/portus-orchestrator>

02 / Component**Dataflow Performance Matcher**

Illinois Tech’s I/O cost prediction for workflow stages across storage tiers and node counts.

Open source ↗

<https://gitlab.com/perflab-exact/dpm/dpm>

03 / Component**CLIO Coder**

Governed agent fleets with bounded tasks and run receipts; the connection to PORTUS is in progress.

Open source ↗

<https://coder.iowarp.ai/docs/guide/fleet-dispatch.html>

05 / What comes next

## Next steps.

1. Build compositional, graph-based surrogate models for recurring workflow motifs.
2. Generate and rank alternative realizations of a workflow: task fusion or decomposition, data staging, synchronous or asynchronous execution, and resource mappings.
3. Close the adaptation loop with active learning on live telemetry.
4. Let a domain scientist describe a workflow in natural language and receive a performant port, with CLIO Coder fleets carrying the work.
5. Record a demonstration of CLIO Coder working with PORTUS.

Who should get in touch

Workflow system developers, HPC and cloud facility teams, and application groups whose workflows change while they run.

[Propose a collaboration](https://iowarp.ai/community/#contact) [Join the community](https://iowarp.ai/community/)

Related

## Topics, research, and demos.

- [Topic **Scientific workflows and reproducible deployment**](https://iowarp.ai/topics/scientific-workflows/)
- [Topic **HPC I/O and storage hierarchies**](https://iowarp.ai/topics/hpc-io/)
- [Research direction **Authority that travels with work** What can a delegated agent actually do?](https://iowarp.ai/research/directions/#authority)
- [Demo **DOE Genesis: SPOTTER-AI and PORTUS** Planned for 2026](https://iowarp.ai/research/demos/#demo-doe-genesis-spotter-ai-and-portus)
- [Demo **Fleet dispatch on a cluster** Planned for 2026](https://iowarp.ai/research/demos/#demo-fleet-dispatch-on-a-cluster)

06 / Sources

## Sources

1. PORTUS project description, DOE Genesis Mission, Pacific Northwest National Laboratory (Project description shared by the project team; not publicly posted)
2. [U.S. Department of Energy Genesis Mission](https://genesis.energy.gov/)
3. [PORTUS orchestrator: agentic orchestration for scientific Slurm workflows](https://gitlab.com/perflab-exact/portus/portus-orchestrator)
4. [Dataflow Performance Matcher: I/O cost prediction across storage tiers and node counts](https://gitlab.com/perflab-exact/dpm/dpm)
5. [Tang, Guo, Kougkas, Sun, Tallent. Characterizing dataflow for I/O-aware scheduling in HPC workflows. IPDPS 2026](https://doi.org/10.1109/IPDPS65963.2026.00076)
6. [CLIO Coder documentation for workers and fleets](https://coder.iowarp.ai/docs/guide/fleet-dispatch.html)

Next application · A5

## CLIO on national research systems.

[Read the next story](https://iowarp.ai/applications/national-infrastructure/) [All applications](https://iowarp.ai/applications/)
