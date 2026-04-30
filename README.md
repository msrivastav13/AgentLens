# AgentLens

Understand what your Agentforce agent actually did — visually.

**Try it now:** <https://msrivastav13.github.io/AgentLens/>

![AgentLens](images/output.png)

## What it does

Load a trace from the **Agentforce DX** extension and AgentLens shows you:

- **Agent Graph** — which sub agents talked to each other, how many times, and in what order
- **Finite State Machine** — the internal orchestration flow for each sub agent: LLM calls, tool executions, variable mutations, and handoffs
- **Step-by-Step Inspector** — walk through every event with full detail: system prompts, model output, tool inputs/outputs, and variable diffs
- **Graph Analysis Report** — one-click PDF with degree distribution, connectivity analysis, betweenness centrality, and algorithm explanations

## Quick Start

1. Open <https://msrivastav13.github.io/AgentLens/> (or `index.html` locally — no server required)
2. Paste or upload the plan response JSON from the Agentforce DX extension
3. Click a sub agent to explore its state machine and step through the trace

## Why

Agentforce traces are large JSON blobs. Reading them raw is painful. AgentLens turns them into something you can actually navigate — so you can debug handoff loops, understand why an LLM chose a tool, or figure out where latency is hiding.

Zero dependencies. Runs entirely in the browser. Works offline.

## License

MIT
