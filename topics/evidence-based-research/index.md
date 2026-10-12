---
title: "Evidence-based autonomous research | IOWarp"
description: "What makes AI-driven research trustworthy: baselines, holdouts, confidence checks, run records, and human review, as applied in CLIO research tools."
url: https://iowarp.ai/topics/evidence-based-research/
---

> What makes AI-driven research trustworthy: baselines, holdouts, confidence checks, run records, and human review, as applied in CLIO research tools.

# Measure the claim, not the story.

Autonomous research systems propose changes and test them. Their output is only as credible as the measurement discipline behind it: a fixed baseline, repeated trials, a holdout the system did not tune against, and a record of every run.

01 The failure mode 02 How IOWarp is approaching it 03 How IOWarp approaches it 04 Common questions

01

## The failure mode

A system that generates both the change and the explanation can produce a persuasive narrative for a result that does not replicate. Evidence has to come from measurements tied to the conditions that produced them.

02

## How IOWarp is approaching it

CLIO Researcher runs a loop that proposes a change to systems code or configuration, measures candidate against baseline in alternating trials, applies confidence and holdout checks, and stages only supported improvements for human review. CLIO Bench records runs and streams them to a dashboard without issuing its own verdicts.

How IOWarp approaches it

## Where to go deeper.

01**Research tooling**

CLIO Researcher, Bench, and Author in the stack.

Continue →

<https://iowarp.ai/platform/#layer-research>

02**Results and milestones**

What the project has built, run, measured, and published.

Continue →

<https://iowarp.ai/progress/>

03**Anthropic on evaluating agents**

Further reading: Evaluating agent outcomes, tool calls, and traces with deterministic, model-based, and human graders.

Open ↗

<https://www.anthropic.com/engineering/demystifying-evals-for-ai-agents>

04**OpenAI’s evaluation flywheel**

Further reading: Diagnosing failure cases, establishing a baseline, and measuring targeted improvements.

Open ↗

<https://github.com/openai/openai-cookbook/blob/main/examples/evaluation/Building_resilient_prompts_using_an_evaluation_flywheel.md>

05**Google DeepMind’s AlphaEvolve research**

Further reading: A coding-agent research system that proposes executable candidates and scores them with automated evaluators.

Open ↗

<https://deepmind.google/blog/alphaevolve-a-gemini-powered-coding-agent-for-designing-advanced-algorithms/>

Applications that use it

- A3
  ### [Provenance and integrity for AI-driven science](https://iowarp.ai/applications/genesis-spotter/)
  A DOE Genesis Mission project at Argonne National Laboratory that traces integrity attacks on scientific AI workflows to their source. CLIO Agent provides the investigating agents.
  Project began August 2026
- A5
  ### [CLIO on national research systems](https://iowarp.ai/applications/national-infrastructure/)
  Where CLIO Core has been built and run: ALCF Aurora, DeltaAI, and the Ares cluster.
  Built and run on national systems

Common questions

## Common questions.

**Can I use CLIO Researcher now?**

Yes. CLIO Researcher is open source and listed with the research tooling on the platform page.

Related

## Research and demos on this topic.

- [Research direction **Provenance an agent can question** When a result is wrong, can we find out why?](https://iowarp.ai/research/directions/#provenance)
- [Research direction **Evidence for agentic science** What would prove an agent made progress?](https://iowarp.ai/research/directions/#evidence)
- [Demo **CLIO on DeltaAI and Aurora** Planned for 2026](https://iowarp.ai/research/demos/#demo-clio-on-deltaai-and-aurora)
- [Demo **DOE Genesis: SPOTTER-AI and PORTUS** Planned for 2026](https://iowarp.ai/research/demos/#demo-doe-genesis-spotter-ai-and-portus)

## References

1. [IEEE eScience 2026 accepted papers, including Acropolis and AgentStage](https://www.escience-conference.org/2026/papers)
2. [Yildirim et al., WisIO: Automated I/O bottleneck detection with multi-perspective views for HPC workflows, ICS 2025](https://doi.org/10.1145/3721145.3725742)
3. [Anthropic on evaluating agents](https://www.anthropic.com/engineering/demystifying-evals-for-ai-agents)
4. [OpenAI’s evaluation flywheel](https://github.com/openai/openai-cookbook/blob/main/examples/evaluation/Building_resilient_prompts_using_an_evaluation_flywheel.md)
5. [Google DeepMind’s AlphaEvolve research](https://deepmind.google/blog/alphaevolve-a-gemini-powered-coding-agent-for-designing-advanced-algorithms/)

## Other concepts

- [T1 Context management for AI agents](https://iowarp.ai/topics/context-management/)
- [T2 Scientific AI agents](https://iowarp.ai/topics/scientific-agents/)
- [T3 MCP servers for scientific computing](https://iowarp.ai/topics/mcp-for-science/)
- [T4 HPC I/O and storage hierarchies](https://iowarp.ai/topics/hpc-io/)
- [T5 Data movement for AI-infused workflows](https://iowarp.ai/topics/data-movement/)
- [T6 Scientific workflows and reproducible deployment](https://iowarp.ai/topics/scientific-workflows/)

Next step

## See this topic at work.

[Provenance and integrity for AI-driven science](https://iowarp.ai/applications/genesis-spotter/) [All concepts](https://iowarp.ai/docs/#concepts)
