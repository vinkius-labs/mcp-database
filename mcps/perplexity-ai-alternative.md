# Perplexity AI MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/perplexity-ai-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Access Perplexity's AI search and chat models — get web-grounded answers with citations, search the web and run AI conversations from any AI agent.

## Description
Connect your **Perplexity AI** account to any AI agent and leverage web-grounded AI models through natural conversation.

### What you can do

- **Chat Completions** — Send conversations to Perplexity models (sonar, sonar-pro, sonar-reasoning) and receive responses with web citations
- **Web Search** — Search the web using Perplexity's dedicated Search API with domain filtering
- **Sonar API** — Get web-grounded responses from the Sonar model with citations and source URLs
- **Model Discovery** — List all available Perplexity models and their capabilities

### How it works

1. Subscribe to this server
2. Enter your Perplexity API Key
3. Start using Perplexity models from Claude, Cursor, or any MCP-compatible client

No more switching between search engines and chat tools. Your AI acts as a web-grounded research assistant.

### Who is this for?

- **Researchers** — get web-grounded answers with citations for fact-checking and literature review
- **Developers** — integrate web search and AI chat into applications via API
- **Analysts** — search the web with domain filters and get structured search results


## Available Tools (8)
- **chat**: Requires the model ID (e.g. "sonar", "sonar-pro", "sonar-reasoning") and messages array in JSON format. Each message must have a "role" ("user", "assistant" or "system") and "content" (text). Optionally set max_tokens, temperature (0-1), top_p (0-1), search domain filter, and whether to return images or related questions. Returns the assistant's response with citations.

Send a chat message to a Perplexity model
- **chat_pro**: Requires messages array in JSON format. Optionally set max_tokens and temperature. Returns the assistant's response with citations.

Send a chat message to the Sonar Pro model for enhanced responses
- **chat_with_reasoning**: Requires messages array in JSON format. Optionally set max_tokens, temperature and reasoning_effort (low, medium, high). Returns the assistant's response with detailed reasoning chain.

Send a message to the Sonar Reasoning model for step-by-step reasoning
- **chat_with_reasoning_pro**: Requires messages array in JSON format. Optionally set max_tokens, temperature and reasoning_effort (low, medium, high). Returns the assistant's response with detailed reasoning chain and citations.

Send a message to the Sonar Reasoning Pro model for deep reasoning
- **get_usage**: Useful for monitoring API consumption and staying within usage limits.

Get API usage statistics
- **list_models**: Each model returns its ID (e.g. "sonar", "sonar-pro", "sonar-reasoning", "sonar-reasoning-pro"), display name and capabilities. Use this to discover which models are available and their IDs for use with the chat and sonar tools.

List all available Perplexity models
- **search**: Returns search results with snippets, citations and source URLs. Requires the search query. Optionally set max_results and domain filter to limit results to specific websites.

Search the web using Perplexity Search API
- **sonar**: This is the core search-enhanced model. Requires messages array in JSON format. Optionally set max_tokens and temperature. Returns the assistant's response with web citations.

Send a message to the Sonar model for web-grounded responses


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Perplexity AI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search the web for 'latest advances in quantum computing 2025'."

**🤖 AI Agent:**
> Found recent articles on quantum error correction breakthroughs, Google's Willow chip achieving below-threshold error rates, and IBM's 1000+ qubit processors. Key sources include Nature, MIT Technology Review and Science Daily.

---

**👤 You:**
> "Ask Sonar: What is the current price of Bitcoin?"

**🤖 AI Agent:**
> Bitcoin is currently trading at $87,234 USD according to CoinMarketCap data from today. The price has increased 3.2% in the last 24 hours with a market cap of $1.73 trillion. Sources: CoinMarketCap, CoinGecko.

---

**👤 You:**
> "Send a chat to sonar-pro asking 'Explain how transformers work in NLP' with return_related_questions enabled."

**🤖 AI Agent:**
> Sonar-pro responded with a detailed explanation of transformer architecture including self-attention, multi-head attention, positional encoding and the encoder-decoder structure. Related questions returned include: 'What is the difference between BERT and GPT?', 'How does self-attention work?' and 'What are transformer limitations?'


## ❓ FAQ

**Q: How do I get a Perplexity API key?**
Log in to the [**Perplexity AI Settings**](https://www.perplexity.ai/settings/api), go to **API Key Management** and click **Create API Key**. Copy the key immediately — it starts with `pplx-` and won't be shown again.

**Q: What models are available?**
Use the `list_models` tool to see all available Perplexity models. Key models include sonar (web-grounded chat), sonar-pro (enhanced reasoning), sonar-reasoning and sonar-reasoning-pro. Each model provides real-time web search with citations.

**Q: Can I filter search results to specific domains?**
Yes! Use the `chat` or `search` tools with the search_domains parameter to limit results to specific websites (e.g. ["wikipedia.org","github.com"]). This is useful for research focused on trusted sources.

**Q: Do responses include citations?**
Yes! All Sonar models return responses with inline citations and a list of source URLs. The citations are embedded in the response text as numbered references [1], [2], etc., and the full source URLs are provided in the response metadata.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/perplexity-ai-alternative](https://vinkius.com/mcp/perplexity-ai-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Perplexity AI** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `perplexity-ai-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Perplexity AI** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "perplexity-ai-alternative": {
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
