# PractiTest MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/practitest)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Bring your end-to-end QA management to your AI — list tests, instances, test sets, requirements, and trace logical software defects natively.

## Description
Connect your **PractiTest** workspaces to any AI agent and empower it to orchestrate the entire QA lifecycle from physical requirements tracing to defect mapping natively via chat conversations.

### What you can do

- **Test Cases & Sets** — Tell the AI to investigate any Test Case or Test Set, discovering exact preconditions and expected results (`list_tests`, `get_test`, `list_sets`)
- **Test Instances & Runs** — Retrieve deep execution histories pinpointing exactly which step caused a regression bounding PASSED/FAILED statuses (`list_runs`)
- **Requirements Tracking** — Audit physical system compliance extracting arrays dictating QA delivery thresholds (`list_requirements`)
- **Issue Mapping** — Find exact Software Defects bound natively to QA traces verifying complex failure logic (`list_issues`)

### How it works

1. Subscribe to this server
2. Supply your PractiTest Personal API Token and Project ID
3. Launch Claude, Cursor, or any compatible MCP client to instruct the AI with full test management autonomy

Forget moving between dashboard views trying to identify where a trace broke down. Simply ask the agent 'Why did the latest Payment flow fail?'

### Who is this for?

- **QA Automation Engineers** — verify integration outputs traversing test run histories instantaneously
- **Product Owners** — read live requirement statuses cross-referencing execution states mapped in the chat window
- **Software Developers** — dive into reported Issues parsing exact test execution failures natively before diving into code


## Available Tools (10)
- **list_tests**: List all test cases in a PractiTest project. PractiTest is an end-to-end test management platform with traceability from requirements to defects. Returns test names, IDs, statuses, custom fields, and traceability links. Uses JSON:API format
- **get_test**: Get full details of a PractiTest test case including name, description, preconditions, steps, expected results, custom fields, and requirement links
- **list_sets**: List all test sets in a PractiTest project. Test sets group test instances for execution. Returns set names, statuses, planned/actual dates, and assigned testers
- **get_set**: Get full details of a PractiTest test set including name, status, instances count, and execution summary
- **list_instances**: List all test instances in a PractiTest test set. Instances are test-set-specific copies of test cases. Returns instance IDs, test references, and last run statuses
- **list_runs**: List all runs for a PractiTest test instance. Runs record actual test execution results. Returns run IDs, statuses (PASSED/FAILED/BLOCKED/NOT_RUN/N_A), durations, and timestamps
- **list_requirements**: List all requirements in a PractiTest project. Requirements provide traceability to test cases and defects. Returns names, statuses, and linked test counts
- **list_issues**: List all issues (defects) in a PractiTest project. Returns issue names, statuses, severities, and linked test references
- **list_custom_fields**: List all custom fields in a PractiTest project. Returns field names, types, applicable entities, and possible values
- **list_users**: List all users in the PractiTest account. Returns user names, emails, roles, and statuses


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PractiTest** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all tests inside our active QA regression instance and find the ones mapped as failed."

**🤖 AI Agent:**
> I queried `list_runs` pulling executions. Exactly 3 Test Runs crashed the regression suite: Run ID `1202` (Login Flow Bypass), Run ID `1203` (Cart State Mismatch), and Run ID `1209` (Payment Fallback Failed). Should I extract step histories for #1209 using `get_test`?

---

**👤 You:**
> "Do we have any new custom fields we should be aware of inside the requirements area?"

**🤖 AI Agent:**
> I analyzed `list_custom_fields` crossing your dictionaries. Let's see... a new custom List field 'GDPR Category' (ID 402) was instantiated targeting Requirement entities with possible values strings: ['P1', 'P2', 'Ignore'].

---

**👤 You:**
> "Are there any open defects (issues) linked directly to testing scenarios surrounding multi-currency operations?"

**🤖 AI Agent:**
> Investigating `list_issues`, I see one highly relevant defect: 'EUR vs GBP Cart Rounding Error' (Issue ID #91). It carries a `High` severity and it strictly ties to instances in your 'Multicurrency V2' test cluster. Current status: UNRESOLVED.


## ❓ FAQ

**Q: Can the AI provide the exact step where a test case failed?**
Yes. If an execution failed, the agent uses `list_runs` for the instance. Since an instance maps directly to test steps, the AI inherently decodes the exact execution traces to show you the failing parameters.

**Q: Is PractiTest's requirement and issue tracing accessible to the AI?**
Yes. Tools like `list_requirements` and `list_issues` expose full traceability trees. You can ask exactly how many QA instances are mapped to Requirement 5.

**Q: Do I need to copy the project ID separately?**
Yes. In PractiTest, APIs execute cleanly isolated within specific Project instances. You must provide the numeric Project ID alongside your Personal Token so the underlying `pt-engine` binds queries strictly to that project.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/practitest](https://vinkius.com/mcp/practitest)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **PractiTest** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `practitest` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **PractiTest** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "practitest": {
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
