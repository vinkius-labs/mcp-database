# Laravel Excellence Prover MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/laravel-excellence-prover)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

AI agents generate Laravel code with N+1 queries, fat controllers, workarounds, and mass assignment holes. This tool forces excellence: optimize queries, use the framework idiomatically, separate responsibilities, guard mass assignment, and respect architecture. Zero tolerance for workarounds.

## Description
AI agents producing Laravel code consistently fail at framework mastery. They write code that works but violates every principle a senior Laravel developer upholds. The result: N+1 performance disasters, workarounds that bypass the framework's built-in solutions, controllers bloated with business logic, mass assignment vulnerabilities waiting to be exploited, and architectural patterns that crumble under scale.

### The Problem It Solves

AI-generated Laravel code fails on five axes:

- **N+1 queries** — Accessing `$user->posts` inside a `@foreach` loop without `with('posts')`. Each iteration fires a separate SQL query. On 100 users, that's 101 queries instead of 2. The agent never calls `Model::preventLazyLoading()` and never audits Blade views for implicit relationship access.
- **Workarounds** — Manual validation arrays instead of FormRequests. `Model::find($id)` with null checks instead of Route model binding. Inline authorization instead of Policies. Manual JSON responses instead of API Resources. The agent reinvents what Laravel already provides — badly.
- **Fat controllers** — Controllers with 50+ lines containing business logic, validation, database transactions, email sending, and cache management. The Single Responsibility Principle treated as a suggestion. Business logic should live in Service or Action classes, never in controllers.
- **Mass assignment exposure** — `$request->all()` passed directly to `create()`. `$guarded = []` on models. Missing `$fillable` arrays. No FormRequest to whitelist fields. An attacker injects `is_admin=true` and the application blindly saves it.
- **Architecture violations** — `env()` calls in application code (breaks after `config:cache`). Missing `DB::transaction()` on multi-model writes. Untyped properties and methods. No query scopes. No API Resources. Events firing before transaction commits.

### How It Works

Laravel Excellence Prover uses 5 Decision Pivots — boolean checkpoints that force the agent to prove its code meets senior-level standards:

1. **queryOptimized** — No N+1 ANYWHERE — including Blade views. Eager loading, scopes, preventLazyLoading.
2. **noWorkarounds** — Every solution uses the Laravel-idiomatic approach. The framework provides it — USE it.
3. **responsibilitySeparated** — Controller handles HTTP. FormRequest validates. Service/Action executes. Model defines data. Event handles side effects.
4. **massAssignmentSafe** — Explicit `$fillable`, `$request->validated()`, sensitive fields excluded.
5. **architectureRespected** — FormRequests, DB transactions, typed code, `config()` not `env()`, route model binding, API Resources.

### Why It Works

- **Tool calls are obligations.** The agent can ignore "use eager loading" in a system prompt. It cannot ignore a schema that demands naming every relationship access, proving no workarounds exist, and mapping the responsibility chain.
- **The priority cascade.** N+1 is checked first because it's the most common and damaging performance issue. A fat controller with fast queries is bad. A thin controller with N+1 is a production outage.
- **Semantic traps.** The engine catches Laravel-specific anti-patterns: vague claims ("follows best practices"), raw SQL without justification, `env()` in application code, generic responsibility claims ("thin controllers"), and platitude conclusions.
- **Zero workaround tolerance.** If Laravel provides a built-in solution (FormRequest, Route model binding, Policies, Events, API Resources), using a manual alternative is a REJECTION. Senior Laravel means knowing the framework deeply enough to never reinvent it.


## Available Tools
- **validate_laravel_excellence**: PILLAR I — BEST PRACTICES: (1) prove NO WORKAROUNDS — every feature uses the Laravel-idiomatic solution (Eloquent scopes, FormRequests, Policies, Middleware, Events, API Resources, route model binding). If Laravel provides it, use it, (2) map RESPONSIBILITIES — Controller handles HTTP only, FormRequest validates, Service/Action executes logic, Model defines data, Event handles side effects. Business logic in the controller is a fat controller, (3) enforce MASS ASSIGNMENT protection — explicit $fillable, $request->validated(), sensitive fields excluded, never $request->all(), never $guarded = [], never Model::unguard() in production. PILLAR II — MAXIMUM PERFORMANCE: (4) demonstrate QUERY OPTIMIZATION — eager loading via with(), Model::preventLazyLoading(), scopes for reusable filters, no N+1 anywhere including Blade views, (5) detail PERFORMANCE STRATEGY — Cache::remember() for expensive reads, paginate()/simplePaginate() for lists, chunk()/cursor() for background processing, select() for needed columns only, Jobs for heavy I/O. PILLAR III — ZERO TOLERANCE: (6) verify ARCHITECTURE — config() not env(), DB::transaction() for multi-writes, typed properties, API Resources for JSON, no dd()/dump(), no magic values (use Enums/constants), $afterCommit on listeners in transactions. If rejected, fix the gap before shipping.

Structured reflection tool for Laravel development excellence — enforces three pillars: best practices (framework idioms), maximum performance (query and cache optimization), and zero tolerance (no workarounds, no code smells). Catches N+1 Detected (lazy-loading relationships in loops or Blade views — "$users = User::all(); foreach ($users as $user) { $user->posts; }" fires N+1 queries. With 1,000 users: 1 query for users + 1,000 queries for posts = 1,001 database hits. Model::preventLazyLoading() in AppServiceProvider catches this in development. "User::with('posts')->get()" fires exactly 2 queries regardless of user count), Workaround Detected (manual implementations bypassing framework features — "if ($request->input('email') && filter_var(...))" is a manual validation workaround. Laravel provides FormRequest with $rules = ['email' => 'required|email:rfc,dns']. Manual file_get_contents() instead of Http::get(). Manual SQL instead of Eloquent. If Laravel provides it, use it — your manual version will be worse), Fat Controller (business logic inside the controller instead of services — "public function store(Request $request) { // 80 lines of validation, calculation, email sending, cache invalidation }" is a fat controller. Controller: HTTP in/out. FormRequest: validation. Service/Action: logic. Model: data. Event/Listener: side effects. Each responsibility in its place), Mass Assignment Unsafe (using $request->all() or $guarded = [] — "User::create($request->all())" allows an attacker to POST is_admin=1 and become admin. $fillable must be explicit. Input must come from $request->validated() via FormRequest. Sensitive fields (is_admin, role, email_verified_at) excluded from mass assignment. Model::unguard() only in database seeders, never in production code), and Architecture Violated (env() in application code, no DB::transaction(), raw responses — "env('STRIPE_KEY')" works locally but returns null in production with config cache. Use config('services.stripe.key'). Multi-model writes without DB::transaction() = partial failures. JSON responses without API Resources = coupled, unversioned output). Call once per feature, endpoint, or refactoring decision


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Laravel Excellence Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I need to list all orders with their products for an admin dashboard. I'll use Order::all() and then loop through to get products in the Blade view."

**🤖 AI Agent:**
> Verdict: N_PLUS_ONE_DETECTED. Order::all() loads orders without products. Each $order->products in Blade fires a separate query. 100 orders = 101 queries. Fix: Order::with('products')->paginate(25). Enable Model::preventLazyLoading() in AppServiceProvider to catch this at dev time. Use withCount('products') if you only need the count.

---

**👤 You:**
> "POST /api/orders: StoreOrderRequest validates input. CreateOrderAction receives DTO, wraps Order + OrderItems in DB::transaction(), returns Order. Order model has $fillable = ['user_id', 'total', 'status']. Queries: Order::with('items.product') for response. Event: OrderCreated dispatched after commit via $afterCommit. Response via OrderResource."

**🤖 AI Agent:**
> Verdict: CODE_PROVEN. Queries optimized (with('items.product')). No workarounds — FormRequest, Action, DB::transaction(), API Resource, Event. Responsibilities separated (Controller→FormRequest→Action→Model→Event). Mass assignment guarded ($fillable explicit). Architecture solid ($afterCommit, typed DTO, Resource). Ship it.

---

**👤 You:**
> "I'll validate in the controller with $request->validate(), use $request->all() to create the user, check authorization with an if-statement, and send the welcome email inline after User::create()."

**🤖 AI Agent:**
> Verdict: FAT_CONTROLLER. Four violations in one method. (1) Validation belongs in a StoreUserRequest FormRequest, not inline. (2) $request->all() is a mass assignment vulnerability — use $request->validated(). (3) Authorization belongs in a Policy, not an if-statement. (4) Email is a side effect — dispatch UserCreated event, handle email in a Listener. Extract ALL of this from the controller.


## ❓ FAQ

**Q: Does Laravel Excellence Prover generate or write Laravel code?**
No. The agent writes the code. The tool VALIDATES that the code meets senior-level Laravel standards — query optimization, framework idioms, responsibility separation, mass assignment protection, and architectural compliance. It catches the five failure modes before the code is committed.

**Q: What does it catch that a system prompt instruction doesn't?**
Prompt instructions are suggestions — agents routinely ignore 'use eager loading' or 'validate with FormRequests.' Tool calls are obligations — the agent must fill every field. The engine has 22 consistency rules that catch specific anti-patterns: N+1, raw SQL without justification, env() in app code, unbounded get()/all(), synchronous heavy I/O, dd()/dump() in production, magic values, vague claims like 'follows best practices', and platitude conclusions. A prompt cannot enforce these — a tool schema can.

**Q: Why is N+1 checked before everything else?**
Because N+1 is the single most common and damaging performance anti-pattern in Laravel. A beautifully architected application with clean controllers and perfect FormRequests will still crash under load if every Blade view triggers 100 lazy-loaded queries. N+1 is checked first because no amount of clean architecture compensates for a database under siege.

**Q: Can I use this for existing legacy Laravel codebases?**
Yes. When refactoring legacy code, call the tool to validate each change against excellence standards. The tool catches the same patterns regardless of whether you're writing new code or improving old code. Start with the most critical pivot: enable Model::preventLazyLoading() to surface all N+1 issues, then progressively extract logic from fat controllers into Services, add FormRequests, and define $fillable.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/laravel-excellence-prover](https://vinkius.com/mcp/laravel-excellence-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Laravel Excellence Prover** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `laravel-excellence-prover` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Laravel Excellence Prover** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "laravel-excellence-prover": {
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
