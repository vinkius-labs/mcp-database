# Cloudflare MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cloudflare-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/cloudflare-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/cloudflare-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ship-it](../categories/ship-it.md)

Manage DNS, Workers, KV, Pages and firewall via Cloudflare — audit records, deploy config and inspect CDN analytics from any AI agent.

## Description
Connect your **Cloudflare** account to any AI agent and take full control of your DNS, edge computing, CDN and security infrastructure through natural conversation.

### What you can do

- **DNS Management** — List, create, update and delete DNS records (A, AAAA, CNAME, MX, TXT) with full control over TTL, priority and Cloudflare proxy status
- **Zone Discovery** — View all domains managed by Cloudflare with their plan type, SSL status, name server assignment and activation state
- **Workers Inventory** — List all deployed serverless Worker scripts with their last deployment timestamps and binding configurations
- **KV Storage** — Browse KV namespaces, read and write key-value pairs for Worker configuration, feature flags and edge-cached data
- **Pages Projects** — View all Cloudflare Pages deployments with their Git source, production branch and build status
- **Firewall Audit** — Review all WAF (Web Application Firewall) rules including filter expressions, actions (block, challenge, allow) and enabled status
- **Load Balancer Health** — Inspect load balancer configurations, origin pools, health check status and traffic steering policies
- **CDN Analytics** — View traffic analytics including request counts, bandwidth, threat mitigation, cache ratio and visitor statistics
- **IP Range Lookup** — Retrieve Cloudflare's complete IP address ranges for origin firewall allow-listing

### How it works

1. Subscribe to this server
2. Enter your Cloudflare API Token
3. Start managing your edge infrastructure from Claude, Cursor, or any MCP-compatible client

Stop clicking through the Cloudflare dashboard to check a DNS record or audit firewall rules. Your AI acts as a dedicated infrastructure engineer.

### Who is this for?

- **DevOps Engineers** — manage DNS records, audit firewall rules and check Worker deployments without leaving your terminal
- **Security Teams** — review WAF configurations, inspect threat analytics and verify IP allow-lists at edge
- **Full-Stack Developers** — read/write KV data for Workers, check Pages deployments and inspect load balancer health


## Available Tools
- **get_zone_analytics**: Use to audit CDN performance, identify traffic spikes and review threat mitigation.

Get analytics data for a Cloudflare zone
- **create_dns_record**: Requires the record type (A, AAAA, CNAME, MX, TXT, etc.), name (hostname) and content (IP address, target hostname, etc.). Optionally set TTL and whether to proxy through Cloudflare CDN (proxied=true enables the orange cloud).

Create a new DNS record in a Cloudflare zone
- **delete_dns_record**: Provide the zone ID and DNS record ID. This action cannot be undone — the record will be immediately removed from Cloudflare nameservers.

Delete a DNS record from a Cloudflare zone
- **list_dns_records**: ) configured for a specific zone. Each record has a type, name, content, TTL and proxied status (whether traffic goes through Cloudflare CDN). Optionally filter by record type (e.g. "A" for IPv4 addresses only).

List DNS records for a Cloudflare zone
- **list_firewall_rules**: Each rule defines a filter expression (e.g. "ip.src in {1.2.3.4}") and an action (block, challenge, allow, log, js_challenge). Use to audit your web application firewall configuration.

List firewall rules for a Cloudflare zone
- **get_kv_value**: Useful for reading Worker configuration, feature flags, cached API responses or session data. Provide the namespace ID and the key name.

Get a value from a Cloudflare KV namespace
- **get_zone**: Provide the zone ID.

Get details for a specific Cloudflare zone
- **list_cloudflare_ips**: Useful for configuring allow-lists, firewall rules and origin server access control to only permit traffic from Cloudflare proxies.

List Cloudflare IP address ranges
- **list_kv_namespaces**: KV namespaces are used by Workers for edge-cached data, configuration and session storage. Each namespace has an ID and title. Use the namespace ID to read/write key-value pairs.

List Cloudflare KV namespaces
- **list_load_balancers**: Cloudflare Load Balancing distributes traffic across multiple origin servers or regions based on health checks, geolocation and steering policies. Each load balancer has a name, target pools, fallback pool and health status.

List load balancers for a Cloudflare zone
- **list_pages_projects**: Cloudflare Pages is a full-stack hosting platform that connects to Git repositories and deploys static/SSG sites. Each project has a name, Git source, production branch and deployment count.

List Cloudflare Pages projects
- **put_kv_value**: Workers use this for edge-cached data, feature flags and configuration. Provide the namespace ID, key name and the value to store. The value can be any text (JSON, plain text, etc.).

Write a value to a Cloudflare KV namespace
- **update_dns_record**: Provide the zone ID and record ID, then any fields to change: name, content, TTL or proxied status. Only the fields you provide will be updated.

Update an existing DNS record
- **list_workers**: Workers are serverless JavaScript/Wasm functions that run at Cloudflare edge locations. Each worker has a name, last deployment timestamp, resource usage and optional bindings (KV, R2, D1). Provide the account ID (found in Cloudflare dashboard URL).

List Cloudflare Workers scripts
- **list_zones**: Each zone represents a domain that uses Cloudflare DNS and CDN services, with status (active, pending), plan type and verification status. Use the zone ID for subsequent DNS, firewall and analytics queries.

List all Cloudflare zones (domains)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cloudflare** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all A records for my example.com zone."

**🤖 AI Agent:**
> I've queried your example.com zone and found 4 A records: `app` → 203.0.113.10 (proxied), `api` → 203.0.113.11 (proxied), `staging` → 203.0.113.20 (DNS only) and `db` → 10.0.0.5 (DNS only). Would you like to modify any of these?

---

**👤 You:**
> "What Workers are currently deployed on my account?"

**🤖 AI Agent:**
> You have 3 Workers deployed: `api-gateway` (last deployed 2h ago, 1.2M invocations today), `image-resizer` (last deployed 5d ago, 340K invocations) and `auth-middleware` (last deployed 1 week ago, 890K invocations). The `api-gateway` is using the most CPU time.

---

**👤 You:**
> "What firewall rules are active on my production zone?"

**🤖 AI Agent:**
> Your production zone has 5 active firewall rules: 1) Block traffic from known bots (action: Block, enabled), 2) Challenge requests from high-risk countries (action: Challenge, enabled), 3) Allow internal team IPs (action: Allow, enabled), 4) Rate limit /api endpoints to 1000 req/5min per IP (action: Challenge, enabled), 5) Log all 4xx responses (action: Log, enabled). Would you like the full filter expressions for any rule?


## Installation & Usage

To install and use the **Cloudflare** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cloudflare-alternative](https://vinkius.com/mcp/cloudflare-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
