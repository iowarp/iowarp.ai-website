---
title: "CLIO on national research systems | IOWarp"
description: "CLIO Core on ALCF Aurora, DeltaAI, and Ares, and NeuroH5 loaded through its HDF5 connector."
url: https://iowarp.ai/applications/national-infrastructure/
---

> CLIO Core on ALCF Aurora, DeltaAI, and Ares, and NeuroH5 loaded through its HDF5 connector.

# CLIO on national research systems.

A context runtime has to work where large-scale science happens. This story records where CLIO Core has been built and run, and how NeuroH5 uses it through its HDF5 connector.

Partners

Argonne Leadership Computing Facility · NCSA · The HDF Group · Illinois Tech

Status

Built and run on national systems

Stack layers

Accelerators · Storage systems · Context runtime

Components

[CLIO Core](https://iowarp.ai/platform/#core) · [Jarvis](https://iowarp.ai/platform/#jarvis) · [I/O adapters and connectors](https://iowarp.ai/platform/#adapters) · [CLIO Core GPU runtime](https://iowarp.ai/platform/#gpu-runtime) · [CLIO Kit](https://iowarp.ai/platform/#kit)

On the web

[Argonne Leadership Computing Facility ↗](https://www.alcf.anl.gov/) · [National Center for Supercomputing Applications ↗](https://www.ncsa.illinois.edu/) · [The HDF Group ↗](https://www.hdfgroup.org/) · [Illinois Institute of Technology ↗](https://www.iit.edu/) · [DeltaAI ↗](https://www.ncsa.illinois.edu/resources-and-services/compute-resources/deltaai/) · [ACCESS ↗](https://access-ci.org/) · [Gnosis project record ↗](https://grc.iit.edu/research/projects/iowarp/) · [INCITE 2026 GPU hackathon ↗](https://www.nersc.gov/news-and-events/calendar-of-events/alcf-incite-gpu-hackathon-2026) · [NeuroH5 ↗](https://github.com/iraikov/neuroh5) · [MiV-Simulator ↗](https://github.com/GazzolaLab/MiV-Simulator)

Record

What the work has produced · Sources

01 / The scientific question

## Does the same context runtime build, deploy, and scale across the national machines scientists actually use?

National systems differ in CPU architecture, accelerators, interconnect, schedulers, and file systems. DeltaAI runs Arm-based NVIDIA Grace Hopper superchips; Aurora uses Intel GPUs and schedules with PBS rather than Slurm.

A runtime that only works on the development cluster is not infrastructure. Portability, repeatable deployment, and measurements under stated conditions are the bar.

**WHERE CONTEXT BREAKS** Deployment itself is context: the scheduler, module stack, network fabric, and storage tiers of each machine. CLIO Core ships Jarvis pipelines that record those choices per system, so a run can be repeated and inspected.

02 / Workflow

## The workflow, stage by stage.

**FIG A5.1** · National infrastructure workflow 3 stages

1. **Ares · Illinois Tech**
  The development and performance-evaluation cluster where CLIO Core is built and run.
  CLIO Core · Jarvis
2. **DeltaAI · NCSA**
  NCSA’s AI system built on NVIDIA Grace Hopper superchips. The platform builds and runs there through an ACCESS allocation.
  CLIO Core
3. **Aurora · ALCF**
  Argonne’s exascale system with Intel GPUs. The Gnosis project record reports a CLIO Core port and scientific workload runs at the INCITE GPU hackathon. Public Jarvis recipes describe Aurora deployment configurations.
  CLIO Core · SYCL

Stages as the project sources describe them. What each stage has produced so far is listed in the record below.

03 / The record

## What the work has produced.

1. The Gnosis project record reports that the team ported CLIO Core to Aurora at the INCITE GPU hackathon and ran scientific workloads on the system. [1] [2] [3]
  CONDITIONS · Institutional account accompanied by public deployment recipes; independently published scaling data is not linked here.
2. CLIO Core builds and runs on the Ares cluster at Illinois Tech and on DeltaAI. [3] [4]
3. NeuroH5 was onboarded through a transfer-engine-backed HDF5 VOL connector and loads without application code changes. [5]

04 / Software in the loop

## The instruments involved.

01 / Component**CLIO Core**

Runtime, transfer engine, and HDF5 VOL connector deployed on each system.

Read more →

<https://iowarp.ai/platform/#core>

02 / Component**Jarvis pipelines**

Per-machine deployment recipes for Aurora, Delta, and other systems.

Open source ↗

<https://github.com/iowarp/clio-core/tree/v2.2.1/jarvis_clio_core/pipelines>

03 / Component**CLIO Kit · Slurm, Lmod, Jarvis**

Servers an agent can use for scheduling and environment management on such systems.

Read more →

<https://iowarp.ai/clio-kit/>

05 / What comes next

## Next steps.

1. Publish Aurora scaling data with node configuration and workload stated.
2. Publish DeltaAI transfer-engine measurements with GPU configuration, file system, and workload stated.
3. Record the 2026 demonstration of one Jarvis pipeline deploying CLIO on DeltaAI and Aurora.

Who should get in touch

Facility staff, allocation holders, and application teams on ACCESS and DOE systems who want a context runtime measured on their machines.

[Propose a collaboration](https://iowarp.ai/community/#contact) [Join the community](https://iowarp.ai/community/)

Related

## Topics, research, and demos.

- [Topic **HPC I/O and storage hierarchies**](https://iowarp.ai/topics/hpc-io/)
- [Topic **Data movement for AI-infused workflows**](https://iowarp.ai/topics/data-movement/)
- [Topic **MCP servers for scientific computing**](https://iowarp.ai/topics/mcp-for-science/)
- [Topic **Scientific workflows and reproducible deployment**](https://iowarp.ai/topics/scientific-workflows/)
- [Topic **Evidence-based autonomous research**](https://iowarp.ai/topics/evidence-based-research/)
- [Demo **CLIO on DeltaAI and Aurora** Planned for 2026](https://iowarp.ai/research/demos/#demo-clio-on-deltaai-and-aurora)

06 / Sources

## Sources

1. [Gnosis Research Center IOWarp project record](https://grc.iit.edu/research/projects/iowarp/)
2. [NERSC event record: ALCF INCITE GPU Hackathon, April 28–30, 2026](https://www.nersc.gov/news-and-events/calendar-of-events/alcf-incite-gpu-hackathon-2026)
3. [CLIO Core Jarvis deployment pipelines for Aurora, Delta, and other systems](https://github.com/iowarp/clio-core/tree/v2.2.1/jarvis_clio_core/pipelines)
4. [DeltaAI system at NCSA](https://www.ncsa.illinois.edu/resources-and-services/compute-resources/deltaai/)
5. [CLIO Core source repository](https://github.com/iowarp/clio-core)

Next application · A6

## GPU direct I/O and compression.

[Read the next story](https://iowarp.ai/applications/gpu-data-movement/) [All applications](https://iowarp.ai/applications/)
