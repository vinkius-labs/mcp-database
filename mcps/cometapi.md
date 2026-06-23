# CometAPI MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cometapi)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Connect to real-time financial market data with APIs for stocks, forex, and crypto that power trading applications.

## Description
Connect your **CometAPI** account to any AI agent and take full control of your multimodal AI workflows through a single, perfectly coordinated intelligence layer.

### What you can do

- **Multimodal Orchestration** — Execute chat completions, generate high-fidelity images, and convert speech to text across 500+ cutting-edge models (GPT-4, Claude, Midjourney, etc.)
- **Model Discovery** — Access complete directories of available LLM, image, and audio models supported by the aggregator directly through your agent
- **Provider Intelligence** — List and monitor supported AI providers (OpenAI, Anthropic, Google) to ensure the perfect model selection for your specific tasks
- **Financial Visibility** — Programmatically track your credit consumption and pricing information to maintain operational oversight of your AI budget
- **Operational Monitoring** — Check real-time API health and verify user profile metadata directly through your agent for reliable multimodal operations

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from the CometAPI dashboard
3. Start interacting with hundreds of AI models from Claude, Cursor, or any MCP client

No more manual toggling between dozens of provider dashboards or managing multiple API keys. Your AI acts as your dedicated model engineer and multimodal coordinator.

### Who is this for?

- **AI Developers** — instantly prototype across multiple providers and models using natural language commands
- **Content Creators** — automate the generation of text, images, and audio assets without leaving your workspace
- **Product Leads** — monitor AI model performance and costs across the entire organization through simple AI queries


## Available Tools (10)
- **create_ai_chat_completion**: Supports GPT-4, Claude, Gemini, etc.

Generate AI text response
- **check_api_health**: Verify API status
- **convert_text_to_speech**: Convert text to audio
- **transcribe_audio_to_text**: Transcribe audio files
- **generate_ai_image**: Generate an image from a prompt
- **get_current_user**: Get authenticated user profile
- **get_pricing_information**: Retrieve model pricing info
- **get_api_usage_statistics**: Get account usage and costs
- **list_available_ai_models**: List all supported AI models
- **list_supported_ai_providers**: ) supported by the aggregator.

List integrated AI providers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CometAPI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a summary of the latest AI trends using GPT-4."

**🤖 AI Agent:**
> AI summary generated! I've used GPT-4 to analyze recent breakthroughs. Highlights include advancements in multimodal reasoning and agentic workflows. Would you like a detailed breakdown for any specific trend?

---

**👤 You:**
> "Create a high-res image of a sustainable city using Midjourney."

**🤖 AI Agent:**
> Visual generation triggered! I've started creating your sustainable city image on Midjourney. You can access the result here: [image_url]. Shall I generate a matching logo design as well?

---

**👤 You:**
> "What is my current credit balance and average daily cost?"

**🤖 AI Agent:**
> Scanning account... You have $25.50 in credits remaining. Your average daily cost is $1.20, giving you approximately 21 days of uptime at current levels. Need a list of supported providers?


## ❓ FAQ

**Q: How do I find my CometAPI API Key?**
Log in to your account, navigate to the **API Dashboard**, and copy your secret key (sk-...).

**Q: Can I generate images with different models?**
Yes! Use the `generate_ai_image` tool and specify the model ID (e.g., 'midjourney' or 'dall-e-3') for your creation.

**Q: Does it support voice-to-text?**
Absolutely. The `transcribe_audio_to_text` tool allows you to convert any public audio URL into text using high-performance STT models.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cometapi](https://vinkius.com/mcp/cometapi)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CometAPI** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cometapi` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CometAPI** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cometapi": {
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
