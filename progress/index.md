---
title: "Results and milestones | IOWarp"
description: "What IOWarp has built, run, and published since 2024, what comes next, and where the figures behind each result are published."
url: https://iowarp.ai/progress/
---

> What IOWarp has built, run, and published since 2024, what comes next, and where the figures behind each result are published.

# Results and milestones.

For reviewers, collaborators, and anyone evaluating the work: what the project has built, run, and published since 2024, and what comes next. Results are stated in plain words with their sources. The figures behind them live with their conditions in papers, release notes, and the project documentation listed at the end of this page.

Timeline

So far, and ahead

Results

What the work has shown

Updated

12 October 2026

01 / Timeline

## So far, and ahead.

### So far

1. Aug 2024 to Jul 2025
  #### Foundations
    - The IOWarp project begins, building on years of systems research at the Gnosis Research Center.
    - The core architecture, the first scientific MCP servers, the OMNI ingestion format, and the Jarvis deployment framework are in place.
      [1]
      [2]
      [3]
    - The integrated IOWarp beta is presented to research cyberinfrastructure teams in Denver.
      [4]
2. Sep 2025 to Feb 2026
  #### Agents on scientific data
    - Agents are recorded in public working on EarthScope, LAMMPS, ParaView, ADIOS2, and Slurm workflows.
      [5]
      [6]
    - Two posters at IEEE eScience 2025 cover agent workflows and GPUDirect data transfer.
      [6]
      [7]
    - CLIO Core has its first public release series.
      [1]
3. Mar 2026 to Jul 2026
  #### One platform
    - The Gnosis project record reports that the team ported CLIO Core to Aurora at the INCITE GPU hackathon and ran scientific workloads there.
      [8]
      [9]
      [10]
    - A major CLIO Core release brings the context transfer and assimilation engines under the CLIO name.
      [1]
4. Aug 2026 to Sep 2026
  #### Science partnerships
    - The team joins two DOE Genesis Mission projects, SPOTTER-AI at Argonne and PORTUS at PNNL.
      [11]
    - A coordinated release across CLIO Core, Kit, Agent, CLIO Coder, and Relay adds the Spotter approval mode to CLIO Agent.
      [12]
    - Materio ships in CLIO Coder and wtf-MS reaches its first stable release.
      [13]
      [14]

### Ahead

1. Nov 2026 to Summer 2027
  #### Launch and validation
    - IOWarp and the CLIO platform soft launch at SC26 in Chicago, November 15–20, 2026, with workshop presentations, research posters, a conference paper, and an HDF5 birds-of-a-feather session.
      [15]
    - The Technical Advisory Board forms at the end of November 2026, after SC26.
    - The Utah materials workflow runs end to end on IOWarp, new HDF5 applications are onboarded, and CLIO Agent consumes wtf-MS.
    - CLIO Core gets broader resilience testing under node failures, deeper integration with inference engines such as llama.cpp, vLLM, and SGLang, and federation across sites.
2. Autumn 2027 onward
  #### Scale and adoption
    - Performance modeling and full-stack optimization reach across the platform.
    - A stable platform release.

02 / Results

## What the work has shown.

- 01
  ### [National research systems](https://iowarp.ai/applications/national-infrastructure/)
  The Gnosis project record reports that the team ported CLIO Core to Aurora at the INCITE GPU hackathon and ran scientific workloads there. This is an institutional account, accompanied by public Aurora deployment recipes; independently published scaling data is not linked here. It builds and runs on DeltaAI and on the Ares cluster at Illinois Tech.
  NeuroH5 was onboarded through a transfer-engine-backed HDF5 VOL connector without application code changes.
  Sources [8] [10] [16] [1]
- 02
  ### [Agents on scientific data](https://iowarp.ai/applications/national-data-platform/)
  With IOWarp context, an agent completed EarthScope data retrieval and visualization through the National Data Platform, where a comparison agent without that context did not.
  Agent-assisted LAMMPS analysis and IOR deployment finished faster than the same tasks done by hand, across several agent and model combinations. The IEEE eScience 2025 poster states the models, prompts, and timings.
  Sources [6] [17]
- 03
  ### [Data movement and GPUs](https://iowarp.ai/applications/gpu-data-movement/)
  GPU kernels submit I/O to CLIO without exiting the kernel, and a workflow-aware compression system chooses a codec for the data at hand. Both are in the CLIO Core source builds.
  The team also characterized GPUDirect data transfer through NVIDIA NIXL for AI workloads.
  Sources [18] [7]
- 04
  ### [Applications and partnerships](https://iowarp.ai/applications/)
  The University of Utah team released the InfiniteScienceGym benchmark. wtf-MS and its CLIO Coder port, Materio, carry materials research planning.
  For SPOTTER-AI, CLIO Agent added the Spotter approval mode, and a read-only provenance MCP server in the agent marketplace was qualified against Flowcept and CMF. For PORTUS, the IOWarp team works on workflow motifs and performance models.
  Sources [13] [19] [12] [20] [21]

03 / Where the figures live

## Where results live.

This site tells the story of the project. Numbers need their machine, workload, baseline, and version beside them, so they are published where those conditions can be kept: in the papers, in each component’s release notes, and on the project documentation sites.

### Project documentation

- [CLIO Core documentation](https://core.iowarp.ai/docs/index.html)
  Installation, the Python API, storage composition, data operators, and the runtime dashboard.
- [CLIO Agent guides](https://clio.iowarp.ai/docs/)
  Installation, model connections, sessions, and marketplace tools.
- [CLIO Kit guides](https://toolkit.iowarp.ai/docs/intro)
  Scientific tools, selective installation, and workflow plugins.
- [CLIO Coder guides](https://coder.iowarp.ai/docs.html)
  Installation, fleets, run receipts, and context continuity.

### Papers and posters

- [IEEE eScience 2025 agent workflow poster](http://cs.iit.edu/~scs/assets/files/islam2025aidriven_poster.pdf)
  Models, prompts, and timings for the EarthScope, LAMMPS, and IOR workflows.
- [NIXL characterization, IEEE eScience 2025](https://doi.org/10.1109/eScience65000.2025.00075)
  GPUDirect data transfer through NIXL for AI workloads.
- [Publications and posters](https://iowarp.ai/research/)
  The full research record.

### Release notes

[CLIO Core releases](https://github.com/iowarp/clio-core/releases) [CLIO Kit releases](https://github.com/iowarp/clio-kit/releases) [CLIO Agent releases](https://github.com/iowarp/clio-agent/releases) [CLIO Coder releases](https://github.com/iowarp/clio-coder/releases) [CLIO Relay releases](https://github.com/iowarp/clio-relay/releases) [GACT and Agent Workspace releases](https://github.com/iowarp/gact-tui/releases) [Agent marketplace releases](https://github.com/iowarp/clio-agent-marketplace/releases) [CLIO Web Search releases](https://github.com/iowarp/clio-web-search/releases) [Materio and wtf-MS releases](https://github.com/iowarp/wtf-ms/releases)

04 / Sources

## Sources

Every source links to its public page. A source without one says what it is.

1. [CLIO Core source repository](https://github.com/iowarp/clio-core)
2. [CLIO Kit source repository](https://github.com/iowarp/clio-kit)
3. Cernuda et al., Jarvis: Towards a shared, user-friendly, and reproducible I/O infrastructure, PDSW 2024 work-in-progress session (Work-in-progress presentation)
4. [IOWarp poster, Denver, July 2025 (figshare)](https://doi.org/10.6084/m9.figshare.29647613.v1)
5. [Agent examining EarthScope data through the National Data Platform (video, October 2025)](https://www.youtube.com/watch?v=9NUf76wnHhA)
6. [Islam, Cernuda, Muradli, Kougkas, Sun. Towards an AI-driven scientific workflow. IEEE eScience 2025 (poster)](https://doi.org/10.1109/eScience65000.2025.00074)
7. [Muradli, Ye, Logan, Kougkas, Sun. Insights into GPUDirect data transfer through NIXL benchmarking. IEEE eScience 2025 (poster and extended abstract)](https://doi.org/10.1109/eScience65000.2025.00075)
8. [Gnosis Research Center IOWarp project record](https://grc.iit.edu/research/projects/iowarp/)
9. [NERSC event record: ALCF INCITE GPU Hackathon, April 28–30, 2026](https://www.nersc.gov/news-and-events/calendar-of-events/alcf-incite-gpu-hackathon-2026)
10. [CLIO Core Jarvis deployment pipelines for Aurora, Delta, and other systems](https://github.com/iowarp/clio-core/tree/v2.2.1/jarvis_clio_core/pipelines)
11. [U.S. Department of Energy Genesis Mission](https://genesis.energy.gov/)
12. [CLIO Agent changelog, including the Spotter approval mode](https://github.com/iowarp/clio-agent/blob/v0.9.4.24/CHANGELOG.md)
13. [wtf-MS materials research planning system](https://github.com/iowarp/wtf-ms)
14. [Materio materials research workflow in the CLIO Coder library](https://github.com/iowarp/clio-coder/tree/main/library/plugins/materio)
15. [SC26: The International Conference for High Performance Computing, Networking, Storage, and Analysis, Chicago, November 15–20, 2026](https://sc26.supercomputing.org/)
16. [DeltaAI system at NCSA](https://www.ncsa.illinois.edu/resources-and-services/compute-resources/deltaai/)
17. [eScience 2025 poster PDF: EarthScope, LAMMPS, ParaView, and IOR agent workflows](http://cs.iit.edu/~scs/assets/files/islam2025aidriven_poster.pdf)
18. [CLIO Core GPU, compression, and cuFile adapter sources](https://github.com/iowarp/clio-core/tree/v2.3.1/context-transfer-engine/adapter)
19. [Bentham and Srikumar. InfiniteScienceGym: An unbounded, procedurally generated benchmark for scientific analysis. COLM 2026 (arXiv:2604.13201)](https://arxiv.org/abs/2604.13201)
20. [CLIO Agent design note: unified Spotter provenance MCP server](https://github.com/iowarp/clio-agent/blob/v0.9.4.24/docs/design/unified-spotter-provenance-mcp-2026-08.md)
21. [Dataflow Performance Matcher: I/O cost prediction across storage tiers and node counts](https://gitlab.com/perflab-exact/dpm/dpm)

Next step

## See each result in its science.

[Read the application stories](https://iowarp.ai/applications/) [IOWarp at SC26](https://iowarp.ai/community/#sc26)
