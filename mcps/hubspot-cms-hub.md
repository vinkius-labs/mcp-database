# HubSpot CMS Hub MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hubspot-cms-hub)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage blog posts, site pages, landing pages, authors, tags, and domains through natural conversation.

## Description
Connect **HubSpot CRM** to any AI agent — instant access to your full CRM data without switching tabs.

### What you can do
- **Contacts** — Search, create, and manage contacts
- **Companies** — Find companies by name or domain
- **Deals** — Search and create deals with pipeline tracking
- **Tickets** — Create and search support tickets
- **Notes** — Create notes attached to any CRM record
- **Owners** — View all owners and team assignments
- **Pipelines** — List deal and ticket pipeline stages

### Who is this for?
- **Sales Reps** — Manage your CRM without leaving your AI assistant
- **Support Teams** — Create tickets and notes on-the-go
- **RevOps** — Pipeline snapshots and owner assignments
- **Managers** — Full CRM visibility through conversation


## Available Tools (9)
- **hs_get_blog_post**: Returns full post details including title, meta description, slug, body content length, author, featured image, publish date, and SEO settings. Use after listing/searching posts to drill into a specific article for complete details.

Get the complete details of a specific HubSpot blog post by ID, including body content length and SEO metadata
- **hs_list_blog_authors**: Returns author display name, URL slug, email, and bio. Authors are linked to blog posts for byline attribution. Use when the user asks about content contributors, wants to find an author profile, or needs author IDs for blog post creation.

List blog authors configured in HubSpot CMS with name, email, slug, and biography
- **hs_list_blog_posts**: Returns post title, URL slug, current state (draft/published/scheduled), author name, and publish date. Use when the user asks about blog content, wants to review recent articles, check publishing status, or audit the content calendar.

List recent blog posts from HubSpot CMS with title, URL slug, publish status, author, and publish date
- **hs_list_blog_tags**: Returns tag name and slug used for content categorization and URL generation. Blog tags group related posts for navigation and topic clustering. Use when the user asks about content categories, available tags, or wants to audit the blog taxonomy.

List blog tags used for categorizing HubSpot blog content with tag name and URL slug
- **hs_list_domains**: Returns domain name, whether DNS is resolving correctly, if the domain is primary, and which HubSpot features use it (CMS, email, landing pages). Use when the user asks about connected domains, DNS configuration, or wants to verify domain setup.

List all domains connected to HubSpot with DNS resolution status, primary domain flag, and usage type
- **hs_list_landing_pages**: Landing pages are standalone conversion-focused pages (signup forms, lead magnets, event registration). Returns page title, slug, status, and full URL. Distinct from regular site pages — landing pages are typically ungated and optimized for form fills. Use when the user asks about conversion pages or lead capture pages.

List HubSpot landing pages designed for conversion with title, URL, publish status, and campaign association
- **hs_list_site_pages**: Returns page title, URL slug, current state (draft/published), and associated domain. Site pages are standard website pages (About, Contact, Pricing, etc.) — distinct from blog posts and landing pages. Use when the user asks about website content, page inventory, or publishing status.

List website pages hosted in HubSpot CMS with title, URL slug, publish status, and domain
- **hs_search_blog_posts**: Returns matching posts with title, slug, status, and date. Use when the user wants to find a specific article, check if a topic has been covered, or locate a post for updating.

Search HubSpot blog posts by title or keyword to find specific articles in the content library
- **hs_search_site_pages**: Returns matching pages with title, slug, status, and domain. Use when the user wants to find a specific website page or check if a topic has a dedicated page.

Search HubSpot site pages by title or keyword to find specific web pages


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HubSpot CMS Hub** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for contacts at Acme Corp"

**🤖 AI Agent:**
> 👥 **Contacts at Acme Corp**
| Name | Email | Phone | Lifecycle |
|---|---|---|---|
| John Smith | john@acme.com | +1 555-0123 | Customer |
| Sarah Chen | sarah@acme.com | +1 555-0456 | Lead |

---

**👤 You:**
> "Create a deal: Enterprise Package $50,000"

**🤖 AI Agent:**
> ✅ **Deal Created!**
- Name: Enterprise Package
- Amount: $50,000
- Pipeline: Sales Pipeline
- Stage: Appointment Scheduled

---

**👤 You:**
> "Show me the deal pipeline stages"

**🤖 AI Agent:**
> 📊 **Sales Pipeline**
1. Appointment Scheduled
2. Qualified to Buy
3. Presentation Scheduled
4. Decision Maker Bought-In
5. Contract Sent
6. Closed Won ✅
7. Closed Lost ❌


## ❓ FAQ

**Q: What HubSpot data can I access?**
Contacts, Companies, Deals, Tickets, Notes, Owners, and Pipelines. All data respects your HubSpot permissions.

**Q: Can I create and update records?**
Yes! Create contacts, deals, tickets, and notes. All through natural conversation.

**Q: How does authentication work?**
Uses a HubSpot Private App token (Bearer). Create a Private App in Settings > Integrations > Private Apps, copy the token, and paste it.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hubspot-cms-hub](https://vinkius.com/mcp/hubspot-cms-hub)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **HubSpot CMS Hub** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hubspot-cms-hub` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **HubSpot CMS Hub** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hubspot-cms-hub": {
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
