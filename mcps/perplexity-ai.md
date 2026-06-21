# Perplexity AI MCP Server

Query Perplexity AI for real-time web search with citations — ask questions, deep research, reasoning, and structured answers directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/perplexity-ai)

## Overview
**Category:** ai-frontier
**Tools Count:** 14

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


## Available Tools
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
- **chat_with_recency_filter**: Available recency filters: "hour", "day", "week", "month", "year".
This ensures the answer is based on recent information only.
Use this for news, recent events, or time-sensitive queries where outdated info is not useful.

Ask Perplexity AI with results filtered by time recency
- **chat_with_related_questions**: The response includes a related_questions array with suggested questions for further exploration.
Use this for research, learning, and discovering related topics you might want to explore.

Ask Perplexity AI and get related follow-up questions
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


## Installation & Usage

To install and use the **Perplexity AI** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/perplexity-ai](https://vinkius.com/mcp/perplexity-ai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
