# HubSpot CMS Hub MCP Server

Manage blog posts, site pages, landing pages, authors, tags, and domains through natural conversation.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/hubspot-cms-hub)

## Overview
**Category:** industry-titans
**Tools Count:** 9

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


## Available Tools
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


## Installation & Usage

To install and use the **HubSpot CMS Hub** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hubspot-cms-hub](https://vinkius.com/mcp/hubspot-cms-hub)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
