# Groq MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/groq)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [superpower](../categories/superpower.md)

Empower LLM applications via Groq — perform ultra-fast LPU-accelerated chat completions, handle audio transcription and translation, and use JSON mode directly from any AI agent.

## Description
Connect your **Groq** account to any AI agent and take full control of your high-speed generative AI inference and LPU-accelerated LLM workflows through natural conversation.

### What you can do

- **LPU Chat Orchestration** — Execute blazing-fast text generation against hardware-accelerated Groq endpoints, utilizing Llama 3, Mixtral, and more flawlessly
- **Intelligent Audio Transcription** — Parse audio streams into high-accuracy language transcripts utilizing hardware-optimized Whisper models natively
- **Cross-Lingual Translation** — Evaluate non-English audio files and retrieve immediate translations exclusively into English text synchronousy
- **Structured JSON Mode** — Constrain AI text inference explicitly to rigid valid JSON formatting to automate data population and system integrations flawlessly
- **Tool & Function Calling** — Bind external definitions resolving explicit function call JSON architectures to enable your AI agents to interact with tools securely
- **Model Discovery** — Enumerate available high-speed models and retrieve specific model IDs and versions for precise active inference boundaries natively
- **Inference Auditing** — Monitor model capabilities and metadata properties to ensure your AI agents are utilizing the most efficient architectural instances synchronousy

### How it works

1. Subscribe to this server
2. Enter your Groq API Key (found in your Groq Cloud Dashboard > API Keys)
3. Start managing your ultra-fast AI inference from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **AI Developers** — test and debug LLM prompts and tool-calling logic with sub-second latency
- **Software Engineers** — generate structured JSON data and transcribe audio files directly from the IDE or chat
- **Product Teams** — monitor model availability and test generative AI features with real-time speed
- **Data Scientists** — evaluate different open-source model performances on Groq's LPU architecture through natural conversation


## Available Tools (8)
- **chat_completion**: Supports Llama, Mixtral, Gemma models.

Generate a chat completion with ultra-fast inference
- **list_models**: List available models
- **get_model**: Get model details
- **create_embedding**: Create text embeddings
- **transcribe_audio**: Transcribe audio to text
- **translate_audio**: Translate audio to English text
- **moderate_content**: Check content for safety
- **structured_output**: Generate structured JSON output


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Groq** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Ask llama3-70b: 'Write a python function to scrape a website.'"

**🤖 AI Agent:**
> Inference complete! Llama 3 response: 'Here is a simple python function using BeautifulSoup and requests to scrape data...' [Blazing-fast response delivered via Groq LPU].

---

**👤 You:**
> "Transcribe this audio meeting: https://example.com/meeting.mp3"

**🤖 AI Agent:**
> Transcription started! I'm using Groq optimized Whisper large-v3 model to parse your meeting audio. I'll provide the full timestamped text for you in just a few seconds.

---

**👤 You:**
> "Get model info for 'mixtral-8x7b-32768'"

**🤖 AI Agent:**
> Retrieving model metadata... Mixtral-8x7b-32768 is a high-performance LLM with a context window of 32,768 tokens. It supports chat completions and tool-calling on Groq's LPU architecture.


## ❓ FAQ

**Q: How fast are Groq's chat completions compared to standard GPUs?**
Groq's LPU architecture is designed for extreme low-latency inference, often delivering hundreds of tokens per second. Your agent uses the 'chat' tool to execute these blazing-fast requests, returning AI responses almost instantly.

**Q: Can my agent transcribe long audio files using Groq Whisper?**
Yes. Use the 'transcribe' tool. Provide the public URL of your audio file and select a Whisper model (e.g., 'whisper-large-v3'). The agent will parse the stream and return the full text transcript flawlessly.

**Q: How do I ensure the AI response is formatted as valid JSON via chat?**
Use the 'chat_json' tool. This activates Groq's JSON mode, which explicitly constrains the text inference to rigid, valid JSON formatting, making it perfect for direct system integrations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/groq](https://vinkius.com/mcp/groq)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Groq** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `groq` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Groq** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "groq": {
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
