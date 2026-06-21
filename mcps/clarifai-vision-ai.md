# Clarifai (Vision AI) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/clarifai-vision-ai)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Manage AI inference via Clarifai — list apps, models, and workflows, and perform computer vision predictions directly from any AI agent.

## Description
Connect your **Clarifai** account to any AI agent and take full control of your computer vision and AI workflows through natural conversation.

### What you can do

- **AI Inference (Predictions)** — Dispatch automated validation inferences and parse exactly what the neural networks evaluated
- **App & Model Management** — List Clarifai apps and models to organize and audit your compute environments
- **Chained Workflows** — Retrieve composed computational blocks that tie multiple models together for complex AI tasks
- **Datasets & Concepts** — Identify data structures used for training and audit the textual concepts tagging your visual data
- **Identity Mapping** — Navigate users and apps to isolate your AI logic across different execution contexts

### How it works

1. Subscribe to this server
2. Enter your Clarifai Personal Access Token (PAT)
3. Start managing your AI workflows from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **AI Developers** — test model predictions and workflow logic using natural language without writing boilerplate code
- **Data Scientists** — audit datasets and concepts to ensure training data consistency across different applications
- **ML Engineers** — monitor and manage active compute brains (models) and their execution contexts
- **Product Teams** — quickly verify AI output and vision logic during the prototyping phase


## Available Tools (6)
- **list_apps**: Identify bounded Clarifai apps managing global compute limits
- **list_models**: Perform structural extraction of computer vision parameters driving AI features
- **predict_model**: /models/{model_id}/outputs` parsing exactly what the AI limit evaluated bounding image classifications.

Dispatch an automated validation inference routing explicit network predictions
- **list_workflows**: Retrieve the exact structural matching verifying chained AI limits
- **list_datasets**: Identify precise physical bounds mapping data structures resolving visual nodes
- **list_concepts**: Extracts explicitly attached semantic bounds tagging datasets matching limits


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Clarifai (Vision AI)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Clarifai apps for user 'user_123'"

**🤖 AI Agent:**
> I found 4 apps for 'user_123': 'Image-Moderation', 'Face-Recognition', 'General-Vision', and 'Custom-Trainer'. Which one would you like to explore?

---

**👤 You:**
> "Predict using model 'general-v2' in app 'General-Vision' with image URL 'https://example.com/photo.jpg'"

**🤖 AI Agent:**
> Inference complete! The model detected: 'Person' (99.2%), 'Outdoors' (95.4%), 'Mountain' (92.1%). I have the full JSON response if you need the bounding boxes.

---

**👤 You:**
> "What datasets are available in the 'Custom-Trainer' app?"

**🤖 AI Agent:**
> The 'Custom-Trainer' app has 2 datasets: 'training-v1' (500 images) and 'validation-v1' (100 images). I can also list the concepts tagging these images.


## ❓ FAQ

**Q: Can my agent run image predictions using custom models?**
Yes. Provide the User ID, App ID, and Model ID, along with the input JSON (containing image URLs or bytes). The agent calls Clarifai's predict API and returns exactly what the AI detected, from tags to bounding boxes.

**Q: How can I audit the datasets being used in my Clarifai app?**
Ask your agent to list datasets for a specific app. It returns the precise physical bounds mapping the image sets, helping you ensure that your training loop is using the correct data boundaries.

**Q: Can I see all active workflows in my organization?**
Absolutely. Use the 'list_workflows' tool. Your agent will pull the chained AI limits, showing you composed computational blocks that tie multiple neural networks together for complex visual tasks.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/clarifai-vision-ai](https://vinkius.com/mcp/clarifai-vision-ai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Clarifai (Vision AI)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `clarifai-vision-ai` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Clarifai (Vision AI)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "clarifai-vision-ai": {
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
