# AgentLens

A zero-dependency, single-file visualizer for **Agentforce** agent plan execution traces. Paste or drop a `PlanSuccessResponse` JSON and instantly see:

- **Topic Graph** — directed graph of agent topic handoffs with transition counts
- **Per-topic FSM** — induced finite-state machine (orchestration vs tool-execution nodes) with step-through playback
- **Trace Stream** — filterable timeline of every plan step: LLM calls, tool executions, variable updates, reasoning iterations, and more
- **Graph Analysis** — degree distribution, SCC/WCC decomposition, betweenness centrality, diameter, and prose insights

## Quick Start

1. Open `index.html` in any browser (works with `file://`, no server required).
2. Click **Paste JSON** or **Upload** and provide a `PlanSuccessResponse` JSON.
3. Click a topic node to explore its FSM and trace timeline.

An example trace is included in `example/trace.json`.

## Features

| Feature | Details |
|---|---|
| Topic transitions | Ring layout with directed edges, multiplicity badges, self-loops |
| FSM playback | Prev/Next/scrub through trace events; active state highlights |
| Filters | Toggle variable updates, reasoning, node entry, enabled tools, `__` vars, `AgentScriptInternal_*` vars, full LLM bodies |
| LLM detail | System prompt, messages sent, model output, tool calls, latency |
| Function detail | Input/output JSON, execution latency |
| Graph metrics | \|V\|, \|E\|, density, SCC, WCC, diameter, betweenness centrality |
| Dark / Light mode | One-click theme toggle, preferences persist |

## Screenshot

![AgentLens](https://github.com/user-attachments/assets/placeholder)

## License

MIT
