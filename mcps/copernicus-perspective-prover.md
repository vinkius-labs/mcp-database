# Copernicus Perspective Prover MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/copernicus-perspective-prover)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [architecture](../categories/architecture.md)

Your AI analyzed the problem from the default perspective and added workarounds when it did not fit. That is an epicycle — not a solution. Copernicus did not add more epicycles to Ptolemy's model. He moved the center from Earth to Sun. 40+ epicycles vanished. This tool forces default questioning, epicycle counting, alternative framing, observer shifting, and simplicity comparison.

## Description
AI agents accept the default perspective and add workarounds when it fails. They never question whether the frame itself is wrong.

### The Problem

- **Default Locked** — 'The obvious approach is...' Why is it obvious? Because it is the default. For 1,400 years, geocentrism was 'obvious.' Copernicus asked: 'What if Earth is NOT the center?'
- **Epicycles Ignored** — 'We can work around that with a special case.' How many special cases do you have? Ptolemy needed 40+ epicycles. Each was 'reasonable.' Together they signaled a broken model. Count them.
- **No Alternative Frame** — 'There is no other way.' Copernicus spent 30 years developing the alternative while the entire establishment insisted there was no other way. What frame have you NOT considered?
- **Observer Fixed** — 'From our perspective, the data shows...' Move the observer. Copernicus moved to the Sun: retrograde motion became simple geometry. Same planets, radically different explanation.
- **Simplicity Uncompared** — 'The new approach is obviously better.' Obviously? Count the workarounds in both frames. Copernicus: 40+ epicycles vs. elliptical orbits. Numbers, not adjectives.

### How It Works

1. **defaultQuestioned** — Current perspective identified and challenged.
2. **epicyclesCounted** — Accumulated workarounds counted as model-failure signals.
3. **alternativeFrameConsidered** — Fundamentally different frame proposed.
4. **observerMoved** — Same data reanalyzed from the new position.
5. **simplicityCompared** — Old vs. new complexity measured with counts.

### Verdict Matrix

| Pivot | Verdict | Meaning |
|---|---|---|
| defaultQuestioned = false | DEFAULT_LOCKED | Analyzing from unquestioned default. |
| epicyclesCounted = false | EPICYCLES_IGNORED | Workarounds not recognized as signals. |
| alternativeFrameConsidered = false | NO_ALTERNATIVE_FRAME | Criticism without alternative. |
| observerMoved = false | OBSERVER_FIXED | New frame described but not used. |
| simplicityCompared = false | SIMPLICITY_UNCOMPARED | No measurable comparison. |
| All pass | PERSPECTIVE_PROVEN | Frame shifted. Epicycles eliminated. |


## Available Tools
- **validate_copernicus_perspective**: Think like Copernicus — the most important scientific revolution was not discovering new data, it was looking at the SAME data from a different position. You must: (1) QUESTION THE DEFAULT — identify the assumed perspective, trace its origin (evidence vs convention vs authority vs habit), and calculate the complexity cost it forces. "The obvious approach" is the most dangerous phrase — geocentrism was obvious for 14 centuries, (2) COUNT EPICYCLES — list every workaround, exception, and special case needed to keep the current model working. Each workaround is a signal, not an edge case. Ptolemy needed 40+ epicycles — each was "reasonable," together they were a symptom. If you have 5+ workarounds, you likely have a broken model, not a complex domain, (3) PROPOSE ALTERNATIVE FRAME — describe a fundamentally different reference point. Not a tweak to the current model — a different CENTER. Copernicus did not add a better epicycle, he moved the Sun to the center. What would change if you moved your center?, (4) MOVE THE OBSERVER — reanalyze the SAME data from the new position. Do not describe the new frame — USE it. What patterns become visible from the new vantage point that were hidden before? Copernicus: retrograde motion became simple geometry. Same planets, different explanation, (5) COMPARE SIMPLICITY — count workarounds in BOTH frames. Not "obviously simpler" — measure: how many exceptions does each frame need? What new complexity does the alternative introduce? Is the tradeoff worth it? Count, do not assert. If rejected, you are locked in the current frame without examining alternatives.

Structured reflection tool for Copernican perspective shifts — questioning default frames by counting accumulated workarounds as model-failure signals. Forces the agent to identify the assumed perspective, count its epicycles (patches that keep a broken model alive), propose a fundamentally different reference frame, reanalyze from the new position, and compare complexity measurably. Catches Default Lock (accepting the current framework as "obvious" without questioning its origin — geocentrism was "obvious" for 1,400 years), Epicycle Blindness (treating 5+ workarounds as "edge cases" instead of recognizing them as symptoms of a broken model), Tweak Addiction (proposing "improvements" to the current frame instead of a fundamentally different center — another epicycle, not heliocentrism), Observer Fixation (describing the alternative frame without actually reanalyzing data from the new position), and Simplicity Assertion ("obviously better" without counting workarounds in both frames). Call once per framework evaluation or when accumulated workarounds exceed 3


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Copernicus Perspective Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "We should keep our monolithic architecture. It is the obvious approach for our team size and the standard way works well enough."

**🤖 AI Agent:**
> DEFAULT_LOCKED — 'The obvious approach' and 'the standard way' are default-locked language. WHY is monolithic the default? Because it is familiar? Because of team size? Copernicus: 'obvious' is what geocentrism was for 1,400 years. What workarounds have you accumulated? How many special cases? Are they growing? Ptolemy needed 40+ epicycles — each was 'reasonable.' Together they signaled a broken model. Count yours.

---

**👤 You:**
> "We use REST APIs everywhere but keep adding workarounds for real-time features — polling, webhooks, SSE adapters. There is no other way to handle our client integrations."

**🤖 AI Agent:**
> NO_ALTERNATIVE_FRAME — Default questioned: good — REST identified as convention. Epicycles counted: polling, webhooks, SSE adapters — three workarounds for what should be native behavior. But 'there is no other way' is frame rigidity. Copernicus heard the same from every university in Europe for 30 years. You PROPOSED event-driven but immediately dismissed it. Move the observer FIRST: how do the same client integrations look from an event-driven center? What if clients consume events instead of polling REST? Analyze from the new position before dismissing.

---

**👤 You:**
> "Our caching layer keeps growing with invalidation rules. Every new feature needs a new cache-busting strategy. Should we add Redis Streams to handle the latest requirement?"

**🤖 AI Agent:**
> EPICYCLES_IGNORED — 'Every new feature needs a new cache-busting strategy' — that is the epicycle signal. Ptolemy added a new epicycle for every planetary anomaly. You are adding a new invalidation rule for every feature. Count them: how many invalidation strategies exist today? Are they growing with each release? Redis Streams is ANOTHER epicycle on top of a model that may be fundamentally wrong. What if caching is not the right frame? What if the data model itself — if restructured — eliminates the need for most caching? Move the observer: look at this from the data consistency perspective, not the performance perspective.


## ❓ FAQ

**Q: How is this different from the Einstein Thought Experiment Prover?**
Einstein changes the RULES — 'what if you rode a light beam?' He explores hypothetical scenarios by modifying physical laws. Copernicus changes the POSITION — 'what if the center is different?' He reframes existing reality from a different vantage point. Einstein creates new physics. Copernicus reorganizes existing observations.

**Q: What is an 'epicycle' in a business context?**
A workaround, exception, or special case added to make the current model work despite evidence it is wrong. 'We can work around that,' 'just add a flag for this case,' 'one more exception.' Ptolemy added 40+ epicycles to geocentrism. Each was logical. Together they proved the model was wrong. Count your workarounds — when they accumulate, the model needs replacing, not patching.

**Q: Can I use this when I am satisfied with the current approach?**
Especially then. Satisfaction with the current approach IS the default-lock. The geocentrists were satisfied for 1,400 years. The tool does not force you to change — it forces you to CHECK. If the current frame has few workarounds and the alternative is more complex, the verdict confirms: PERSPECTIVE_PROVEN with the old frame validated.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/copernicus-perspective-prover](https://vinkius.com/mcp/copernicus-perspective-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Copernicus Perspective Prover** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `copernicus-perspective-prover` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Copernicus Perspective Prover** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "copernicus-perspective-prover": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
