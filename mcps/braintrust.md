# Braintrust MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/braintrust)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [brain-trust](../categories/brain-trust.md)

Automate AI evaluations with Braintrust — organize projects, test model datasets, run benchmarks, and manage prompts via any AI agent.

## Description
Connect your **Braintrust** AI observation platform to any agent and maintain intense logic evaluation capabilities directly over conversation.

### What you can do

- **Project Analytics** — Retrieve logic banks and branch isolated AI test sets
- **Experiments** — Create real trace regression tests appending unique LLM scoring iterations
- **Datasets** — Query accurate Ground Truth sets and insert new prompt templates mapping your system accuracy
- **Prompt Versioning** — Grab perfectly frozen semantic prompts without editing core code boundaries

### How it works

1. Add this server to your AI cluster
2. Bind your personal Braintrust API ID variables
3. Leverage complex model tuning pipelines querying native AI logic regressions on chat

Automate LLM regression analyses effortlessly. Rather than scrolling tables, your bot handles strict semantic checking via Braintrust infrastructure logic directly.

### Who is this for?

- **AI Developers** — push Ground Truth evaluation text datasets on the fly testing prompt differences
- **Machine Learning Engineers** — track specific variable distributions checking accurate regressions remotely
- **Product Teams** — observe exact string prompts dynamically pushing features validating response styles
- **Data Scientists** — construct massive matrices and evaluate test runs without pulling script queries


## Available Tools (10)
- **create_experiment**: Establish a new historical experiment trace to record LLM pipeline tests
- **create_project**: Create a new project environment for tracking AI evaluations and datasets
- **list_datasets**: List isolated Ground Truth text banks used for automated evaluation scoring
- **list_env_vars**: Probe the Braintrust AI Gateway configurations managing model API keys securely
- **list_experiments**: Retrieve all evaluation experiments mapping model test scores and metrics
- **get_dataset**: Retrieve a specific dataset containing exact schemas bounding LLM outputs
- **get_prompt**: Retrieve exact variable contexts and literal text templates for a prompt
- **insert_dataset_row**: Append new test cases into a dataset matrix targeting specific evaluations
- **list_projects**: Retrieve the list of all AI evaluation projects in Braintrust
- **list_prompts**: Retrieve explicitly version-controlled system prompts isolated in Braintrust


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Braintrust** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active test datasets configured under Braintrust."

**🤖 AI Agent:**
> I've fetched your Ground Truth repositories. There's 1 dataset active under ID 4a83b9c named 'Support-Responses-Testing'. Should I list the rows nested there?

---

**👤 You:**
> "Look up prompt template using specific ID XYZ."

**🤖 AI Agent:**
> Prompt XYZ returns successfully. It tracks specific {{user}} tags targeting strict instructions enforcing a professional tone. The JSON mapping version is 1.0.4. Do you need further metadata?

---

**👤 You:**
> "Analyze recent experiments across multiple models testing behavior."

**🤖 AI Agent:**
> Extracted the historical trace boundaries. Experiment run ID V3 generated a 94% alignment score compared to the previously logged V2 base structure matrix mapping differences on false positives.


## ❓ FAQ

**Q: Can I insert new test data dynamically tracking specific limits?**
Yes. Utilizing the `insert_dataset_row` method, you can effortlessly inject exact JSON tracking payload mapping strings directly inside the text corpus evaluating the final results.

**Q: Does it pull out original Prompt definitions stored securely?**
Certainly. The `get_prompt` command isolates and returns perfectly version-controlled bounding parameters slicing literal templates natively hosted under the Braintrust database.

**Q: How deeply can it inspect test regressions or scoring limits?**
Using the robust `list_experiments` call, you can branch full arrays separating LLM version behaviors over massive iterations tracking the performance anomalies accurately.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/braintrust](https://vinkius.com/mcp/braintrust)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Braintrust** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `braintrust` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Braintrust** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "braintrust": {
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
