# Pet Medication Dose Splitter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pet-medication-dose-splitter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate the exact number and fraction of tablets needed for pet medication dosing.

## Description
The Pet Medication Dose Splitter is a precision utility designed to help pet owners and caregivers determine the exact physical dose of medication required. By inputting your pet's weight, the prescribed dosage rate (mg/kg), and the available pill strength (mg), the tool calculates the total milligrams needed and translates that into a practical instruction, such as 'give 1 and 3/4 tablets'. It uses `evaluate_pill_division` to identify if a split is easy or potentially inaccurate. If you encounter an awkward fraction like one-third of a tablet, the tool will provide a `difficultyWarning` and suggest alternative pill strengths that allow for a cleaner, safer dose. Always verify all calculations with your veterinarian before administering any medication.


## Available Tools (3)
- **fetch_safety_disclaimer**: Retrieves the mandatory safety warning
- **calculate_dosage_requirement**: Returns total mg required.

Determines the total milligrams of medication needed for a specific pet
- **evaluate_pill_division**: Returns whole pills, fraction, and ease of split.

Translates a required milligram dose into physical pill counts and identifies potential splitting inaccuracies


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pet Medication Dose Splitter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "My dog weighs 20kg. The vet prescribed 5mg/kg of this medication, and I have 10mg tablets. How many tablets should I give?"

**🤖 AI Agent:**
> For a 20kg dog at 5mg/kg, you need 100mg total. Using 10mg tablets, you should give 10 tablets.

---

**👤 You:**
> "I have a 5lb cat. The dose is 2mg/kg and the pill is 5mg. How much should I give?"

**🤖 AI Agent:**
> A 5lb weight is approximately 2.27kg. At 2mg/kg, the total dose needed is 4.54mg. Using 5mg tablets, you should give approximately 0.91 tablets (nearly one whole tablet).

---

**👤 You:**
> "Calculate the dose for a 10kg pet needing 2.5mg/kg using 5mg tablets."

**🤖 AI Agent:**
> The total dose required is 25mg. Using 5mg tablets, you should give exactly 5 tablets.


## ❓ FAQ

**Q: How accurate are the dosage calculations?**
The tool provides precise mathematical calculations based on your inputs. However, physical pill splitting can be imprecise. If a split is identified as difficult via `evaluate_pill_division`, please use caution and consult your vet.

**Q: What should I do if the pill fraction is hard to split?**
If the tool provides a warning about difficulty, it means the fraction (like 1/3) is not easily measurable. Check the `suggestedAlternatives` provided by the tool for different pill strengths that might result in an easier split.

**Q: Is this tool a substitute for professional veterinary advice?**
No. This tool is strictly for instructional purposes to assist with physical dosing. You must always verify the calculated dose and any splitting instructions with a licensed veterinarian before giving medication to your pet.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pet-medication-dose-splitter](https://vinkius.com/mcp/pet-medication-dose-splitter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pet Medication Dose Splitter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pet-medication-dose-splitter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pet Medication Dose Splitter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pet-medication-dose-splitter": {
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
