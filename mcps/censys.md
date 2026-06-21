# Censys MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/censys)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/censys-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/censys-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fort-knox](../categories/fort-knox.md)

Search internet-connected hosts, SSL certificates and attack surface — discover exposed services and vulnerabilities.

## Description
Connect to **Censys** and explore the world's largest internet scanning platform through natural conversation.

### What you can do

- **Host Search** — Search internet-facing hosts by service, port, OS, location and more
- **Host Details** — Get comprehensive info on any IP including all services and certificates
- **Host History** — View how a host's services and ports have changed over time
- **Certificate Search** — Find SSL/TLS certificates by issuer, subject, validity and more
- **Certificate Details** — Get full parsed certificate data by fingerprint
- **Certificate Hosts** — Find all hosts using a specific certificate
- **Aggregation** — Analyze distributions of services, countries and ASNs
- **Host Diff** — Compare two hosts to identify infrastructure differences

### How it works

1. Subscribe to this server
2. Enter your Censys API ID and Secret
3. Start exploring internet exposure data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Security Researchers** — discover exposed services, track vulnerabilities and analyze attack surfaces
- **Sysadmins** — monitor their organization's external exposure and identify misconfigurations
- **Threat Hunters** — track certificate usage, find related infrastructure and identify suspicious hosts


## Available Tools
- **aggregate_hosts**: Groups results by a specified field (e.g. "services.port", "location.country", "autonomous_system.name") and returns bucket counts. Useful for understanding the distribution of services, countries or ASNs matching a query.

Aggregate host search results by a specific field
- **get_account_info**: Useful for checking remaining API quota and account limits.

Get your Censys account information
- **get_certificate**: Returns the full parsed certificate including subject, issuer, validity, key info, extensions, CT logs and raw PEM data.

Get detailed info for a specific certificate by fingerprint
- **get_certificate_hosts**: Useful for finding all domains sharing a certificate (SANs). Returns IP addresses, ports and timestamps. Pagination via cursor.

Get hosts using a specific certificate
- **get_host**: Returns all open ports, service banners, TLS certificates, operating system detection, geolocation, autonomous system info and last updated timestamps.

Get detailed info for a specific IP address
- **get_host_history**: Shows how the host's services, ports and certificates have changed over time. Returns timestamps, services observed and changes detected. Pagination via cursor.

Get historical scan data for a specific IP
- **search_certificates**: Supports query syntax: issuer names, subject fields, serial numbers, validity dates, key algorithms, certificate transparency logs and more. Returns fingerprints, subjects, issuers, validity periods and key info.

Search for SSL/TLS certificates
- **search_hosts**: Supports powerful query syntax: service names (e.g. "nginx"), ports (e.g. "services.port:443"), protocols, operating systems, autonomous systems, geographic locations and more. Returns IP addresses, open ports, services, banners and locations. Pagination via cursor.

Search for internet-connected hosts
- **view_host_diff**: Useful for identifying changes between hosts or finding similar infrastructure.

Compare two hosts to see differences


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Censys** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find all nginx servers in Brazil."

**🤖 AI Agent:**
> Found 15,000+ hosts running nginx in Brazil. Top ports: 80 (HTTP), 443 (HTTPS), 8080 (HTTP alternate). Common OS: Ubuntu, Debian, CentOS. Sample IPs include servers in São Paulo, Rio de Janeiro and Brasília regions.

---

**👤 You:**
> "Get details for IP 8.8.8.8."

**🤖 AI Agent:**
> 8.8.8.8 (Google Public DNS): Open ports 53 (DNS), 443 (HTTPS/DoH). Services: DNS server, DNS over HTTPS. Location: Mountain View, CA, US. ASN: AS15169 (Google LLC). Last updated: 2 hours ago.

---

**👤 You:**
> "Find certificates issued by Let's Encrypt expiring this month."

**🤖 AI Agent:**
> Found 500+ Let's Encrypt certificates expiring this month. Top issuers: R3, E1, E5. Common subjects include domains ending in .com, .org and .net. Most use RSA 2048-bit or ECDSA P-256 keys.


## Installation & Usage

To install and use the **Censys** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/censys](https://vinkius.com/mcp/censys)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
