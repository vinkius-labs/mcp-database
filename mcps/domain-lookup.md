# Domain Lookup MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/domain-lookup)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Keyless domain availability and DNS intelligence — check if a domain is free, read its registry record, resolve DNS, and browse TLDs, straight from the official IANA and Cloudflare sources.

## Description
Connect any AI agent to **official domain registration data** — the same RDAP records that registries publish for every TLD, plus live DNS over HTTPS. No key, no account, no rate limits to manage.

### What you can do

- **Check availability** — ask "is example.com free?" and get an answer from the registry that actually owns the TLD. The engine resolves the right RDAP server per TLD through the IANA bootstrap, so a `.com` query hits Verisign and a `.io` query hits Identity Digital, automatically.
- **Read the full record** — registrar, creation and expiry dates with days remaining, EPP statuses, authoritative nameservers, public contacts and DNSSEC signing.
- **Check many at once** — paste a list of candidates and get an availability summary for the whole batch, useful when comparing names.

### How it decides

For the 1200+ TLDs that publish RDAP, the answer is authoritative: HTTP 200 means registered, 404 means free. Some TLDs publish no RDAP at all; for those the engine falls back to DNS and **labels the answer as inferred**, so an agent never mistakes a guess for a fact. Every response carries an `authoritative` flag and the method used.

### Also included

- **DNS lookups** — A, AAAA, MX, TXT, NS, CNAME, SOA, CAA, SRV and PTR records via Cloudflare DNS-over-HTTPS, with validation status.
- **DNSSEC checks** — the DS record from the parent zone against the domain's own DNSKEYs, to see whether the delegation chain is complete.
- **TLD browser** — IANA's full list of top-level domains, paged and searchable, showing which ones support authoritative lookup.
- **Domain parsing** — splits a hostname into registrable domain, public suffix and subdomain using the Public Suffix List, so `www.example.co.uk` is handled correctly.
- **Name suggestions** — given a base name, generates and checks variants across popular TLDs and common prefixes, returning only the ones that look free.


## Available Tools (8)
- **check_multiple_domains**: Use it when comparing candidates — "which of these names are still free". Each row carries its own authoritative flag, because a batch can mix TLDs with RDAP and TLDs without it.

Check many domain names at once and get an availability summary for the whole list
- **get_dnssec_status**: A signed domain with both records can be validated end to end by resolvers; a DS with no matching DNSKEY means validation would fail. Use this to check whether a domain is protected against DNS spoofing.

Check whether a domain is DNSSEC-signed, with its DS and DNSKEY records
- **get_domain_info**: Use this after check_domain_availability when you need the detail behind a taken domain. Registries differ in how much they publish — .com gives full dates and a registrar, some ccTLDs give only the nameservers, and DENIC (.de) publishes no creation date at all. Missing fields mean "not published by this registry", not "unknown". If the domain is free, registered is false and the other fields are empty.

Full registration record for a domain — registrar, creation and expiry dates, nameservers, statuses, DNSSEC
- **list_top_level_domains**: Each row says whether that TLD has an RDAP server, which is what makes a check_domain_availability answer authoritative for it. Search narrows by substring, so search=io finds .io and every TLD containing it. Use this to discover TLDs or to check whether an availability answer for a given TLD will be a fact or an inference.

Browse the official IANA list of top-level domains, with which ones support authoritative lookup
- **lookup_dns_records**: For A and AAAA the CNAME is reported separately so you see the effective host. The trusted field says whether the answer was cryptographically validated. Use this for "where does this domain point" and "what are its mail servers" — a domain with no A records and no MX is parked or unused. Supported types: A, AAAA, NS, MX, TXT, CNAME, SOA, CAA, SRV, PTR.

Live DNS records for a domain — A, AAAA, MX, TXT, NS, CNAME, CAA and more, via DNS-over-HTTPS
- **parse_domain**: example.co.uk it returns the registrable domain example.co.uk, the suffix co.uk and the subdomain www. Naive splits get this wrong because some effective TLDs have two labels. Use this before any other lookup when the input might be a subdomain, since RDAP and DNS work on the registrable domain.

Split a hostname into its pieces — registrable domain, public suffix and subdomain
- **suggest_domain_names**: g. "mybrand") and get back the variants that look free. The engine combines the name with the TLDs you list — or a popular default set (com, io, ai, app, dev, co, net, org, xyz, so, sh, me) — and with prefixes like get-, try- and the -hq suffix, then filters to the ones that are available. Use it for "help me name my project". Every suggestion keeps its authoritative flag: names from TLDs without RDAP are DNS-inferred and should be confirmed at a registrar before you fall in love with them.

Find available variants of a brand or idea across popular TLDs and common prefixes
- **check_domain_availability**: g. example.com) and reports whether it is registered or available. For most TLDs the answer is authoritative: it comes from the official RDAP server for that TLD, resolved through the IANA bootstrap. Some ccTLDs publish no RDAP at all; for those the answer comes from DNS and is labelled authoritative: no, so read that field. This is the tool for "is this domain taken".

Check whether a domain name is free to register — authoritative from the registry that owns the TLD, keyless


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Domain Lookup** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is mybrand.com available? If not, what does its registration record show?"

**🤖 AI Agent:**
> check_domain_availability answers from the .com registry. If it is taken, get_domain_info returns the registrar, the creation and expiry dates with days remaining, the EPP statuses and the authoritative nameservers.

---

**👤 You:**
> "Find me an available name for a project called lumen, across a few good TLDs."

**🤖 AI Agent:**
> suggest_domain_names combines the base with popular TLDs and prefixes like get- and try-, then returns only the variants that look free, each with its confidence level.

---

**👤 You:**
> "Where does example.com point, and is it DNSSEC-signed?"

**🤖 AI Agent:**
> lookup_dns_records resolves A, AAAA, MX, TXT and other record types via Cloudflare DNS-over-HTTPS, and get_dnssec_status reads the DS record from the parent zone against the domain's own DNSKEYs.


## ❓ FAQ

**Q: Do I need an API key?**
No. This reads the official RDAP servers each registry publishes, the IANA TLD list, the Public Suffix List and Cloudflare DNS-over-HTTPS. All are public and require no key or account.

**Q: How accurate is the availability answer?**
For TLDs that publish RDAP — over 1200 of them, including .com, .net, .org and most new extensions — the answer comes from the registry itself and is authoritative. A few TLDs publish no RDAP; those fall back to DNS and are returned with authoritative: no, so you know to confirm at a registrar before registering.

**Q: Why does one domain answer authoritatively and another does not?**
Each TLD is run by its own registry, and each registry decides whether to publish RDAP. The engine looks up the right server per TLD through the IANA bootstrap, so it always asks the registry that owns the name. When no server exists, it says so instead of guessing, and gives the best available DNS-based signal.

**Q: Can it register a domain for me?**
No, and deliberately so. This is read-only intelligence: it tells you what is free and what a taken domain looks like. To register, take the name it found to the registrar of your choice.

**Q: Does it work with international domain names?**
Yes. Unicode names are converted to their punycode A-label form before any registry or DNS query, and both forms are returned so you can see the name as written and as the network sees it.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/domain-lookup](https://vinkius.com/en/ai-agent-connect/domain-lookup)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Domain Lookup** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `domain-lookup` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Domain Lookup** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "domain-lookup": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
