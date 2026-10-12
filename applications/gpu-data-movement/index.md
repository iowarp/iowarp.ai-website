---
title: "GPU direct I/O and compression | IOWarp"
description: "How CLIO Core reaches into the GPU: CUDA kernels that issue I/O to IOWarp, payload offload to host memory and NVMe, and GPU compression."
url: https://iowarp.ai/applications/gpu-data-movement/
---

> How CLIO Core reaches into the GPU: CUDA kernels that issue I/O to IOWarp, payload offload to host memory and NVMe, and GPU compression.

# GPU direct I/O and compression.

Accelerators changed where scientific data has to be. CLIO Core now reaches into the GPU: kernels submit I/O to IOWarp without leaving the device, GPU-resident data spills to host memory and NVMe, and data can be compressed on the GPU before it moves. The research builds on NVIDIA technologies such as CUDA, cuFile, NIXL, and nvCOMP.

Partners

Illinois Tech Gnosis Research Center · Argonne co-authors on KV-cache research

Status

Research thread across the stack

Stack layers

Accelerators · Operating system · Storage systems · Context runtime

Components

[CLIO Core GPU runtime](https://iowarp.ai/platform/#gpu-runtime) · [GPU compression](https://iowarp.ai/platform/#gpu-compression) · [Direct GPU I/O research](https://iowarp.ai/platform/#gpu-direct) · [GPU–NVMe bridge](https://iowarp.ai/platform/#gnb) · [Linux I/O backends](https://iowarp.ai/platform/#os-io) · [Tiered block devices](https://iowarp.ai/platform/#tiers) · [CLIO Core](https://iowarp.ai/platform/#core)

On the web

[Illinois Institute of Technology ↗](https://www.iit.edu/) · [Argonne National Laboratory ↗](https://www.anl.gov/) · [NVIDIA NIXL ↗](https://github.com/ai-dynamo/nixl) · [NVIDIA nvCOMP ↗](https://developer.nvidia.com/nvcomp)

Record

What the work has produced · Sources

01 / The scientific question

## Can scientific data move to and from GPU memory as a first-class tier, without a detour through the CPU?

AI-infused workflows compute on GPUs but still read and write through the host: the kernel ends, the CPU copies, the file system writes, and the GPU waits. Every bounce costs bandwidth and time.

Model memory has the same shape. The KV cache of LLM inference grows with context length and overflows GPU memory, turning inference into a storage-hierarchy problem.

**WHERE CONTEXT BREAKS** The question is the one IOWarp asks at every tier: which data must be next to compute now, and which can wait somewhere cheaper. On a GPU, answering it takes I/O primitives that run inside the kernel and placement that treats GPU memory as the top of the hierarchy.

02 / Workflow

## The workflow, stage by stage.

**FIG A6.1** · Accelerated computing workflow 4 stages

1. **Issue I/O from the GPU**
  GPU-side primitives let CUDA, ROCm, and SYCL kernels submit work to CLIO without exiting the kernel.
  CLIO Core GPU runtime
2. **Offload payloads**
  GPU-resident vectors are backed by transfer-engine storage, with a GPU and host-memory page cache that spills to NVMe and brings data back on demand.
  GPU vector · block devices
3. **Compress on the device**
  nvCOMP, cuSZ, cuSZp, ndzip, and ZFP for SYCL shrink data before it moves; a dynamic system chooses the method for the workflow.
  CLIO compression
4. **Remove the CPU hop**
  Current source builds provide NVIDIA cuFile and NIXL paths. Earlier research explored a BaM-style GPU page cache and a Linux kernel module that gave GPUs their own NVMe queues; those prototypes remain in archived source.
  GPU I/O · archived prototypes

Stages as the project sources describe them. What each stage has produced so far is listed in the record below.

03 / The record

## What the work has produced.

1. Primitives let GPU kernels submit I/O commands to CLIO without exiting the kernel, and a dynamic compression system chooses a method for the workflow. [1]
  CONDITIONS · Source builds only
2. CLIO Core includes GPU-resident vectors, GPU compression backends, a cuFile adapter, and NIXL transport support in its source builds. [1]
  CONDITIONS · Optional source builds; GPU validation depends on the backend and some tests remain opt-in
3. Characterization of GPUDirect data transfer through NVIDIA NIXL for AI workloads. [2]
4. Related team research with Argonne collaborators treats the LLM KV cache as a tier: PKAS schedules inference with the cache in view, and PagedEviction prunes cache blocks for long contexts. [3] [4]

04 / Software in the loop

## The instruments involved.

01 / Component**CLIO Core · GPU extensions**

GPU runtime, GPU vectors, GPU compression, and cuFile and NIXL adapters, in CUDA, ROCm, and SYCL source builds.

Open source ↗

<https://github.com/iowarp/clio-core>

02 / Component**The CLIO stack**

How the accelerator and operating-system layers fit under the runtime.

Read more →

<https://iowarp.ai/platform/#layer-gpu>

03 / Component**Publications**

NIXL characterization and KV-cache research.

Read more →

<https://iowarp.ai/research/>

05 / What comes next

## Next steps.

1. Publish GPU offload measurements with GPU model, interconnect, storage, and workload stated.
2. Bring GPU tests into continuous integration on GPU runners.
3. Record the 2026 demonstration of GPU payload offload with CLIO Core CUDA kernels.

Who should get in touch

GPU systems researchers, inference-serving teams, and facilities with GPU-attached NVMe or GPUDirect-capable storage.

[Propose a collaboration](https://iowarp.ai/community/#contact) [Join the community](https://iowarp.ai/community/)

Related

## Topics, research, and demos.

- [Topic **Data movement for AI-infused workflows**](https://iowarp.ai/topics/data-movement/)
- [Topic **Context management for AI agents**](https://iowarp.ai/topics/context-management/)
- [Topic **HPC I/O and storage hierarchies**](https://iowarp.ai/topics/hpc-io/)
- [Research direction **The GPU as a storage tier** Can data reach GPU memory without a detour through the CPU?](https://iowarp.ai/research/directions/#gpu-tier)
- [Research direction **Memory as a storage hierarchy** Which facts belong hot, durable, or replayable?](https://iowarp.ai/research/directions/#memory-hierarchy)
- [Demo **GPU payload offload** Planned for 2026](https://iowarp.ai/research/demos/#demo-gpu-payload-offload)

06 / Sources

## Sources

1. [CLIO Core GPU, compression, and cuFile adapter sources](https://github.com/iowarp/clio-core/tree/v2.3.1/context-transfer-engine/adapter)
2. [Muradli, Ye, Logan, Kougkas, Sun. Insights into GPUDirect data transfer through NIXL benchmarking. IEEE eScience 2025 (poster and extended abstract)](https://doi.org/10.1109/eScience65000.2025.00075)
3. [Ye, Maurya, Chitty-Venkata, Nicolae, Kougkas, Sun. PKAS: Predictive KVCache-aware scheduling for faster LLM and transformer inferences. HPDC 2026](https://doi.org/10.1145/3806645.3807819)
4. [Chitty-Venkata, Ye, Raskar, Kougkas, Sun, Emani, Vishwanath, Nicolae. PagedEviction: Structured block-wise KV cache pruning for efficient LLM inference. Findings of EACL 2026](https://doi.org/10.18653/v1/2026.findings-eacl.168)

Next application · A1

## Agents in the materials workflow.

[Read the next story](https://iowarp.ai/applications/materials-science/) [All applications](https://iowarp.ai/applications/)
