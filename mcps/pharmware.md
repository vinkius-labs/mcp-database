# PharmWare MCP Server

Automate cannabis laboratory testing via PharmWare — manage samples, track test results, issue Certificates of Analysis, and monitor lab workflows from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/pharmware)

## Overview
**Category:** erp-operations
**Tools Count:** 12

## Description
Connect your **PharmWare** Cannabis Testing Laboratory Platform to any AI agent and take full control of your laboratory operations, quality assurance, and compliance workflows through natural conversation.

### What you can do

- **Client Management** — List all cultivators, processors, and retailers who submit samples to your laboratory for testing
- **Sample Tracking** — Monitor all cannabis samples received with chain of custody, testing status, and priority levels
- **Test Panels** — Browse available analytical methods (potency, terpenes, pesticides, heavy metals, microbials, mycotoxins)
- **Test Results** — Access complete analytical findings with pass/fail determinations against regulatory limits
- **Certificates of Analysis** — Retrieve all issued CoAs with QR codes for consumer verification and regulatory compliance
- **Batch Traceability** — Track production batches through laboratory testing with seed-to-sale linkage
- **Laboratory Workflows** — Monitor active processes from sample intake through CoA issuance with QC checkpoints
- **Instrument Management** — Verify calibration status and maintenance schedules for HPLC, GC-MS, ICP-MS systems
- **Compliance Reports** — Generate regulatory submissions, monthly summaries, and trend analyses
- **Platform Integrations** — Check health of connections to WeedMaps, Metrc, BioTrack, and state regulatory APIs
- **User Administration** — Review laboratory staff roles, permissions, and training certifications
- **Audit Trails** — Access complete operation logs for FDA 21 CFR Part 11 compliance and inspection readiness

### How it works

1. Subscribe to this server
2. Enter your PharmWare API credentials (API Key and API Secret)
3. Start managing your cannabis laboratory from Claude, Cursor, or any MCP-compatible client

No more navigating complex LIMS interfaces or manually reconciling test queues. Your AI acts as a dedicated laboratory information systems analyst.

### Who is this for?

- **Laboratory Directors** — verify instrument calibration, review pending CoAs, and monitor throughput metrics without logging into PharmWare
- **Quality Managers** — audit test results, investigate deviations, and ensure ISO/IEC 17025 compliance through conversational queries
- **Analytical Chemists** — check sample queues, verify test panel configurations, and access batch histories directly from the bench
- **Client Relations** — provide cultivators and processors with real-time sample status updates and CoA delivery confirmations


## Available Tools
- **list_audit_logs**: Each audit log entry contains the timestamp, performing user, action type (sample created, result modified, CoA issued, workflow completed, user permission changed), affected record ID, previous and new values (for modifications), IP address, and justification comment (if required). Fundamental for regulatory inspections, data integrity investigations, deviation root cause analysis, and FDA 21 CFR Part 11 compliance. AI agents use this to reconstruct event sequences during quality investigations, identify unauthorized changes, and generate audit-ready documentation packages.

List all audit trail entries for laboratory operations and data changes
- **list_batches**: Each batch entry contains the batch ID, producing facility license number, batch size, cannabis product type, harvest or manufacture date, linked samples submitted for testing, batch testing status (pending, partial, complete), disposition (released, quarantined, rejected, destroyed), and seed-to-sale tracking identifiers. Essential for batch-level compliance monitoring, recall management, and regulatory reporting. AI agents reference this when tracing contamination issues, verifying batch clearance for distribution, or generating lot-based compliance reports.

List all cannabis batches tracked through laboratory testing
- **list_certificates**: Each CoA record includes the certificate number, linked sample and batch, issuing laboratory accreditation details, comprehensive analytical results (potency profile, terpene fingerprint, contaminant screening), regulatory compliance statement, authorized signatory, issuance date, and QR code for consumer verification. Critical for product release decisions, regulatory audits, and consumer transparency programs. AI agents use this to verify CoA authenticity, batch compliance status, and generate client-facing documentation packages.

List all Certificates of Analysis (CoA) issued by the laboratory
- **list_clients**: Each client record contains company name, license number, contact information, client type (cultivation facility, processing plant, dispensary, or third-party tester), account status, and billing information. Essential for laboratory client management, sample intake workflows, and regulatory compliance reporting. AI agents should reference this when identifying sample ownership, generating client-specific reports, or verifying active testing contracts.

List all clients (cultivators, processors, retailers) registered in PharmWare
- **list_instruments**: Each instrument record contains the instrument name (HPLC system, GC-MS, ICP-MS, spectrophotometer), manufacturer, model, serial number, installation location, calibration status, last calibration date, next scheduled maintenance, qualification status (IQ/OQ/PQ), and associated test methods. Critical for instrument qualification, preventive maintenance scheduling, and analytical data integrity. AI agents should reference this to verify instrument readiness before assigning tests, schedule calibration activities, or troubleshoot analytical failures.

List all laboratory instruments and equipment with calibration status
- **list_integrations**: Each integration record contains the platform name (WeedMaps, Metrc, BioTrack, Leaf Data Systems, state regulatory API), integration type (bidirectional data sync, CoA publishing, sample status updates, regulatory reporting), connection status, last synchronization timestamp, data mapping configuration, and error logs. Critical for multi-platform compliance, automated CoA distribution, and real-time regulatory reporting. AI agents reference this to verify integration health, troubleshoot sync failures, and ensure seamless data flow between laboratory systems and external platforms.

List all external system integrations (WeedMaps, state APIs, seed-to-sale platforms)
- **list_reports**: Each report entry includes the report type (monthly summary, regulatory submission, client statement, trend analysis, deviation investigation, corrective action report), generation date, reporting period, associated clients or samples, regulatory agency destination (if applicable), and distribution status. Essential for regulatory compliance documentation, client billing reconciliation, and laboratory performance analytics. AI agents use this to prepare state-mandated reports, analyze testing trends, and identify quality improvement opportunities.

List all laboratory reports and compliance documents generated
- **list_results**: Each result contains the result ID, linked sample, test panel performed, analytical findings (THC/CBD potency percentages, terpene concentrations, pesticide residue levels, heavy metal concentrations, mycotoxin detection), pass/fail determination against regulatory limits, analyst who performed the test, review status, and date of completion. Fundamental for quality assurance, client notification workflows, and regulatory data submissions. AI agents should query this to verify sample compliance before releasing Certificates of Analysis or advising clients on product disposition.

List all laboratory test results with analytical data
- **list_samples**: Each sample contains the unique sample ID, submitting client, sample type (flower, edible, concentrate, topical, cartridge), received date, testing priority (standard, rush, priority), sample condition upon receipt, chain of custody documentation, and current testing status (received, in-progress, completed, failed). Critical for laboratory workflow management, turnaround time tracking, and seed-to-sale traceability compliance. AI agents use this to monitor sample queues, predict completion dates, and alert clients about status changes.

List all cannabis samples submitted for laboratory testing
- **list_tests**: Each test entry includes the test name (potency, terpenes, pesticides, heavy metals, mycotoxins, microbials, residual solvents, water activity, moisture content), test method (HPLC, GC-MS, ICP-MS, ELISA, qPCR), accreditation status, turnaround time, pricing, and regulatory limits per jurisdiction. Essential for test panel configuration, method validation, and compliance with state-specific cannabis testing requirements. AI agents reference this when configuring sample test orders, explaining testing scopes to clients, or verifying analytical method accreditation.

List all test panels and analytical methods available in the laboratory
- **list_users**: Each user record contains the username, full name, assigned role (laboratory director, quality manager, analytical chemist, sample technician, administrative staff), department, permission level (read-only, data entry, review/approval, system administrator), account status (active, inactive, locked), last login date, and training certification expiry. Essential for access control management, audit trail integrity, and ISO/IEC 17025 personnel competency requirements. AI agents should query this to verify user authorization before approving test results, assigning quality-critical tasks, or conducting access reviews.

List all laboratory users with roles and permissions
- **list_workflows**: Each workflow entry includes the workflow name (sample intake, potency testing, contaminant screening, CoA review, sample disposal), step definitions, assigned roles and responsibilities, quality control checkpoints, average completion time, and current instances in progress. Essential for laboratory operations management, staff task assignment, and process optimization. AI agents use this to guide technicians through testing procedures, identify workflow bottlenecks, and ensure ISO/IEC 17025 quality management system compliance.

List all laboratory workflow templates and active processes


## Installation & Usage

To install and use the **PharmWare** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pharmware](https://vinkius.com/mcp/pharmware)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
