# Helicone (LLM Observability) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/helicone-llm-observability)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Monitor LLM usage via Helicone — track requests, analyze costs, measure latency, and manage prompts.

## Description
Connect your **Helicone** account to any AI agent and take full control of your LLM observability and gateway monitoring through natural conversation.

### What you can do

- **Request Monitoring** — Query deep proxy logs to inspect exact prompts and outputs sent to LLM APIs directly from your agent
- **Cost Analysis** — Break down spending by model, user, or custom metadata properties to monitor your AI burn rate in real-time
- **Latency Optimization** — Measure Time To First Token (TTFT) and pinpoint slowness caused by specific upstream LLM providers
- **Prompt Management** — Access managed prompt versions and track iterative changes in your AI instruction logic natively
- **Session Tracing** — Isolate and analyze multi-turn graph traces connecting consecutive LLM calls to debug complex agentic workflows
- **User Insights** — Track precise LLM interactions based on Helicone tags and identify your most active human clients
- **Feedback & RLHF** — Extract user critiques (Thumbs Up/Down) and log offline Human-in-the-Loop verdicts to improve model grounding

### How it works

1. Subscribe to this server
2. Enter your Helicone API Key
3. Start monitoring your LLM infrastructure from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **LLM Engineers** — debug prompt performance and measure TTFT latency across multiple upstream providers
- **Product Owners** — monitor AI spending and calculate costs per user, feature, or organization
- **Data Scientists** — analyze user feedback and improve model response quality through logged critiques
- **DevOps/SREs** — ensure the availability and reliability of your AI gateway and proxy layers


## Available Tools (10)
- **query_costs**: Perform structural extraction of properties driving active Account logic
- **query_feedback**: Inspect deep internal arrays mitigating specific Plan Math
- **query_latency**: Provision a highly-available JSON Payload generating hard Customer bindings
- **log_feedback**: Identify precise active arrays spanning native Hold parsing
- **query_prompts**: Retrieve explicit Cloud logging tracing explicit Vault limits
- **list_properties**: Identify precise active arrays spanning native Gateway auth
- **query_requests**: Identify bounded CRM records inside the Headless Helicone Platform
- **query_sessions**: Enumerate explicitly attached structured rules exporting active Billing
- **query_users**: Dispatch an automated validation check routing explicit Gateway history
- **get_prompt_versions**: Irreversibly vaporize explicit validations extracting rich Churn flags


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Helicone (LLM Observability)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much did we spend on GPT-4o yesterday?"

**🤖 AI Agent:**
> Yesterday, you spent a total of $42.15 on GPT-4o across 12,450 requests. The largest portion came from the 'Customer Support' feature tag ($28.40). Would you like a breakdown by user?

---

**👤 You:**
> "Show me the 10 slowest requests from the last hour"

**🤖 AI Agent:**
> I've identified the 10 slowest requests. The highest TTFT was 4.2s for an 'anthropic.claude-3-opus' call. Average latency for these 10 is 3.1s. Would you like to inspect the prompt for the slowest one?

---

**👤 You:**
> "List all versions for the 'customer-service-bot' prompt"

**🤖 AI Agent:**
> Found 5 versions for 'customer-service-bot'. Version 5 (latest) was deployed 2 days ago with updated grounding rules. Version 4 was active for 3 months. I can fetch the exact instruction text for any version.


## ❓ FAQ

**Q: Can I see the exact prompt that caused a specific error?**
Yes. Use the `query_requests` tool to fetch direct prompts and outputs from the proxy logs. You can filter by status or custom tags to find the exact interaction that needs debugging.

**Q: How do I track costs for a specific customer ID?**
Ask your agent to `query_costs` and include your customer identity in the filter. Helicone maps costs per model and user, allowing you to see exactly how much each client is burning in LLM tokens.

**Q: Can my agent log human feedback into Helicone?**
Absolutely. Use the `log_feedback` tool to inject offline Human-in-the-Loop verdicts or text critiques directly into Helicone's database, helping you refine your model's grounding over time.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/helicone-llm-observability](https://vinkius.com/mcp/helicone-llm-observability)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Helicone (LLM Observability)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `helicone-llm-observability` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Helicone (LLM Observability)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "helicone-llm-observability": {
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
