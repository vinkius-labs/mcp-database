# infrastructure MCP Servers

Explore the open database of **infrastructure** Model Context Protocol (MCP) servers.

| Tool Name | Description |
|-----------|-------------|
| [Agent Load Balancer Calculator](../mcps/agent-load-balancer-calculator.md) | Deterministic load balancing engine for distributing request rates across agent instances. |
| [Agent Rate Limiter Calculator](../mcps/agent-rate-limiter-calculator.md) | Deterministic distributed rate limiting for agentic workloads. |
| [Agora](../mcps/agora.md) | Orchestrate Agora real-time engagement — manage channels, monitor usage, and handle cloud recording directly from any AI agent. |
| [AI App Rate Limiting Economics](../mcps/ai-app-rate-limiting-economics.md) | Calculate the economic impact of rate-limiting strategies on AI infrastructure and revenue. |
| [API Key Rotation Manager](../mcps/api-key-rotation-manager.md) | Deterministic API key rotation to prevent rate limits and exhaustion. |
| [AWS API Gateway Throttling Calculator](../mcps/aws-api-gateway-throttling-calculator.md) | Calculate AWS API Gateway RPS, burst capacity, quotas, and operational limits. |
| [AWS Auto Scaling Group Capacity Calculator](../mcps/aws-auto-scaling-group-capacity-calculator.md) | Calculate exact instance requirements and scaling thresholds for AWS Auto Scaling Groups. |
| [AWS CloudFormation Stack Limits Calculator](../mcps/aws-cloudformation-stack-limits-calculator.md) | Verify AWS CloudFormation template compliance and calculate stack limits. |
| [AWS CloudWatch Logs Calculator](../mcps/aws-cloudwatch-logs-calculator.md) | Deterministic tool for estimating AWS CloudWatch Logs ingestion, storage, and service limits. |
| [AWS Config Coverage Calculator](../mcps/aws-config-coverage-calculator.md) | Calculate AWS Config rule limits, resource coverage, and infrastructure requirements. |
| [AWS Direct Connect Bandwidth Calculator](../mcps/aws-direct-connect-bandwidth-calculator.md) | Calculate AWS Direct Connect connection counts, redundancy requirements, and architectural limits. |
| [AWS Disaster Recovery Calculator](../mcps/aws-disaster-recovery-calculator.md) | Deterministic RTO and RPO estimation for AWS disaster recovery strategies. |
| [AWS ElastiCache Cluster Calculator](../mcps/aws-elasticache-cluster-calculator.md) | Deterministic sizing for AWS ElastiCache clusters including Redis and Memcached. |
| [AWS IoT Core Device & Limits Calculator](../mcps/aws-iot-core-device-limits-calculator.md) | Calculate AWS IoT Core messaging throughput, device scale, and resource limits. |
| [AWS MSK Partition & Throughput Calculator](../mcps/aws-msk-partition-throughput-calculator.md) | Deterministic sizing for AWS MSK clusters, calculating partitions, storage, and network limits. |
| [AWS Neptune Sizing Calculator](../mcps/aws-neptune-sizing-calculator.md) | Deterministic sizing for AWS Neptune graph databases. |
| [AWS SQS Calculator](../mcps/aws-sqs-calculator.md) | Calculate SQS payload strategies, throughput, and in-flight limits. |
| [AWS SSM Parameter Store Sizing Calculator](../mcps/aws-ssm-parameter-store-sizing-calculator.md) | Deterministic sizing and validation tool for AWS Systems Manager Parameter Store configurations. |
| [AWS Timestream Sizing Calculator](../mcps/aws-timestream-sizing-calculator.md) | Deterministic sizing engine for AWS Timestream workloads. |
| [Brunel Engineering Prover](../mcps/brunel-engineering-prover.md) | A warehouse system hit 3x its tested throughput on a Tuesday morning. Sorting stations jammed in 12 minutes. 4 hours of standstill. $180K in delayed shipments. The operations manual said 'should handle expected growth.' Nobody tested what 'expected' meant — or when it stopped being true. Brunel specified Box Tunnel's gradient to exactly 1 in 100. Every brick course counted. This tool forces that rigor: analyze what breaks at 10x/100x, map integration interfaces, specify exact tolerances, quantify risks with probability and blast radius, and challenge precedent at your scale. |
| [CIDR IP Calculator](../mcps/cidr-ip-calculator.md) | Perform IPv4 and IPv6 subnet mathematics, including network boundaries and host range calculations. |
| [Circuit Breaker State Manager](../mcps/circuit-breaker-state-manager.md) | Prevents cascading failures by managing service health states. |
| [Concrete Corrosion Predictor](../mcps/concrete-corrosion-predictor.md) | Estimates reinforcement corrosion rates, spalling time, and remaining service life. |
| [COO Operations Prover](../mcps/coo-operations-prover.md) | An operations plan said 'we will scale' without modeling arrival rates. It claims 'economies of scale' without a single cost data point. It writes SLAs that say 'best effort.' That is not operations — that is hope. This tool forces five COO-level operational axes: capacity modeling, failure isolation, cost leverage, process discipline, and accountability mechanisms. |
| [Deterministic Feature Flag Evaluator](../mcps/deterministic-feature-flag-evaluator.md) | Evaluate feature flags using consistent, hash-based logic to prevent session flicker. |
| [Docker Compose Validator](../mcps/docker-compose-validator.md) | Validate Docker Compose files for structural errors, port conflicts, and dependency cycles. |
| [ECS Task Sizing Calculator](../mcps/ecs-task-sizing-calculator.md) | Calculate precise AWS ECS task resources, EC2 capacity, and scaling configurations. |
| [European Data Localization Economics](../mcps/european-data-localization-economics.md) | Calculate the financial and operational impact of European data residency requirements. |
| [Idempotency Key Enforcer](../mcps/idempotency-key-enforcer.md) | Prevents duplicate execution of identical side-effectful operations using an in-memory LRU cache. |
| [Kubernetes Architecture Prover](../mcps/kubernetes-architecture-prover.md) | An AI generated Kubernetes manifests for a payment service. No resource requests or limits. No PodSecurityStandards. Single replica, no PDB. Zero NetworkPolicies — every pod could reach every other pod. The payment pod got OOM-killed at 3 AM by a logging sidecar with no memory ceiling. This tool forces resource governance, security hardening, reliability design, observability instrumentation, and network restriction on every workload. |
| [Kubernetes Resource Request Calculator](../mcps/kubernetes-resource-request-calculator.md) | Computes Kubernetes CPU/memory requests and limits from observed usage metrics (p50/p95/p99). |
| [Load Balancer Distributor](../mcps/load-balancer-distributor.md) | Deterministic simulation engine for evaluating load balancing algorithms. |
| [Message Queue Throughput Calculator](../mcps/message-queue-throughput-calculator.md) | Plan capacity for Kafka, RabbitMQ, or SQS by calculating consumer needs, backlog drain time, and concurrency. |
| [Multi-Tenant Isolation Calculator](../mcps/multi-tenant-isolation-calculator.md) | Deterministic resource isolation and quota calculator for multi-tenant environments. |
| [OpenSearch Shard Calculator](../mcps/opensearch-shard-calculator.md) | Deterministic AWS OpenSearch shard distribution and resource allocation calculator. |
| [PiLAB](../mcps/pilab.md) | Manage infrastructure and security via PiLAB — control PiVirt virtual machines, inspect PiTrust certificates, and oversee 3SO OAuth clients directly from any AI agent. |
| [Pub-Sub Topic Router](../mcps/pub-sub-topic-router.md) | Deterministic routing engine for hierarchical topic patterns and wildcard subscriptions. |
| [Rate Limiter State Calculator](../mcps/rate-limiter-state-calculator.md) | Deterministic engine for evaluating Token Bucket, Leaky Bucket, and sliding window rate limiting states. |
| [Security Audit Prover](../mcps/security-audit-prover.md) | An AI agent committed a Stripe API key to git, built SQL queries with string concatenation, and deployed an admin endpoint with no authentication — all in 4 minutes. The key was scraped from GitHub within 90 seconds. This tool forces input sanitization validation, secret management auditing, authentication enforcement, injection prevention, and dependency supply chain checks against OWASP Top 10. |
| [SNS Fanout & Filtering Calculator](../mcps/sns-fanout-filtering-calculator.md) | Calculate AWS SNS fanout, throughput, and filter policy complexity. |
| [Voice AI Economics Calculator](../mcps/voice-ai-economics-calculator.md) | Calculate voice AI integration costs, infrastructure needs, and UX value. |
| [vpc-cidr-calculator](../mcps/vpc-cidr-calculator.md) | Deterministic AWS VPC CIDR and subnet layout generator. |
| [WebSocket Capacity Planner](../mcps/websocket-capacity-planner.md) | Estimate WebSocket connection limits, server fleet requirements, and network overhead. |


---
*Auto-generated by Vinkius Registry Sync*