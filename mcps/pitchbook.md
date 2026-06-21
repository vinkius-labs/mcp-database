# PitchBook MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pitchbook)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [brain-trust](../categories/brain-trust.md)

AI private market intelligence: research companies, deals, investors, and funds via agents.

## Description
### What you can do

Connect AI agents to the PitchBook Direct Data API for comprehensive private market intelligence:

- **Search companies** across global private and public markets with industry and status filters
- **Get complete company profiles** with founding dates, headquarters, employees, and industry classifications
- **Track financing history** from Seed to Series D+ with deal sizes, investor syndicates, and valuations
- **Research deals** including VC investments, M&A transactions, LBOs, and public offerings
- **Analyze investors** — VC firms, PE firms, angels, family offices, and corporate venture arms
- **Explore investment funds** with AUM, vintage years, stage preferences, and sector focus
- **Find professionals** — founders, executives, board members, and key decision-makers
- **Identify limited partners** — pension funds, endowments, sovereign wealth funds, and family offices
- **Get AI-powered VC exit predictions** for portfolio companies with IPO and acquisition probability scores

### How it works

1. **Connect your PitchBook account** via API token from your Direct Data subscription
2. **Ask your AI agent** to research companies, analyze deal flow, or map investor networks
3. **Natural language commands** replace manual PitchBook platform searches
4. **Structured market data** returned in formatted responses with pagination metadata

### Who is this for?

Essential for **venture capitalists**, **private equity professionals**, **investment bankers**, **corporate development teams**, **limited partners**, **fundraisers**, **management consultants**, and **financial journalists**. Let AI agents perform company due diligence, track competitor fundraising, identify potential acquirers or investors, research LP backgrounds, map professional networks, and assess exit probabilities. Perfect for professionals who need to answer questions like 'What companies raised Series A in AI/ML last quarter?', 'Which PE firms are most active in healthcare buyouts?', or 'What is the predicted exit probability for this portfolio company?'


## Available Tools
- **get_companies**: Returns company names, statuses, industries, locations, and key identifiers. Use optional filters to narrow results by industry, location, company status (Active, Acquired, Closed, IPO), or other attributes. Results follow JSON:API format with pagination metadata. Use this to find startups, established companies, or emerging players in specific sectors.

Search and list companies in the PitchBook private market database
- **get_company_financing**: Each round shows announced date, amount raised (USD), lead investors, participating investors, deal structure, and post-money valuation if disclosed. Requires the company ID from get_companies or get_company results. Use this to analyze a company's fundraising trajectory, total capital raised, and investor syndicate composition.

Get complete funding/financing history for a specific company
- **get_company**: Requires the company ID from get_companies results. Use this for comprehensive company due diligence and background research.

Get detailed profile for a specific company in PitchBook
- **get_deal**: ), announced date, deal size (if disclosed), all participating companies, investors, funds, and financial advisors, deal terms and structure, and any publicly available valuation data. Requires the deal ID from get_deals results. Use this for deep analysis of specific transactions, competitive deal intelligence, or investment thesis validation.

Get detailed information about a specific deal/transaction
- **get_deals**: Returns deal names, types (VC Deal, M&A, IPO, LBO, etc.), announced dates, deal sizes (if disclosed), and participating entities. Use optional filters to narrow by deal type, industry, location, or date range. Results follow JSON:API format with pagination metadata. Use this to track recent deal activity, identify active investors, or monitor M&A trends.

Search and list deals (VC investments, M&A, offerings) in PitchBook
- **get_fund**: Requires the fund ID from get_funds results. Use this for fund-level due diligence, LP allocation decisions, or understanding fund investment strategies.

Get detailed information about a specific investment fund
- **get_funds**: Returns fund names, types, sizes (if disclosed), vintages (year), investor/firm names, and key identifiers. Use optional filters to narrow by fund type, vintage year, fund size, or investor. Use this to analyze fund raising trends, identify active funds in a vintage, or research fund managers for LP due diligence.

Search and list investment funds in PitchBook
- **get_investor**: ), sector focus areas, geographic focus, notable portfolio companies, and key personnel. Requires the investor ID from get_investors results. Use this for thorough investor due diligence, LP fundraising research, or understanding investment firm strategies.

Get detailed profile for a specific investor/firm
- **get_investors**: Returns investor names, types (VC, PE, Angel, Corporate VC, etc.), headquarters locations, fund counts, total AUM (if disclosed), and key identifiers. Use optional filters to narrow by investor type, location, or fund size. Use this to find potential investors, research competitor firms, or map the investment landscape.

Search and list investors (VC firms, angels, PE firms) in PitchBook
- **get_limited_partners**: Returns LP names, types, locations, total commitments (if disclosed), and key identifiers. Use optional filters to narrow by LP type, location, or commitment size. Use this for LP fundraising research, understanding LP allocation trends, or identifying potential fund investors.

Search and list limited partners (LPs) in PitchBook
- **get_professional**: Requires the professional ID from get_professionals results. Use this for thorough individual due diligence, founder background checks, or mapping professional deal flow networks.

Get detailed profile for a specific professional
- **get_professionals**: Returns names, current titles, organizational affiliations, locations, and key identifiers. Use optional filters to narrow by title, organization, or location. Use this to find key decision-makers, research founder backgrounds, or map professional networks in the startup ecosystem.

Search and list professionals (founders, executives, investors) in PitchBook
- **get_vc_exit_predictor**: Returns the predicted exit likelihood score, predicted exit type (IPO, Acquisition, Secondary), predicted exit timeframe, and comparable exits used in the model. Requires the company ID from get_companies results. Use this to assess exit probability for portfolio companies, identify likely IPO candidates, or evaluate acquisition potential of target companies. Note: This is a predictive model output, not a guaranteed outcome.

Get AI-powered VC exit prediction for a specific company


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PitchBook** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for artificial intelligence startups that raised a Series A round in the last 6 months."

**🤖 AI Agent:**
> I have retrieved the latest funding data for AI startups via PitchBook, highlighting companies such as [Company Name] and detailed valuations.


## ❓ FAQ

**Q: Is a PitchBook Direct Data API subscription required?**
Yes. This integration requires an active PitchBook Direct Data API token.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pitchbook](https://vinkius.com/mcp/pitchbook)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **PitchBook** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `pitchbook` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **PitchBook** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pitchbook": {
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
