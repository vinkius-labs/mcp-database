# Gradient AI (LLM API & Finetuning) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gradient-ai-llm-api-finetuning)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Access powerful LLMs, fine-tune models on your own data, and generate embeddings directly through your AI agent.

## Description
Connect to **Gradient AI** to leverage enterprise-grade LLM infrastructure. This server allows you to manage fine-tuned models, generate high-quality completions, and process text with specialized tools like sentiment analysis and entity extraction.

### What you can do

- **Model Management** — List foundational models and manage your custom fine-tuned instances.
- **Fine-Tuning** — Train models on your specific datasets to improve performance on niche tasks.
- **Advanced Completions** — Generate text with support for RAG (Retrieval Augmented Generation) and guidance parameters.
- **Embeddings** — Convert text into high-dimensional vectors for search and similarity tasks.
- **NLP Tools** — Perform sentiment analysis, answer questions from documents, and extract entities automatically.

### How it works

1. Subscribe to this server
2. Enter your Gradient API Key and Workspace ID
3. Start building and deploying custom AI solutions from your MCP client

### Who is this for?

- **AI Engineers** — quickly iterate on fine-tuning experiments and test model completions.
- **Data Scientists** — generate embeddings and perform NLP analysis without complex local setups.
- **Developers** — integrate advanced LLM capabilities into applications with minimal friction.


## Available Tools (19)
- **analyze_sentiment**: Analyze the sentiment of a document
- **answer_question**: Answer a question based on a source document
- **complete_model**: Generate a completion for a given prompt
- **generate_embeddings**: Generate embeddings for the provided inputs
- **upload_file**: Upload a file for use in other operations
- **create_model**: Create a new fine-tuned model instance
- **create_rag_collection**: Create a collection for RAG operations
- **create_transcription**: Start an audio transcription job
- **delete_model**: Delete a fine-tuned model
- **extract_entity**: Extract structured data from a document based on a schema
- **extract_pdf**: Extract text and data from a PDF file
- **fine_tune_model**: Train a model on provided samples
- **get_model**: Retrieve details about a specific model
- **get_transcription**: Retrieve the result of a transcription job
- **list_embeddings**: List available models for generating embeddings
- **list_models**: List available foundational and fine-tuned models
- **list_rag_collections**: List all RAG collections in the workspace
- **personalize_document**: Personalize a document for a specific audience
- **summarize_document**: Summarize a document


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gradient AI (LLM API & Finetuning)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all the models available in my Gradient workspace."

**🤖 AI Agent:**
> I've retrieved the models from your workspace. You have access to foundational models like 'llama3-8b' and your custom fine-tuned models such as 'customer-support-v1'.

---

**👤 You:**
> "Analyze the sentiment of this text: 'The new API performance is incredible!'"

**🤖 AI Agent:**
> The sentiment analysis for that text is 'Positive' with a high confidence score. The language used indicates strong satisfaction.

---

**👤 You:**
> "Generate a completion for 'Explain quantum computing' using model id 'base-llama3'."

**🤖 AI Agent:**
> Using the 'base-llama3' model: 'Quantum computing is a type of computing that uses quantum-mechanical phenomena, such as superposition and entanglement...' [Full response follows]


## ❓ FAQ

**Q: How can I start training a custom model with my own data?**
You can use the `fine_tune_model` tool. Simply provide the model ID and an array of training samples. The agent will handle the submission to Gradient's training infrastructure.

**Q: Can I use RAG (Retrieval Augmented Generation) with this server?**
Yes! The `complete_model` tool includes an optional `rag` parameter, allowing you to provide context or collection IDs to ground the model's responses in specific data.

**Q: How do I generate vector embeddings for my documents?**
Use the `generate_embeddings` tool by specifying a model slug (like 'bge-large') and a list of text inputs. It will return the high-dimensional vectors for your text.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gradient-ai-llm-api-finetuning](https://vinkius.com/mcp/gradient-ai-llm-api-finetuning)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Gradient AI (LLM API & Finetuning)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `gradient-ai-llm-api-finetuning` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Gradient AI (LLM API & Finetuning)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gradient-ai-llm-api-finetuning": {
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
