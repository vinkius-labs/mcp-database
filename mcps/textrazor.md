# TextRazor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/textrazor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Advanced Natural Language Processing (NLP) to extract entities, topics, and relations from text or URLs.

## Description
Connect **TextRazor** to your AI agent to unlock state-of-the-art text analysis capabilities. This server allows your agent to perform deep semantic analysis on raw text or live web content, identifying thousands of entity types and complex relationships.

### What you can do

- **Deep Text Analysis** — Extract entities, topics, relations, and dependency trees from any text input or public URL.
- **Custom Dictionaries** — Create and manage your own dictionaries to identify domain-specific terminology or proprietary entities.
- **Content Categorization** — Automatically classify content into thousands of topics and categories for better organization.
- **Entity Disambiguation** — Link extracted entities to knowledge bases like DBPedia and Freebase for rich context.
- **Cleanup & Extraction** — Automatically strip HTML tags or use metadata to improve analysis accuracy on web pages.

### How it works

1. Subscribe to this server
2. Enter your TextRazor API Key
3. Start analyzing documents and websites directly from your AI assistant

### Who is this for?

- **Data Scientists** — automate the extraction of structured data from massive amounts of unstructured text
- **Content Managers** — automatically tag and categorize articles or blog posts for SEO and discovery
- **Market Researchers** — monitor news and social media by extracting key entities and relations in real-time


## Available Tools
- **add_dictionary_entries**: Add entries to a custom dictionary
- **analyze_text**: Provide either text or url, and a comma-separated list of extractors.

Analyze text or URL to extract entities, topics, relations, etc
- **create_category**: Create or update a custom classifier/category
- **create_dictionary**: Create a new custom dictionary
- **delete_category**: Delete a custom classifier
- **delete_dictionary**: Delete a custom dictionary and its entries
- **get_account**: Get account details, usage, and limits
- **get_dictionary**: Get details of a specific custom dictionary
- **list_categories**: List all categories in a custom classifier
- **list_dictionary_entries**: List all entries in a custom dictionary
- **list_dictionaries**: List all custom dictionaries


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TextRazor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze this text for entities and topics: 'TextRazor is a startup based in London specializing in NLP.'"

**🤖 AI Agent:**
> I've analyzed the text. I found entities like 'TextRazor' (Company) and 'London' (Place), and identified topics related to 'Natural Language Processing' and 'Technology startups'.

---

**👤 You:**
> "Extract relations and dependency trees from the URL https://www.textrazor.com/"

**🤖 AI Agent:**
> I've processed the content from the URL. I've mapped out the grammatical dependency trees and extracted key relations between the entities mentioned on the page.

---

**👤 You:**
> "Create a new dictionary called 'MedicalTerms' for specialized analysis."

**🤖 AI Agent:**
> I have successfully created the 'MedicalTerms' dictionary. You can now start adding entries to it using the add_dictionary_entries tool.


## ❓ FAQ

**Q: How can I analyze a web page directly without copying the text?**
Use the `analyze_text` tool and provide the target link in the `url` parameter. TextRazor will fetch the content and process it based on your requested extractors.

**Q: Can I filter entities by specific types like DBPedia?**
Yes, the `analyze_text` tool includes an `entities_filterDbpediaTypes` parameter. You can provide a list of types to narrow down the results to exactly what you need.

**Q: How do I manage custom terminology for my business?**
You can use `create_dictionary` to initialize a new knowledge base and then use `add_dictionary_entries` to populate it with your specific terms and IDs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/textrazor](https://vinkius.com/mcp/textrazor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **TextRazor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `textrazor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **TextRazor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "textrazor": {
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
