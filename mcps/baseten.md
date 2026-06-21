# Baseten MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/baseten)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Manage your Baseten AI models — orchestrate deployments, list secrets, and run serverless inference predictions autonomously.

## Description
Connect your **Baseten** account to any AI agent and track, deploy, and execute your machine learning models through natural conversation.

### O que você pode fazer

- **Model Management** — List managed models, fetch configurations, and understand active routing boundaries
- **Serverless Deployments** — Inspect exact replica states, autoscaling configurations, and deployment versions
- **Inference Execution** — Run direct predictions (`predict`) pushing tensor payloads or JSON directly to GPU weights
- **Workspace Secrets** — Enumerate active environment secrets securely mapped inside the isolated orchestration ecosystem

### Como funciona

1. Subscribe to this server
2. Enter your Baseten API Key
3. Gain complete ML-Ops control over your active inference nodes using Claude, Cursor, or your preferred agent

Scale unified AI infrastructure without bouncing between terminal windows. Your agent becomes a capable Machine Learning Operator tracking your GPU lifecycle.

### Para quem é?

- **ML Engineers** — execute test payloads to deployments instantaneously without spinning up local Python notebooks
- **DevOps/SREs** — audit running deployment resources and verify replica states reliably from your core IDE
- **AI Researchers** — inspect version schemas and manage inference pipeline architectures quickly


## Available Tools
- **list_models**: List Baseten managed models
- **get_model**: Get a specific Baseten model
- **predict**: Formulate the explicit tensor shapes or dictionaries strictly matching the deployed instance.

Invoke a serverless model inference prediction
- **list_deployments**: List active inferences bounds matching a specific model
- **get_deployment**: Get explicit details of a running deployment
- **list_secrets**: List securely managed workspace secrets without showing values


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Baseten** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List standard machine learning models we currently host on Baseten."

**🤖 AI Agent:**
> You have 2 primary managed models explicitly mapped: A fine-tuned 'Llama-3-70B-Instruct' (ID: XYZ) and a custom computer vision 'Defect-Detector-V2' (ID: ABC). Want to pull explicit active Deployment states for the Llama model?

---

**👤 You:**
> "Run a prediction against the Sentiment model ID 12345 using this text input: 'The new feature completely broke my workflow.'"

**🤖 AI Agent:**
> The Baseten inference pipeline returned the following calculated object mapping successfully: `{"score": 0.12, "label": "NEGATIVE"}`. Prediction executed cleanly across targeted model instances in real-time.

---

**👤 You:**
> "Check if our Baseten project has a secret scoped as 'OPENAI_API_KEY_FALLBACK'."

**🤖 AI Agent:**
> I checked the environment isolation layer. `OPENAI_API_KEY_FALLBACK` is indeed fully provisioned alongside `HF_TOKEN`. Secret logic passes checks avoiding explicit plaintext extractions over network streams as per Baseten guidelines.


## ❓ FAQ

**Q: Can the AI agent run a prediction directly against my hosted model?**
Yes. By pushing a correctly formatted JSON payload to the 'predict' tool, the agent securely triggers inference on the GPU instances, returning the exact calculated response data transparently to your editor context.

**Q: Is my workspace and environmental secret data kept safe?**
Baseten secret fetching natively obscures variable values. When you use 'list_secrets', the agent simply evaluates the key names and identifiers existing across your environment to verify configurations without exposing plaintext passwords.

**Q: How do I check auto-scaling configurations for an explicitly deployed model?**
You can examine exactly how instances are managed by using 'get_deployment'. Tell the agent to target an active deployment ID and it maps the scaling limits, replica status, and container bounds out-of-the-box.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/baseten](https://vinkius.com/mcp/baseten)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Baseten** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `baseten` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Baseten** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "baseten": {
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
