# Diagrams MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/diagrams)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Turn text into diagrams — flowcharts, UML, graphs and charts — rendered from Mermaid, PlantUML, D2 and more, with no key.

## Description
Connect any AI agent to the public **Kroki** and **mermaid.ink** rendering services and let it produce real diagrams — the kind that go into a design doc, a slide, a ticket or a README. No key, no account.

### What you can do

- **See what is possible** — nine diagram languages, each with a one-line description of what it is good for, and the output formats it supports
- **Get a working starter** — a minimal, valid example in any language, already rendered, ready to edit
- **Validate before you commit** — check that source parses, with the renderer's own error message when it does not
- **Render to SVG or PNG** — returns the shareable URL, and for SVG the markup itself, ready to paste into an HTML page, a doc or a slide
- **Render Mermaid to PNG** — a second renderer for the raster PNG that slides, chat and some wikis need

### Why it matters

A design doc that says "the flow is A then B then C" makes the reader draw it. This draws it. The agent writes the diagram source, gets back a URL that serves the image forever, and the reader sees the picture.

### Languages

mermaid (flowcharts, sequence, Gantt), plantuml (full UML), graphviz (DOT), d2, excalidraw (hand-drawn), ditaa (ASCII art), nomnoml (compact UML), vega (charts from JSON), wavedrom (timing waveforms).


## Available Tools (5)
- **get_diagram_example**: Use it to learn the syntax or as a skeleton to edit. Supports the same names as list_diagram_types.

Get a working starter snippet for one diagram language
- **list_diagram_types**: It lists every renderer (mermaid, plantuml, graphviz, d2, excalidraw, ditaa, nomnoml, erd, vega_lite, wavedrom) with a one-line description of what each is good for, plus the svg and png output formats. Everything renders through the public Kroki service with no key.

List the diagram languages and output formats this server can render
- **render_diagram**: Pass the source and the language; get back a public URL that serves the rendered image, plus — for svg — the markup itself, ready to paste into an HTML page, a doc or a slide. Output defaults to svg; choose png only where svg is not accepted. If the source does not parse, the error names the line; call get_diagram_example for a working starter. The URL is deterministic: the same source always yields the same image, so it is safe to embed permanently.

Render diagram source to SVG or PNG and return it with a shareable URL
- **render_mermaid_image**: Returns a stable public URL; the same source always renders the same image. Mermaid only; for other languages use render_diagram.

Render a Mermaid diagram to a PNG image URL via the mermaid.ink service
- **validate_diagram**: Cheaper than render_diagram when the goal is only to confirm syntax — for example before writing the diagram into a file that a build step renders.

Check that diagram source parses, without rendering it


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Diagrams** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Draw the deployment pipeline we just designed as a flowchart."

**🤖 AI Agent:**
> Rendered. I wrote the pipeline as a Mermaid flowchart — commit, build, test, staging, production, with the approval gate branching back — and rendered it to SVG. It comes back as a URL that serves the image permanently and the SVG markup, so you can paste it straight into the design doc. The same source always renders the same image, so the link will not rot.

---

**👤 You:**
> "I have our schema in a text file. Show it as a diagram."

**🤖 AI Agent:**
> Done. I read the schema and laid it out in Graphviz DOT with the tables as nodes and the foreign keys as edges, so the layout is automatic and stays tidy however many tables there are. It rendered to SVG with a permanent URL and the markup to paste in. If you would rather edit it by hand, Mermaid is friendlier to write and I can convert it.

---

**👤 You:**
> "Put this sequence into the slide deck as an image, not code."

**🤖 AI Agent:**
> Rendered to PNG. The slide strips raw SVG, so I used the raster path instead — Mermaid sequence diagram rendered through mermaid.ink. It returns a PNG URL that embeds anywhere an image goes, and the file is a real raster image at any zoom. The same diagram is also available as SVG if the deck ever accepts vectors.


## ❓ FAQ

**Q: Do I need an API key?**
No. This renders through the public Kroki and mermaid.ink services, which need no key or account.

**Q: Which diagram language should I use?**
Mermaid for flowcharts, sequence and Gantt — it is the friendliest to write by hand. PlantUML for full UML. Graphviz when you need automatic layout of many nodes. D2 for modern styled diagrams. Vega for charts from JSON, and wavedrom for digital timing waveforms. Call list_diagram_types to see all nine with what each is for.

**Q: Why does the tool hand back a URL — where is the image?**
The URL serves the rendered image directly and deterministically: the same source always produces the same image, so it is safe to embed permanently in a doc or slide. For SVG the tool also returns the markup itself, so you can paste it straight into an HTML page or a document that accepts raw SVG.

**Q: Can I get a PNG?**
For mermaid, plantuml, graphviz and ditaa, pass output_format png to render_diagram — or use render_mermaid_image for a Mermaid-only PNG through mermaid.ink. d2, excalidraw, nomnoml, vega and wavedrom render SVG only; the tool refuses a format a language does not support rather than returning an error from the server.

**Q: My diagram did not render. What now?**
The error message quotes the renderer's own parse error. Call get_diagram_example with the same diagram type to get a working starter, edit it towards your diagram, and use validate_diagram to check the syntax without committing to a render.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/diagrams](https://vinkius.com/en/ai-agent-connect/diagrams)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Diagrams** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `diagrams` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Diagrams** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "diagrams": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
