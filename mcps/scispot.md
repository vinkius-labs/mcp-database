# Scispot MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/scispot)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-management](../categories/data-management.md)

Automate cannabis laboratory testing via Scispot LIMS — manage samples, track analytical results, issue Certificates of Analysis, and monitor lab workflows from any AI agent.

## Description
Connect your **Scispot** API-first Cannabis Testing Laboratory LIMS to any AI agent and take full control of your laboratory operations, quality assurance workflows, and regulatory compliance through natural conversation.

### What you can do

- **Sample Management** — Track all cannabis samples received with chain of custody, testing priority, and real-time status updates
- **Test Panels** — Browse available analytical methods including potency, terpenes, pesticides, heavy metals, mycotoxins, and microbials
- **Analytical Results** — Access complete test findings with pass/fail determinations against state-specific regulatory limits
- **Certificates of Analysis** — Retrieve all issued CoAs with QR codes for consumer verification and automatic Metrc submission
- **Batch Traceability** — Monitor production batches through laboratory testing with full seed-to-sale linkage
- **Plate Management** — Oversee high-throughput batch processing with 96-well and 384-well plate tracking
- **Analytical Runs** — Review instrument run data including QC metrics, system suitability, and analyst assignments
- **Order Tracking** — Monitor client testing orders from submission through invoicing with ETA predictions
- **Instrument Health** — Verify calibration status, maintenance schedules, and operational readiness for HPLC, GC-MS, ICP-MS systems
- **Workflow Automation** — Track standardized laboratory processes from sample intake to CoA approval with bottleneck identification
- **Client Directory** — Access complete client profiles including license types, testing history, and custom panel configurations
- **Audit Trails** — Retrieve comprehensive operation logs for FDA 21 CFR Part 11 compliance and ISO/IEC 17025 inspection readiness

### How it works

1. Subscribe to this server
2. Enter your Scispot API key (generated from Account Settings)
3. Start managing your cannabis laboratory from Claude, Cursor, or any MCP-compatible client

No more navigating complex LIMS dashboards or manually reconciling sample queues. Your AI acts as a dedicated laboratory information systems analyst.

### Who is this for?

- **Laboratory Directors** — verify instrument calibration, review pending CoAs, monitor throughput metrics, and ensure ISO/IEC 17025 compliance without logging into Scispot
- **Quality Managers** — audit test results, investigate deviations, track non-conformance workflows, and prepare inspection documentation through conversational queries
- **Analytical Chemists** — check sample queues, verify test panel configurations, access run histories, and review QC metrics directly from the bench
- **Client Relations** — provide cultivators and processors with real-time sample status updates, CoA delivery confirmations, and order progress reports


## Available Tools
- **list_audit_logs**: Each audit log entry contains the precise timestamp (ISO 8601), performing user name and ID, action type (sample created, result modified, CoA issued, workflow step completed, user permission changed, instrument calibration recorded), affected record ID and type, previous and new values for any modifications, IP address and user agent, and justification comment (if required for critical changes). Fundamental for regulatory inspections, data integrity investigations, deviation root cause analysis, FDA 21 CFR Part 11 compliance, and ISO/IEC 17025 quality system requirements. AI agents use this to reconstruct event sequences during quality investigations, identify unauthorized or suspicious changes, monitor user activity patterns, generate audit-ready documentation packages, and demonstrate data integrity to regulatory inspectors.

List all audit trail entries for laboratory operations and data modifications
- **list_batches**: Each batch entry contains the batch ID, producing facility license number, batch size and unit of measure, cannabis product type, harvest or manufacture date, linked samples submitted for testing, batch testing status (pending, partial, complete, failed), final disposition (released, quarantined, rejected, destroyed, reworked), and seed-to-sale tracking identifiers (Metrc UID, state compliance tags). Essential for batch-level compliance monitoring, recall management, regulatory reporting, and inventory reconciliation. AI agents reference this when tracing contamination issues, verifying batch clearance for distribution, generating lot-based compliance reports, or investigating quality deviations.

List all cannabis production batches tracked through laboratory testing
- **list_certificates**: Each CoA record includes the certificate number, linked sample and batch, issuing laboratory name and accreditation number, comprehensive analytical results (potency profile with THC/CBD percentages, terpene fingerprint with individual concentrations, contaminant screening results for pesticides, heavy metals, mycotoxins, and microbials), regulatory compliance statement, authorized signatory name and signature, issuance date, expiration date, and QR code for consumer verification. Critical for product release decisions, regulatory audit documentation, consumer transparency programs, and integration with state traceability systems (Metrc) and retail platforms (WeedMaps). AI agents use this to verify CoA authenticity, confirm batch compliance status, generate client-facing documentation packages, and ensure automatic regulatory submissions.

List all Certificates of Analysis (CoA) issued by the laboratory
- **list_clients**: Each client record contains company name, license number and type (cultivation facility, processing plant, dispensary, distributor, third-party tester), primary contact information, account status (active, suspended, pending), billing terms, sample volume history, preferred communication methods, and any special testing requirements or custom panels configured. Essential for laboratory client relationship management, sample intake workflows, account-based reporting, and regulatory compliance documentation. AI agents should reference this when identifying sample ownership, generating client-specific reports, verifying active testing contracts, communicating results, and analyzing client testing patterns.

List all clients (cultivators, processors, retailers) using laboratory services
- **list_instruments**: Each instrument record contains the instrument name (HPLC system, GC-MS, ICP-MS, qPCR thermocycler, spectrophotometer), manufacturer, model number, serial number, installation location, calibration status, last calibration date, next scheduled maintenance, qualification status (IQ/OQ/PQ completion), associated test methods, and current operational status (active, under maintenance, offline, decommissioned). Critical for instrument qualification management, preventive maintenance scheduling, analytical data integrity verification, and regulatory inspection readiness. AI agents should reference this to verify instrument readiness before assigning tests, schedule calibration activities, troubleshoot analytical failures, and generate equipment utilization reports.

List all laboratory instruments with calibration and maintenance status
- **list_orders**: Each order record contains the order ID, requesting client company, order date, requested test panels, number of samples included, priority level (standard, rush, priority), order status (pending, in-progress, completed, invoiced), assigned laboratory team, estimated completion date, and billing information. Critical for order management, client communication, laboratory capacity planning, and revenue tracking. AI agents use this to monitor order progress, identify bottlenecks, prioritize workflow assignments, communicate status updates to clients, and generate order fulfillment reports.

List all testing orders and service requests from clients
- **list_plates**: Each plate entry contains the plate ID, plate format (96-well, 384-well), assay type assigned, number of samples loaded, number of standards and controls, run date, associated instrument, and processing status (prepared, in-run, completed, failed). Critical for managing high-volume testing operations, optimizing throughput, tracking reagent usage, and ensuring data integrity for multi-sample analytical runs. AI agents use this to monitor plate preparation status, identify incomplete runs, optimize well assignments, and troubleshoot analytical failures at the plate level.

List all laboratory plates used for batch sample processing
- **list_results**: Each result contains the result ID, linked sample and batch, test panel performed, comprehensive analytical findings (THC/CBD potency percentages, full terpene profiles, pesticide residue levels, heavy metal concentrations, mycotoxin detection, microbial counts), pass/fail determination against regulatory limits, analyst who performed the test, reviewer approval status, and date of completion. Fundamental for quality assurance workflows, client notification processes, regulatory data submissions, and product release decisions. AI agents should query this to verify sample compliance before releasing Certificates of Analysis, advising clients on product disposition, or preparing regulatory reports.

List all laboratory test results with complete analytical data
- **list_runs**: Each run entry contains the run ID, instrument name and type (HPLC, GC-MS, ICP-MS, spectrophotometer), method or assay performed, start and end timestamps, operating analyst or technician, number of samples processed, quality control results (standard recoveries, blank checks, duplicate precision), system suitability status, and overall run disposition (accepted, rejected, requires review). Essential for instrument utilization tracking, method performance monitoring, analyst productivity assessment, and regulatory audit preparation. AI agents should query this to verify run completion status, identify failed runs requiring reanalysis, schedule instrument maintenance, and generate throughput reports.

List all analytical runs executed on laboratory instruments
- **list_samples**: Each sample contains the unique sample ID, submitting client or cultivator, sample type (flower, edible, concentrate, topical, cartridge), received date, testing priority level, sample condition upon receipt, chain of custody documentation, and current testing status (received, in-progress, completed, failed, on-hold). Critical for laboratory workflow management, sample intake tracking, turnaround time monitoring, and seed-to-sale traceability compliance. AI agents use this to manage sample queues, predict completion dates, prioritize rush orders, and notify clients about status changes.

List all cannabis samples submitted for laboratory testing
- **list_tests**: Each test entry includes the test name (potency, terpenes, pesticides, heavy metals, mycotoxins, microbials, residual solvents, water activity, moisture content, homogeneity), test methodology (HPLC, GC-MS, ICP-MS, ELISA, qPCR, LC-MS/MS), accreditation status, standard turnaround time, pricing tier, and regulatory limits per jurisdiction. Essential for test panel configuration, method validation, ISO/IEC 17025 compliance, and state-specific cannabis testing requirements. AI agents reference this when configuring sample test orders, explaining testing scopes to clients, verifying analytical method accreditation, and ensuring compliance with regulatory testing mandates.

List all analytical test panels and methods available in the laboratory
- **list_workflows**: Each workflow entry contains the workflow name (sample intake and login, potency testing, contaminant screening, CoA review and approval, sample disposal, non-conformance investigation), step definitions with sequential order, assigned roles and responsibilities at each step, quality control checkpoints and decision gates, average completion time, current instances in progress, and bottleneck indicators. Essential for laboratory operations management, staff task assignment, process optimization, and ISO/IEC 17025 quality management system compliance. AI agents use this to guide technicians through standardized testing procedures, identify workflow bottlenecks causing delays, ensure quality checkpoints are not bypassed, and generate process efficiency reports.

List all laboratory workflow templates and active processes


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Scispot** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all cannabis samples currently in testing and their expected completion dates."

**🤖 AI Agent:**
> Scanning active laboratory queue via Scispot... I found 31 samples currently in testing across your analytical departments. Breakdown: 12 samples in Potency (HPLC) — average completion 2025-04-12, 8 samples in Terpene Profiling (GC-MS) — expected 2025-04-13, 6 samples in Pesticide Screening (LC-MS/MS) — due 2025-04-14, and 5 samples in Heavy Metals (ICP-MS) — targeting 2025-04-15. Four samples are marked as priority rush orders with 24-hour turnaround commitments. Would you like the detailed chain of custody and testing status for any specific client submissions?

---

**👤 You:**
> "List all pending Certificates of Analysis awaiting quality manager review and authorized signatory approval."

**🤖 AI Agent:**
> Reviewing CoA approval queue in Scispot... I found 9 Certificates of Analysis pending quality manager review and authorized signatory approval. Notable entries: CoA-2025-1047 (Blue Dream Batch BD-5521 — potency 29.1% THC, full contaminant panel clearance), CoA-2025-1048 (OG Kush Batch OG-4492 — terpene profile verified, pesticides non-detect), and CoA-2025-1051 (Sour Diesel Concentrate SD-C903 — residual solvents within state limits, mycotoxins passed). Average pending review time is 16 hours. Three are rush orders requiring release within 24 hours. Should I prioritize these for immediate signatory review?

---

**👤 You:**
> "Check the integration status with Metrc seed-to-sale tracking and automatic CoA publishing to state regulatory systems."

**🤖 AI Agent:**
> Querying Scispot integration health dashboard... All external platform connections are operational and compliant. Metrc seed-to-sale synchronization: last successful transmission 2025-04-09 15:47 UTC (189 CoAs published automatically, 0 submission failures, 3 pending retries for network timeouts). State regulatory API compliance: all mandatory test result submissions current through Q1 2025 reporting period. Automated CoA consumer portal (WeedMaps integration): 17 new certificates pushed in last 24 hours, all QR verification codes confirmed active and scannable. GLUE instrument data ingestion: 5 HPLC systems and 3 GC-MS instruments transmitting raw chromatograms successfully. No integration errors or data sync failures detected in past 14 days. Would you like me to generate a comprehensive integration performance summary for your records?


## ❓ FAQ

**Q: Can my AI automatically verify if a cannabis sample has passed all required tests and is ready for Certificate of Analysis issuance?**
Yes! Use the `list_results` tool to fetch all completed analytical findings for a specific sample. Your AI agent will respond with comprehensive pass/fail determinations across potency, terpenes, pesticides, heavy metals, mycotoxins, and microbial panels. Once all state-mandated tests show passing results, use `list_certificates` to verify CoA generation status and confirm automatic Metrc submission. Always verify regulatory limit compliance before releasing products to distribution or retail channels.

**Q: How do I quickly identify which laboratory instruments are approaching calibration expiry or require preventive maintenance?**
Simply ask the agent to run the `list_instruments` action. It will compile all analytical equipment tracked via Scispot GLUE integration with calibration status, last service date, next scheduled maintenance, IQ/OQ/PQ qualification records, and current operational state. The AI will proactively highlight any HPLC, GC-MS, ICP-MS, or other systems approaching calibration expiry or overdue for preventive maintenance. This ensures your laboratory maintains ISO/IEC 17025 compliance, analytical data integrity, and inspection readiness at all times.

**Q: Does the Scispot integration allow modifying test results, deleting samples, or revoking issued Certificates of Analysis?**
No. The current toolset focuses strictly on read-only querying and analytical operations — listing samples, reviewing results, checking certificates, monitoring workflows, and tracking instrument health. State alteration operations (modifying test data, deleting samples, revoking certificates, or changing approvals) are not currently exposed. This design assures your laboratory records remain secure against destructive queries, maintains complete audit trail integrity for regulatory inspections, and preserves data immutability required by FDA 21 CFR Part 11 and ISO/IEC 17025 standards.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/scispot](https://vinkius.com/mcp/scispot)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Scispot** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `scispot` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Scispot** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "scispot": {
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
