# Perplexity AI MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/perplexity-ai)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Query Perplexity AI for real-time web search with citations — ask questions, deep research, reasoning, and structured answers directly from any AI agent.

## Description
Connect your **Perplexity AI** API key to any AI agent and harness the power of real-time web search with AI-generated answers, citations, and related questions through natural conversation.

### What you can do

- **Answer Questions** — Ask any question and get grounded answers with real-time web search and source citations
- **Deep Research** — Perform exhaustive research on complex topics with comprehensive reports and thorough citations
- **Logical Reasoning** — Solve complex problems requiring step-by-step analysis and chain-of-thought reasoning
- **Domain-Filtered Search** — Restrict search results to specific domains for academic, technical, or trusted-source queries
- **Recency Filtering** — Get answers based on recent information only (hour, day, week, month, or year)
- **Multi-Turn Conversations** — Maintain context across multiple questions for iterative research sessions
- **Structured Output** — Get responses in JSON format following a defined schema for programmatic integration
- **Visual Results** — Include relevant images and related questions in search results

### How it works

1. Subscribe to this server
2. Enter your Perplexity API key from your account settings
3. Start researching, asking questions, and getting cited answers from Claude, Cursor, or any MCP-compatible client

No more switching between search engines and reading through pages of results. Your AI acts as a dedicated research assistant with real-time web access.

### Who is this for?

- **Researchers** — perform comprehensive literature reviews, deep research on topics, and get cited answers instantly
- **Analysts** — filter searches to trusted domains, get recent data, and perform complex reasoning with structured outputs
- **Students** — ask questions with citations for academic work, get related questions for further study, and understand complex topics
- **Developers** — get structured JSON responses, code analysis, and reasoning for technical problem-solving


## Available Tools (14)
- **chat_with_recency_filter**: Available recency filters: "hour", "day", "week", "month", "year".
This ensures the answer is based on recent information only.
Use this for news, recent events, or time-sensitive queries where outdated info is not useful.

Ask Perplexity AI with results filtered by time recency
- **chat_with_related_questions**: The response includes a related_questions array with suggested questions for further exploration.
Use this for research, learning, and discovering related topics you might want to explore.

Ask Perplexity AI and get related follow-up questions
- **chat_completion**: The Sonar model searches the web, synthesizes information, and provides a concise answer.
This is the basic query tool for factual questions, summaries, and general knowledge.
Use this for quick lookups where you need accurate, up-to-date information.

Ask Perplexity AI a question and get a grounded, cited answer
- **chat_with_citations**: Each claim or fact in the response is linked to its original source.
This is essential for research, fact-checking, and academic work where sources matter.
The response includes a citations array with URLs of all referenced sources.

Ask Perplexity AI and get answers with source citations
- **chat_with_domain_filter**: Provide domains as a comma-separated list (e.g., "arxiv.org,nih.gov,github.com").
Only sources from the specified domains will be used in generating the answer.
Use this for domain-specific research, academic papers, or trusted sources only.
Citations are automatically included to verify sources.

Ask Perplexity AI restricting search to specific domains
- **chat_with_history**: Provide messages as a JSON array of {role: "user"|"assistant"|"system", content: "text"} objects.
This enables follow-up questions where the model understands previous context.
Use this for complex queries that build on previous answers or require contextual understanding.
Example: [{ "role": "user", "content": "What is quantum computing?" }, { "role": "assistant", "content": "Quantum computing uses quantum bits..." }, { "role": "user", "content": "How does it differ from classical computing?" }]

Ask Perplexity AI with multi-turn conversation history
- **chat_with_images**: The response includes an images array with URLs to related images found during the search.
Use this for visual topics, product searches, or when you need images to accompany the answer.

Ask Perplexity AI and get relevant images with the answer
- **deep_research**: This model performs extensive web searches and generates detailed reports with thorough citations.
It takes longer than regular queries but provides much more depth and breadth.
Use this for complex topics, literature reviews, competitive analysis, or thorough investigations.
Maximum tokens default to 4096 for comprehensive responses.

Perform deep research with exhaustive web search and comprehensive report
- **follow_up**: Provide the conversation history as a JSON array of messages and the follow-up question.
This maintains context from previous turns in the conversation.
Use this for multi-turn research sessions where each question builds on previous answers.

Ask a follow-up question in an ongoing conversation with Perplexity AI
- **list_models**: Use this to discover what models are available
before choosing which one to use for your queries.

List all available Perplexity AI models
- **reasoning**: This model excels at multi-step reasoning, mathematical problems, code analysis, and chain-of-thought tasks.
Use this for problems requiring step-by-step analysis, mathematical proofs, code reviews, or logical deductions.
Citations are included where external information is referenced.

Ask Perplexity AI for complex logical reasoning and step-by-step analysis
- **search_query**: This combines all search features: cited sources, relevant images, and follow-up questions.
Use this when you want the fullest possible search result with all supplementary information.
The response includes content, citations array, images array, and related_questions array.

Perform a comprehensive web search with citations, images, and related questions
- **structured_query**: The model will return the answer as JSON matching your schema definition.
Provide the JSON schema as a string. This is useful for programmatic data extraction,
API integrations, and when you need consistent, parseable responses.
Example schema: { "type": "object", "properties": { "name": { "type": "string" }, "age": { "type": "number" } } }

Ask Perplexity AI and get a structured JSON response following a schema
- **system_prompt_query**: The system prompt defines how the model should respond (e.g., "You are a medical expert...", "Answer in bullet points...").
Use this for specialized queries, role-playing, formatting requirements, or domain-specific expertise.
Example system prompt: "You are a senior software architect. Explain concepts with code examples."

Ask Perplexity AI with a custom system prompt to set behavior and context


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Perplexity AI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the latest developments in quantum computing as of this week?"

**🤖 AI Agent:**
> Based on recent developments this week, there are three major breakthroughs in quantum computing:

1. **IBM's 1000+ qubit processor** achieved new error correction milestones, reducing error rates by 50% compared to previous generations.
2. **Google Quantum AI** demonstrated quantum advantage in optimization problems for logistics, showing 100x speedup over classical algorithms.
3. **A team at MIT** developed a new topological qubit design that maintains coherence at higher temperatures.

📚 **Sources:** Nature.com, MIT News, IBM Research Blog

Would you like me to research any of these breakthroughs in more detail?

---

**👤 You:**
> "Do deep research on the competitive landscape of electric vehicle manufacturers in Southeast Asia, including market share, pricing strategies, and government incentives."

**🤖 AI Agent:**
> I've conducted comprehensive research on the EV competitive landscape in Southeast Asia. Here's the analysis:

## Market Leaders
1. **BYD** — 35% market share, aggressive pricing ($15K-30K), strong government partnerships in Thailand and Indonesia
2. **Tesla** — 18% market share, premium positioning ($40K+), expanding Supercharger network
3. **Neta (Hozon)** — 12% market share, budget-friendly ($10K-20K), popular in Vietnam

## Government Incentives
- **Thailand:** Up to ฿150,000 ($4,200) subsidy per EV, 0% import duty until 2025
- **Indonesia:** 0% luxury tax for EVs, $3,500 purchase incentive
- **Vietnam:** 0% registration fee until 2027, reduced road tax

## Key Strategies
- Local manufacturing to avoid import tariffs
- Battery swapping infrastructure partnerships
- Fleet sales to ride-hailing platforms (Grab, Gojek)

📚 **15 sources cited** including Reuters, BloombergNEF, and regional government reports.

Would you like me to dive deeper into any specific country or manufacturer?

---

**👤 You:**
> "Search for news about AI regulation in the European Union from the last month, restricted to europa.eu and reuters.com domains."

**🤖 AI Agent:**
> I found 5 recent articles about AI regulation in the EU from the last month, restricted to europa.eu and reuters.com:

1. **EU Commission publishes implementation guidelines for the AI Act** — europa.eu, 2 weeks ago
2. **European countries scramble to meet AI Act compliance deadlines** — reuters.com, 1 week ago
3. **EU establishes new AI Office to enforce regulations** — europa.eu, 3 weeks ago
4. **Industry leaders respond to EU AI Act risk classification system** — reuters.com, 4 days ago
5. **EU member states finalize national AI regulatory frameworks** — europa.eu, 5 days ago

📚 **Citations:** All 5 sources from europa.eu and reuters.com with direct links.

Would you like me to summarize any of these articles in detail?


## ❓ FAQ

**Q: How do I get a Perplexity API key?**
Log in to your [**Perplexity AI account**](https://www.perplexity.ai/), go to **Settings > API**, and generate a new API key. Copy the key (it starts with `pplx-`) immediately. Paste it into the API key field below. This key authenticates all requests to https://api.perplexity.ai.

**Q: What's the difference between Sonar, Sonar Pro, Deep Research, and Reasoning Pro models?**
**Sonar** is the fastest model for quick factual answers and basic synthesis. **Sonar Pro** handles complex queries better with more thorough analysis and follow-up support. **Sonar Deep Research** performs exhaustive web searches and generates comprehensive reports with thorough citations — best for research papers and deep investigations. **Sonar Reasoning Pro** excels at logical reasoning, multi-step analysis, mathematical problems, and chain-of-thought tasks.

**Q: Can I restrict search results to specific domains or time periods?**
Yes! Use `chat_with_domain_filter` to restrict search to specific domains (e.g., arxiv.org, nih.gov, github.com). Use `chat_with_recency_filter` to get results only from the last hour, day, week, month, or year. You can also combine both for domain-specific recent information. Citations are automatically included to verify sources.

**Q: How does Perplexity AI differ from regular search engines?**
Unlike regular search engines that return a list of links, Perplexity AI reads the web in real-time, synthesizes information from multiple sources, and provides a direct, concise answer with citations. It's like having a research assistant that reads dozens of pages and summarizes the key findings with source links. You get answers, not just links.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/perplexity-ai](https://vinkius.com/mcp/perplexity-ai)
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
3. Set Type to "SSE" (or "streamable HTTP"), enter `perplexity-ai` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Perplexity AI** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "perplexity-ai": {
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
