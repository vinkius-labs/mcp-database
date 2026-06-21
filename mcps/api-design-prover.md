# API Design Prover MCP Server

An AI agent designed an API with GET /users/create. That single endpoint broke HTTP caching for 200 consumer services. No versioning. No error contract. Raw arrays on one route, wrapped objects on another. This tool forces semantic HTTP verbs, explicit versioning strategy, unified response envelopes, bounded pagination, and RFC 7807 error structures — before any code is written.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/api-design-prover)

## Overview
**Category:** productivity
**Tools Count:** 1

## Description
LLMs design APIs the way junior developers do — they pick verbs randomly, skip versioning, return different shapes on every endpoint, and dump error stack traces to the client. The result: 200 consumer services break when you refactor a single route. Clients write custom parsers for each endpoint. Nobody can paginate. Nobody can cache.

### The Problem

AI-generated API designs commit five protocol violations that compound into integration nightmares:

- **Verb Abuse** — GET /users/create. POST for reads. PUT for partial updates. The agent treats HTTP methods as cosmetic labels. Every misused verb breaks caching, idempotency guarantees, and proxy behavior for every consumer downstream.
- **Version Blindness** — No `/v1/` prefix. No header strategy. No deprecation policy. The first schema change becomes a breaking change for every integrated service. Rollback is impossible.
- **Shape Chaos** — Raw arrays on `/users`, wrapped objects on `/users/:id`, nested envelopes on `/users/:id/orders`. Three endpoints, three different response contracts. Client SDKs become unmaintainable.
- **Unbounded Lists** — `GET /orders` returns 47,000 rows. No cursor. No limit. No offset. The mobile client crashes. The CDN times out. The database locks.
- **Error Void** — Status 500 with `{ message: 'Something went wrong' }`. No error code. No RFC 7807. No machine-readable structure. The frontend shows a generic toast. Support tickets multiply.

### How It Works

API Design Prover validates every contract through 5 Decision Pivots:

1. **verbsSemantic** — GET is read-only and idempotent. POST creates. PUT replaces entirely. PATCH updates partially. DELETE removes. No exceptions. No 'it depends.'
2. **versioningDefined** — URL path (`/v1/`), header, or query param — with an explicit deprecation timeline. 'We'll version later' fails this pivot.
3. **responseConsistent** — Every endpoint returns `{ data: T, meta?: {}, errors?: [] }`. No raw arrays. No naked objects. One shape, every route.
4. **paginationHandled** — Collection endpoints use cursor or limit/offset with a hard maximum (e.g., max 100). `GET /users` without bounds fails immediately.
5. **errorContracted** — Errors follow RFC 7807 Problem Details: `{ type, title, status, detail, instance }`. String messages are rejected.

### The Verdict Matrix

| First Failing Pivot | Verdict | Meaning |
|---|---|---|
| verbsSemantic = false | VERB_ABUSE | HTTP semantics violated. Caching and idempotency broken. |
| versioningDefined = false | VERSION_MISSING | No versioning strategy. First change breaks all consumers. |
| responseConsistent = false | SHAPE_INCONSISTENT | Different response shapes per endpoint. Client SDKs unmaintainable. |
| paginationHandled = false | UNBOUNDED_RESPONSE | Lists return unlimited rows. Memory leaks and timeouts guaranteed. |
| errorContracted = false | ERROR_UNDEFINED | No standard error structure. Consumers cannot handle failures programmatically. |
| All pivots pass | API_PROVEN | Semantic verbs, versioned, consistent shape, paginated, RFC 7807 errors. |

### Why It Works

- **Tool calls are obligations.** The agent cannot claim 'versioning is handled' without naming the strategy. Filling the fields IS the design work.
- **Consistency engine catches contradictions.** Claiming `responseConsistent=true` while returning raw arrays on one route triggers rejection with a specific coaching message.
- **Semantic traps detect vague answers.** 'We follow REST best practices,' 'errors are handled by the framework,' or 'pagination will be added later' all trigger automatic rejection.


## Available Tools
- **validate_api_design**: You must: (1) MAP VERBS — every endpoint mapped to its HTTP verb with semantic correctness. GET = read (idempotent, cacheable, no side effects). POST = create (non-idempotent). PUT = full replace (idempotent, client sends entire resource). PATCH = partial update (only changed fields). DELETE = remove (idempotent). Any deviation from these semantics must be justified — "convenience" is not a justification, (2) DEFINE VERSIONING — method (URL path /v1/ preferred for visibility, header Accept-Version for flexibility, NEVER query params), what constitutes a breaking change (removing/renaming fields, changing types, altering error codes, removing endpoints), deprecation timeline (minimum 6 months), old version sunset policy, migration guides, (3) SHOW RESPONSE SHAPE — the EXACT JSON envelope every consumer receives on EVERY endpoint. Same structure for success, error, single resource, and list. Consumers should never need conditional parsing based on which endpoint they called, (4) SPECIFY PAGINATION — cursor-based (for real-time feeds, no count) or offset/limit (for stable datasets, with count). Max page size enforced server-side (never trust client). Default page size. Metadata returned (total, next_cursor, has_more), (5) CONTRACT ERRORS — structured error responses for every failure mode. RFC 7807 ({ type, title, status, detail, instance }) or equivalent with machine-readable code, human-readable message, correlation ID for tracing, and validation error array for 422s. If rejected, your API has a design flaw that will cost consumers integration time. Fix it.

Structured reflection tool for REST/HTTP API design (Stripe/GitHub-grade, RFC 7807 compliant). Forces the agent to define verb semantics, versioning with deprecation, response envelope shape, pagination bounds, and error contracts BEFORE implementing an endpoint. Catches Verb Abuse (POST for reads, GET with side effects, PUT for partial updates), Unversioned APIs (no deprecation policy, breaking consumers silently), Shape Inconsistency (different response structures per endpoint — success vs error vs list), Unbounded Responses (no pagination, no max page size — returning 100K records in one call), and Uncontracted Errors (500 with "Internal Server Error" string instead of structured RFC 7807). Call once per API surface. Based on Stripe/GitHub API guidelines, RFC 7807 Problem Details, and REST API Design Rulebook (Masse 2011)


## Installation & Usage

To install and use the **API Design Prover** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/api-design-prover](https://vinkius.com/mcp/api-design-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
