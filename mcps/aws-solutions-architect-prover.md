# AWS Solutions Architect Prover MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/aws-solutions-architect-prover)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [cloud-infrastructure](../categories/cloud-infrastructure.md)

A Principal-level AWS Solutions Architect reviewing every cloud decision your AI makes. 20 years of production scars — service sprawl, $40K NAT Gateway bills, IAM breaches, multi-region theater — packaged into a review that runs in seconds. Get the AWS discipline you would pay $300K/year to hire, applied to every architecture your team ships.

## Description
## What You Get

A Principal AWS Solutions Architect on demand. The kind of person AWS Enterprise Support sends to keynotes and to Fortune 500 CTO offices. The kind who has watched a customer burn $18K/month on unused NAT Gateways, prevented a startup from choosing EKS for their 3-person team, and shut down 27 breach attempts because IAM was scoped tight from Day 0.

This MCP puts that discipline behind every AWS architecture decision your team makes. Every time your AI generates a cloud design, it faces a senior review before you ship.

## Why It Pays for Itself

**AWS overspend is the industry default.** Flexera's State of the Cloud report puts wasted cloud spend at 32%. This Prover catches the top 5 causes: NAT Gateway ($32/mo idle + $0.045/GB you forgot), cross-AZ transfer ($0.01/GB compounding at scale), egress ($0.09/GB every time data leaves), VPC endpoints you should have bought, and service sprawl (EKS when Fargate works).

**IAM misconfiguration is the #1 root cause of AWS breaches.** Every `Resource: "*"` blocked at design time is a breach prevented before your team pushes code.

**Multi-region is theater when 99.95% is enough.** The Prover refuses Aurora Global Database, DynamoDB Global Tables, and Route 53 failover unless the availability SLO or data residency requirement earns them. Multi-AZ meets 99.95%. Save the multi-region tax for workloads that actually need it.

**Service sprawl is technical debt disguised as architecture.** Kinesis + MSK + EventBridge + SQS + SNS in the same design is not resilience — it is indecision. The Prover forces one primitive per role, defended against rejected alternatives.

## The Review Framework

The Senior SA runs your architecture through five gates. Skipping a gate is not allowed. The order is not negotiable.

| Gate | What the Senior SA Demands | What You Get |
|---|---|---|
| **1. Requirements Quantified** | RPS, p99 latency in ms, availability SLO in 9s, RTO/RPO in minutes, compliance scope. No marketing words. | Design decisions tied to real numbers, not aspirations. |
| **2. Blast Radius Mapped** | What fails at AZ, region, account, and service. Multi-region only when the SLO earns it. | Availability that matches your SLO — no theater, no gaps. |
| **3. Services Minimized** | Every service defended against a rejected alternative. Fargate over EKS unless you name why. SQS over Kinesis unless you name why. | The smallest AWS surface area that meets the SLOs — lower cost, lower ops burden. |
| **4. Real TCO Calculated** | NAT Gateway, cross-AZ, egress, VPC endpoints, PIOPS, support tier. Itemized. | An AWS bill you can defend to your CFO before you deploy. |
| **5. Security Designed In** | Least-privilege IAM (zero wildcards), KMS CMK with rotation, GuardDuty/Config/CloudTrail Day 0, Block Public Access on every bucket. | Compliance posture ready for SOC2, PCI-DSS, or HIPAA audit from Day 1. |

### The Verdict

```
Gate 1 fails → REQUIREMENT_HALLUCINATION   (numbers missing)
Gate 2 fails → BLAST_RADIUS_IGNORANCE      (failure domains unmapped)
Gate 3 fails → SERVICE_SPRAWL               (services stacked, not chosen)
Gate 4 fails → COST_HALLUCINATION           (hidden AWS fees ignored)
Gate 5 fails → SECURITY_AFTERTHOUGHT        (IAM wildcards, deferred controls)
All pass     → WELL_ARCHITECTED             (ship it)
```

Every rejection names the exact gate that failed and the concrete fix. No vague feedback. No hand-waving.

## Who This Is For

- **CTOs and Engineering VPs** who cannot afford a $30K/month AWS surprise, and cannot hire a Principal SA for every team.
- **Cloud and Platform teams** whose junior engineers ship AI-generated Terraform they cannot fully defend.
- **Startup founders** who need Fargate + RDS discipline, not EKS + MSK resume theater.
- **Regulated industries** (fintech, healthtech, gov) where IAM misconfiguration is not just a bug — it is a compliance finding.
- **Consultancies and MSPs** who need every proposal to survive a senior AWS review before it reaches the customer.

## What You Do Not Need

You do not need to configure AWS credentials. The Prover does not touch your AWS account, your bill, or your infrastructure. It reviews the architecture itself — the design, the reasoning, the tradeoffs — the way a Senior SA would in a whiteboard session. All the value, none of the access surface.


## Available Tools (1)
- **validate_aws_architecture**: The order is non-negotiable — most AWS failures come from executing these steps out of sequence. You must: (1) QUANTIFY REQUIREMENTS — extract concrete numbers. RPS peak and sustained, p50/p95/p99 latency in ms, availability SLO as 9s (99.9%, 99.95%, 99.99%), RTO in minutes, RPO in minutes, data volume in GB and growth rate, user count, compliance scope (PCI-DSS, HIPAA, SOC2). "Scalable" and "high-performance" are marketing words, not requirements, (2) MAP BLAST RADIUS — name what fails at every AWS scope level. AZ failure: how does the workload survive one AZ going dark? Region failure: what is the multi-region strategy and does the SLO justify it? Account failure: is production isolated in a dedicated account for blast radius bounding? Service failure: what happens when SQS is throttled or KMS is unavailable? "AWS handles it" is not a map, (3) MINIMIZE SERVICES — the best AWS service is no AWS service. For every service in your architecture, name the AWS alternative you REJECTED and the concrete reason. Fargate over EKS (control plane cost, ops burden), SQS over Kinesis (no replay > 24h need), Aurora over DynamoDB (relational needs). Reject Kafka on MSK unless you can name the ordering guarantee, throughput, or ecosystem tool that SQS cannot provide, (4) CALCULATE REAL TCO — itemize the AWS invoice. Compute + storage + NAT Gateway ($32/mo + $0.045/GB) + cross-AZ transfer ($0.01/GB) + egress ($0.09/GB) + VPC endpoints ($22/mo per endpoint per AZ) + PIOPS + CloudWatch + support tier + ops burden in engineer-hours. "Serverless is cheap" is a slogan. At sustained load, Lambda + API Gateway + DynamoDB frequently exceeds Fargate + ALB + Aurora by 2-3x, (5) DESIGN SECURITY IN — Day 0, not Day 90. IAM roles for compute (never access keys), policies scoped to specific ARNs (never `Resource: "*"`), aws:PrincipalTag and aws:ResourceTag condition keys, KMS CMK per data domain with rotation, S3 Block Public Access on every bucket, VPC endpoints for AWS service traffic, GuardDuty + Config + CloudTrail + Security Hub enabled on Day 0, Secrets Manager with automatic rotation, compliance conformance packs where scoped. If rejected, you violated the Algorithm sequence.

Structured reflection tool that forces execution of the 5-Step AWS Well-Architected Algorithm before validating any AWS cloud architecture decision. The algorithm must be executed IN ORDER — skipping steps is the most common failure. Catches Requirement Hallucination (accepting vague terms like "scalable", "high performance", "cloud-native" without extracting concrete SLIs, SLOs, RTO, or RPO — a senior architect never chooses a service before quantifying the numbers), Blast Radius Ignorance (proposing multi-region for a 200-user internal tool or single-AZ for a payment system — multi-AZ meets 99.95%, multi-region needs a business case like data residency or 99.99%+ SLO. "AWS handles it" is not a failure domain analysis), Service Sprawl (stacking Kinesis + MSK + EventBridge + SQS + SNS in the same architecture because the LLM cannot decide — a senior architect picks ONE messaging primitive matching volume, ordering, retention, and consumer model; ONE compute abstraction ordered from least operational burden (App Runner, Fargate) to most (EKS)), Cost Hallucination (calling Lambda "cheap" while ignoring API Gateway $3.50/M requests, DynamoDB WCU/RCU, VPC endpoints $22/mo per AZ, NAT Gateway $32/mo + $0.045/GB, cross-AZ $0.01/GB, egress $0.09/GB, and support tier — the TCO is the invoice, not the compute bill), and Security Afterthought (writing `Resource: "*"`, using access keys instead of IAM roles, deferring MFA and encryption to "later" — Day 0 is when least-privilege IAM, KMS CMK rotation, VPC endpoints, GuardDuty, Config, and CloudTrail must exist, not Day 90). Call once per major AWS architectural decision


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AWS Solutions Architect Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "We are building our new internal reporting tool on AWS. High performance, scalable, cloud-native. Stack: EKS for containers, MSK for events, Kinesis Data Streams for analytics, Aurora Global Database across us-east-1 and eu-west-1, Lambda for glue code because serverless is cheap. Security: IAM policies with `Action: 's3:*', Resource: '*'` for simplicity, we will lock it down later."

**🤖 AI Agent:**
> REQUIREMENT_HALLUCINATION + SERVICE_SPRAWL + SECURITY_AFTERTHOUGHT — Three gates failed in one paragraph. Gate 1: 'high performance, scalable, cloud-native' are marketing words. Give me RPS, p99 latency, availability SLO, RTO, RPO, and the actual user count. For an internal reporting tool this is almost certainly 100 RPS peak and 99.9% availability — which does NOT justify multi-region. Gate 3: EKS + MSK + Kinesis + Aurora Global + Lambda is five services doing overlapping jobs. Fargate + a single SQS queue + Aurora single-region would ship in two weeks and cost 60% less. Gate 5: `Action: 's3:*', Resource: '*'` is not simplicity — it is a breach waiting to happen. Scope to specific bucket ARNs. Use IAM roles, not access keys. Delete 'we will lock it down later' from the vocabulary. Security is Day 0.

---

**👤 You:**
> "Payment reconciliation service. Requirements: 250 RPS peak, p99 < 400ms, 99.95% availability, RTO 30 min, RPO 5 min, PCI-DSS scoped. Blast radius: multi-AZ within us-east-1 (three AZs), account-level isolation (payment-prod AWS account, no other workloads), RDS Aurora with cross-region read replica in us-west-2 for RPO 5min (async, warm standby, not active-active). Rejected multi-region active-active because 99.95% is met by multi-AZ and PCI scope grows with regions. Services: ECS Fargate (rejected EKS: no k8s-specific need, adds control plane cost and ops burden), Aurora PostgreSQL Serverless v2 (rejected DynamoDB: relational reconciliation needs joins), SQS FIFO (rejected Kinesis: no need for replay > 24h, no need for consumer parallelism > shards). TCO monthly: Fargate 4 vCPU x 4 tasks = $180, Aurora Serverless v2 avg 2 ACU = $195, SQS = $5, ALB = $22, VPC endpoints (S3, KMS, Secrets Manager) 3 x $22 = $66, CloudWatch = $30, cross-AZ replication ~50GB/day x $0.01 = $15, egress ~2GB/day x $0.09 = $5.4, AWS Business Support = $100 minimum, total ~$620/mo. Security: IAM roles for tasks, no access keys, KMS CMK per data domain with annual rotation, S3 Block Public Access on all buckets, GuardDuty enabled Day 0, AWS Config with PCI-DSS conformance pack, CloudTrail organization trail, Security Hub enabled, no `Action: '*'` in any policy, Secrets Manager for credentials with 30-day rotation."

**🤖 AI Agent:**
> WELL_ARCHITECTED — All five gates passed. Gate 1: SLIs and SLOs quantified (250 RPS, p99 < 400ms, 99.95%, RTO 30min, RPO 5min) with PCI-DSS scope. Gate 2: blast radius mapped at AZ, account, and region levels — multi-AZ earns the 99.95% SLO and cross-region async replica earns RPO 5min without inflating PCI scope. Gate 3: single choice per role (Fargate over EKS, Aurora Serverless v2 over DynamoDB, SQS FIFO over Kinesis) with rejected alternatives named. Gate 4: itemized $620/mo including VPC endpoints, cross-AZ, egress, and support — no hidden line items. Gate 5: IAM roles not keys, scoped policies with no wildcards, KMS CMK with rotation, Block Public Access, GuardDuty/Config/CloudTrail/Security Hub Day 0. Ship it.

---

**👤 You:**
> "We will use Lambda + API Gateway + DynamoDB for our new API. It handles 40 million requests per month, sustained load. Serverless is cheap so we do not need to calculate TCO in detail."

**🤖 AI Agent:**
> COST_HALLUCINATION — 'Serverless is cheap' is a slogan, not an architectural argument. At 40M requests/month sustained, here is the real invoice: API Gateway REST at $3.50/million = $140/mo, Lambda 512MB average 200ms = ~$8/mo compute (cheap here), DynamoDB on-demand at ~$1.25 per million writes and $0.25 per million reads for a 4:1 read/write ratio = $50/mo minimum plus storage, plus VPC endpoints if Lambda calls other services ($22/mo per endpoint per AZ x 3 AZs x 2 endpoints = $132/mo), plus NAT Gateway if any Lambda leaves the VPC to the internet ($32/mo + $0.045/GB). Realistic total: $380-$500/mo minimum. Compare: two Fargate tasks (1 vCPU, 2GB) behind an ALB with the same DynamoDB = ~$120/mo. At sustained load, 'serverless is cheap' inverts. Enumerate every line item before you sign off.


## ❓ FAQ

**Q: How much AWS spend can this typically save?**
The senior SA persona targets the five most expensive AWS mistakes: idle NAT Gateways ($32/mo each, often 3-6 in a VPC), forgotten cross-AZ transfer at scale, egress that quietly ranges from $500 to $50,000/mo, VPC endpoints omitted so every S3 call goes through NAT, and EKS control planes chosen where Fargate would suffice ($73/mo per cluster). Teams that put this review in front of every design typically recover 20-40% of AWS spend inside 90 days. The savings scale with the size of the AWS footprint.

**Q: Is this a replacement for AWS Trusted Advisor or Well-Architected Tool?**
No — those tools inspect deployed infrastructure. This Prover reviews the architecture BEFORE you deploy, at the design and reasoning stage where an AI just produced the plan. Trusted Advisor finds the idle NAT Gateway after it has cost you $384/year. The senior SA persona in this MCP catches it in the design conversation, before the CDK template is written. The two are complementary: this is your Day 0 review, Trusted Advisor is your Day 90 audit.

**Q: Does this need AWS credentials or access to my account?**
No. The senior SA persona works purely at the reasoning level — reviewing the design, the tradeoffs, and the justifications your AI produces. It never authenticates against AWS, never reads your account, never touches your infrastructure. There is nothing to configure and no attack surface to worry about. Approve it once, use it forever.

**Q: What does the senior SA actually reject?**
The five patterns that show up in every junior AWS review: (1) marketing words as requirements — 'scalable', 'high performance', 'cloud-native' with no RPS, no p99, no SLO; (2) multi-region as a default instead of a decision earned by 99.99%+ SLO or data residency; (3) service sprawl — Kinesis + MSK + EventBridge stacked because the AI could not commit; (4) 'serverless is cheap' as an argument without API Gateway, DynamoDB, VPC endpoint, and NAT Gateway line items; (5) `Resource: "*"`, access keys, and 'we will lock it down later'. Every rejection names the exact gate and the concrete fix.

**Q: How does the senior SA compare to the CTO Architect Prover?**
The CTO Architect Prover is cloud-agnostic — stack fitness, failure tolerance, migration safety, and observability at any provider or on-prem. The AWS Solutions Architect Prover is AWS-native — it knows the specific pricing of NAT Gateway, the shape of IAM policies, when EKS beats Fargate, and where Aurora Serverless v2 beats DynamoDB. Use the CTO Prover to decide whether you should be on AWS at all. Use this Prover once you are.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/aws-solutions-architect-prover](https://vinkius.com/mcp/aws-solutions-architect-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AWS Solutions Architect Prover** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `aws-solutions-architect-prover` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AWS Solutions Architect Prover** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "aws-solutions-architect-prover": {
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
