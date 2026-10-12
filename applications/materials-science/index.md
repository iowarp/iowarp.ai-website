---
title: "Agents in the materials workflow | IOWarp"
description: "How IOWarp brings agents into a materials workflow that runs from design on HPC to X-ray tomography and fatigue testing."
url: https://iowarp.ai/applications/materials-science/
---

> How IOWarp brings agents into a materials workflow that runs from design on HPC to X-ray tomography and fatigue testing.

# Agents in the materials workflow.

The University of Utah team is IOWarp’s primary domain science partner. It contributes materials science workflows and AI research, and those workflows show what the stack has to carry, from a designed part to a defensible account of how it fails.

Partners

University of Utah · Illinois Tech · The HDF Group

Status

Active collaboration

Stack layers

Storage systems · Context runtime · Agents and tools · Applications

Components

[I/O adapters and connectors](https://iowarp.ai/platform/#adapters) · [CLIO Core](https://iowarp.ai/platform/#core) · [CLIO Kit](https://iowarp.ai/platform/#kit) · [CLIO Coder](https://iowarp.ai/platform/#coder) · [Materio and wtf-MS](https://iowarp.ai/platform/#materio)

On the web

[University of Utah ↗](https://www.utah.edu/) · [Illinois Institute of Technology ↗](https://www.iit.edu/) · [The HDF Group ↗](https://www.hdfgroup.org/) · [InfiniteScienceGym ↗](https://infinitesciencegym.github.io/) · [Utah Mechanical Engineering ↗](https://www.mech.utah.edu/) · [Utah Kahlert School of Computing ↗](https://www.cs.utah.edu/)

Record

What the work has produced · Sources

01 / The scientific question

## Can an AI agent carry a materials study from design to simulation to characterization without losing track of the part, the process, and the data?

A modern materials study crosses many systems. The Utah team’s reference workflow comes from a University of Utah and Purdue University study of fatigue in topology-optimized, additively manufactured metal parts. It joins computational design, manufacturing, characterization, and mechanical analysis into one research pipeline.

Three sub-workflows carry it: topology optimization with Abaqus and Tosca on HPC; X-ray computed tomography of the printed specimens, with image segmentation in Dragonfly; and materials data management that ties design, process, and measurement together. Each runs on different software, machines, and instruments.

**WHERE CONTEXT BREAKS** A tomography volume is only useful next to the build parameters and the simulation that predicted where the part would crack, yet those live in different places and often only in people’s notebooks. When the Utah team gave an agent domain skills for Abaqus, it could read the models and reason about them, but it could not yet submit, monitor, and retrieve jobs on a remote HPC system. Closing that gap, and keeping one record of each part across every stage, is the stack’s job.

02 / Workflow

## The workflow, stage by stage.

**FIG A1.1** · Materials science workflow 4 stages

1. **Design on HPC**
  Topology optimization in Abaqus and Tosca. Agent skills built by the materials team let a model interpret Abaqus models and generate simulation configurations.
  Abaqus skills · CLIO Kit · CLIO Core
2. **Build and characterize**
  Printed specimens are imaged by X-ray computed tomography and segmented. Volumes are meant to enter the runtime from local file systems or Globus collections, with their metadata attached.
  CLIO Core assimilation
3. **Keep one record**
  Simulation inputs, outputs, and experimental metadata form one consistent record of each part’s design and processing history, the layer an agent needs to reason across stages.
  CLIO Core · HDF5
4. **Plan the next study**
  A materials question becomes a synthesis of the supplied literature, a map of the laboratory actually available, and an assumption-checked research plan with a reviewed paper handoff.
  wtf-MS · Materio

Stages as the project sources describe them. What each stage has produced so far is listed in the record below.

**FIG A1.2** · The reference workflow Source: Utah reference workflow

The reference materials workflow and where CLIO fits. A diagram of the target workflow, not a measured run.

03 / The record

## What the work has produced.

1. wtf-MS, a research-planning framework for materials science created by Daisy Quach at the University of Utah, with guardrail and verification scripts from The HDF Group, reached its first stable release and ships in CLIO Coder as Materio. [1] [2]
2. InfiniteScienceGym, a procedurally generated benchmark for scientific data analysis from the University of Utah team, found that current proprietary and open-weight models still fall well short on its question-answering task. The public leaderboard carries the scores. [3] [4]
  CONDITIONS · COLM 2026
3. CLIO Core’s assimilation engine ingests from Globus endpoints or local file systems without application code changes, the path characterization data is meant to take into the runtime. [5]
  CONDITIONS · Globus ingestion is a source-build option

04 / Software in the loop

## The instruments involved.

01 / Component**CLIO Core**

Assimilation from local and Globus sources, tiered placement, and the shared data record.

Read more →

<https://iowarp.ai/platform/#core>

02 / Component**CLIO Kit**

HDF5, Parquet, ParaView, and Slurm tools an agent uses on intermediate data and jobs.

Read more →

<https://iowarp.ai/clio-kit/>

03 / Component**wtf-MS**

The materials research-planning workflow for Claude Code, under the MIT license.

Open source ↗

<https://github.com/iowarp/wtf-ms>

04 / Component**Materio in CLIO Coder**

The same workflow for CLIO Coder, in its plugin library.

Open source ↗

<https://github.com/iowarp/clio-coder/tree/main/library/plugins/materio>

05 / What comes next

## Next steps.

1. Integrate wtf-MS so CLIO Agent can use it directly.
2. Run the reference workflow end to end on IOWarp and test it for repeatability against the original, manual study.
3. Extend agent support from topology optimization to tomography characterization and materials data management.
4. Bring InfiniteScienceGym into IOWarp so users can benchmark scientific agents on their own questions.

Who should get in touch

Materials groups with simulation, manufacturing, or characterization pipelines, facility data teams, and anyone whose workflow crosses more instruments and machines than one person can track.

[Propose a collaboration](https://iowarp.ai/community/#contact) [Join the community](https://iowarp.ai/community/)

Related

## Topics, research, and demos.

- [Topic **Scientific workflows and reproducible deployment**](https://iowarp.ai/topics/scientific-workflows/)
- [Topic **Scientific AI agents**](https://iowarp.ai/topics/scientific-agents/)
- [Topic **Data movement for AI-infused workflows**](https://iowarp.ai/topics/data-movement/)
- [Research direction **Evidence for agentic science** What would prove an agent made progress?](https://iowarp.ai/research/directions/#evidence)
- [Demo **Materio for materials research** Planned for 2026](https://iowarp.ai/research/demos/#demo-materio-for-materials-research)

06 / Sources

## Sources

1. [wtf-MS materials research planning system](https://github.com/iowarp/wtf-ms)
2. [Materio materials research workflow in the CLIO Coder library](https://github.com/iowarp/clio-coder/tree/main/library/plugins/materio)
3. [Bentham and Srikumar. InfiniteScienceGym: An unbounded, procedurally generated benchmark for scientific analysis. COLM 2026 (arXiv:2604.13201)](https://arxiv.org/abs/2604.13201)
4. [InfiniteScienceGym public leaderboard](https://infinitesciencegym.github.io/)
5. [CLIO Core Globus materials-science assimilation test](https://github.com/iowarp/clio-core/tree/v2.3.1/context-assimilation-engine/test/integration/globus_matsci)

Next application · A2

## Agents on the National Data Platform.

[Read the next story](https://iowarp.ai/applications/national-data-platform/) [All applications](https://iowarp.ai/applications/)
