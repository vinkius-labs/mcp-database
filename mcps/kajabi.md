# Kajabi MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kajabi)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

All-in-one business platform for creators — manage courses, customers, and marketing via AI.

## Description
Empower your AI agent to orchestrate your entire digital product ecosystem with **Kajabi**. This unified server provides your agent with instant access to course management, customer relationship auditing, and sales monitoring. Your agent can instantly list your contacts, audit product offers, and retrieve detailed purchase history without you ever touching the Kajabi dashboard. Whether you are monitoring marketing performance or managing student access, your agent acts as a dedicated business operations manager through natural conversation.

### What you can do

- **Contact Intelligence** — List all contacts and retrieve detailed metadata to analyze your audience demographics.
- **Product Auditing** — Fetch complete information for your courses and digital products, including technical identifiers.
- **Sales Monitoring** — Retrieve lists of all financial orders and individual purchases to track revenue trends.
- **Offer Management** — List and inspect all active offers and their associated products in your account.
- **Site Content** — Access blog posts and other site data to monitor your content strategy and distribution.

### How it works

1. Subscribe to this server
2. Enter your Kajabi API Client ID and Client Secret
3. Start managing your digital business from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Course Creators & Solopreneurs** — instantly retrieve student statuses and audit sales during launch cycles.
- **Operations Managers** — automate business health checks and monitor customer growth through natural language.
- **Marketing Teams** — track the performance of different offers and analyze conversion trends without manual reports.
- **SaaS Developers** — integrate Kajabi workflows into internal tools via an AI-guided interface.
- **Customer Success Teams** — verify user purchases and product access levels to resolve inquiries faster.


## Available Tools (16)
- **get_contact_details**: Get contact details
- **get_offer_details**: Get offer details
- **get_product_details**: Get product details
- **list_contacts**: Automatically uses the default site. Provide site_id if you have multiple sites and want to query a specific one.

List all contacts
- **list_customers**: Provide site_id if you have multiple sites.

List all customers
- **list_offers**: Provide site_id if you have multiple sites.

List all offers
- **list_orders**: Provide site_id if you have multiple sites.

List all orders
- **list_blog_posts**: List all blog posts
- **list_products**: List all products
- **list_purchases**: Provide site_id if you have multiple sites.

List all purchases
- **list_sites**: Use this to get the site_id needed for filtering contacts, customers, offers, and orders.

List all sites
- **add_tag_to_contact**: Use list_tags to find available tag IDs and list_contacts to find contact IDs.

Add a tag to a contact
- **get_course_details**: Get course details
- **list_courses**: List all courses
- **list_tags**: Use tag IDs with add_tag_to_contact and remove_tag_from_contact to manage contact segmentation.

List all contact tags
- **remove_tag_from_contact**: Use list_contacts to find the contact ID and their current tags.

Remove a tag from a contact


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kajabi** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all contacts in my Kajabi account."

**🤖 AI Agent:**
> Retrieving your contact directory... You currently have 1,200 contacts in your database. Notable entries include active students and newsletter subscribers. Would you like to inspect a specific profile?

---

**👤 You:**
> "Show me all financial orders from the last month."

**🤖 AI Agent:**
> Fetching recent orders... I've identified 45 successful transactions from the last 30 days, totaling $4,500 in revenue. I can list the specific customer emails and amounts for you.

---

**👤 You:**
> "What courses are currently active in my account?"

**🤖 AI Agent:**
> Checking your product list... You have 3 active courses: 'AI Mastery', 'Digital Marketing 101', and 'Advanced Funnel Strategies'. Would you like the technical ID for any of these?


## ❓ FAQ

**Q: How do I list all active offers in my Kajabi account?**
Use the `list_offers` tool. It retrieves a comprehensive list of all offers you have configured, allowing you to audit pricing and product associations.

**Q: Can I see the technical details for a specific course?**
Yes! Use the `get_product_details` tool with the Product ID. Your agent will fetch the metadata, title, and current status for that specific digital product.

**Q: Does the integration allow auditing customer purchases?**
Absolutely. You can use the `list_purchases` and `list_orders` tools to monitor individual transaction history and verify which customers have access to specific offers.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kajabi](https://vinkius.com/mcp/kajabi)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Kajabi** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `kajabi` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Kajabi** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "kajabi": {
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
