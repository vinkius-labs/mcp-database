# Kajabi MCP Server

All-in-one business platform for creators — manage courses, customers, and marketing via AI.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/kajabi)

## Overview
**Category:** ecommerce
**Tools Count:** 16

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


## Available Tools
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


## Installation & Usage

To install and use the **Kajabi** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kajabi](https://vinkius.com/mcp/kajabi)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
