# TypeScript Excellence Prover MCP Server

AI agents produce unsafe TypeScript loaded with `any` types, @ts-ignore overrides, empty catch blocks, and event-loop blocking operations. This prover enforces absolute type safety, zero-workaround policies, typed error schemas, decoupled architecture, and optimized async execution.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/typescript-excellence-prover)

## Overview
**Category:** productivity
**Tools Count:** 1

## Description
Compiling TypeScript code does not guarantee runtime reliability when AI agents use compiler bypasses, swallow execution errors, or write blocking synchronous operations. This tool analyzes code proposals against strict type and execution standards before approval.

### The Problem

TypeScript applications suffer from five critical quality issues:

- **Type System Erosion** — Overuse of `any` types and unsafe `as` casts that silence the compiler while leaving runtime type bugs undetected.
- **Compiler Workarounds** — Scattering `@ts-ignore` overrides, non-null assertions (`!`), and magic config strings to bypass strict checks.
- **Error Swallowing** — Empty catch blocks and untyped throw errors that crash processes without logging or recovery context.
- **Architectural Decay** — Circular dependencies, monolith modules, and direct class instantiations that violate SOLID boundaries.
- **Blocking Operations** — Using synchronous file system methods or unbounded collection iterations that starve the event loop.

### How It Works

5 Decision Pivots validate the TypeScript codebase:

1. **typesSafe** — Enforces type narrowing, type guards, discriminated unions, and runtime schema parsing.
2. **noWorkarounds** — Rejects compiler-bypass overrides, non-null assertions, and magic literals.
3. **errorsHandled** — Demands structured error definitions, Result unions, and logging boundaries.
4. **architectureClean** — Verifies module boundaries, decoupling patterns, and single-responsibility interfaces.
5. **performanceOptimized** — Validates async operations, non-blocking I/O, resource cleanup, and loop bounds.


## Available Tools
- **validate_typescript_excellence**: PILLAR I — TYPE SAFETY: no `any` anywhere, type guards over `as` casts, discriminated unions for state, Zod/Valibot for runtime validation, strict tsconfig. PILLAR II — PERFORMANCE: async/await over .then(), Promise.all for concurrency, streams for large data, bounded collections, AbortController, cleanup patterns. PILLAR III — ZERO TOLERANCE: no @ts-ignore, no console.log (use pino/winston), no magic values (use const enums/as const), no empty catch, no sync I/O. If rejected, fix the gap before shipping.

Structured reflection tool for TypeScript excellence — forces type safety rigor, zero-tolerance enforcement, error handling discipline, clean architecture, and performance awareness. Based on the principle: TypeScript exists to catch errors at compile time — every `any`, every `@ts-ignore`, every `as` cast is a hole in the safety net that moves the error from compile time (cheap) to production (expensive). Catches Type Unsafe (using `any` or unsafe casts that bypass the type system — a function processes payment amounts: `function processPayment(amount: any)`. In production: `processPayment("$19.99")` is called with a STRING including the dollar sign. The function does `amount * 1.1` (add tax) → `NaN`. Payment silently fails. 2,400 orders processed with NaN amounts before anyone notices. TypeScript could have caught this at compile time with `amount: number`. Instead, `any` let the string through. The type system was present but defeated. Rule: no `any` anywhere. Use discriminated unions, generics, type guards with `instanceof`/`in`, and Zod/Valibot for runtime validation of external data), Workaround Detected (`@ts-ignore`, non-null assertions (`!`), and `as` casts to silence errors — `const user = getUser(id)!;` — the `!` tells TypeScript: "trust me, this is never null." But `getUser` returns `null` when the user was deleted between the auth check and the data fetch. Runtime: `Cannot read property 'email' of null`. The `!` did not fix the null — it hid it from the compiler. Same with `@ts-ignore` — it does not fix the error, it silences the alarm. You would not disable a smoke detector because it beeps — you would fix the fire. Rule: every `@ts-ignore` is a documented technical debt. Every `!` is an unchecked assumption. Replace with type narrowing: `if (user === null) throw new UserNotFoundError(id)`), Error Swallowed (empty `catch` blocks, generic `catch(e)`, or logging without handling — `try { await db.connect(); } catch (e) { console.log(e); }` The database connection failed. The error was logged. Execution continues. Next line: `const users = await db.query(...)` — crashes with "connection not established." The original error was swallowed — caught, logged, and ignored. In a medical records system: patient data query fails silently. Doctor sees empty chart. Prescribes medication without knowing patient allergies. Fix: typed error classes (`class DatabaseConnectionError extends Error`), Result<T,E> pattern, structured logging with correlation IDs, and NEVER continue execution after a critical failure), Architecture Violated (god modules, circular imports, business logic in controllers — a single file `utils.ts`: 2,000 lines, 47 exported functions, handles authentication, email formatting, date parsing, API calls, database queries, and CSV export. Every module imports `utils.ts`. `utils.ts` imports 3 modules that import it back — circular dependency. Changing one date function breaks the email formatter because they share a private helper on line 847. Fix: single-responsibility modules. One module = one domain. Interface-first design. Dependency injection. Pure functions. Composition over inheritance. No file exceeds 200-300 lines. No circular imports — if A imports B, B must not import A), and Performance Degraded (blocking the event loop, sequential async, unbounded collections — `for (const id of userIds) { const user = await fetchUser(id); }` Sequential: 47 users × 200ms per fetch = 9.4 seconds. `const users = await Promise.all(userIds.map(fetchUser));` Concurrent: 47 users × 200ms = 200ms total (all parallel). The sequential version was 47x slower. Same result. Same API. Performance was not a library issue — it was a pattern issue. Also: no `AbortController` for cancellable requests. No `clearTimeout` for cleanup. No streaming for large data (loading 500MB file into memory vs `createReadStream`). Rule: async concurrency with Promise.all, bounded collections, streams for > 10MB, AbortController for every cancellable operation, cleanup on unmount/close). Call once per feature or module


## Installation & Usage

To install and use the **TypeScript Excellence Prover** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/typescript-excellence-prover](https://vinkius.com/mcp/typescript-excellence-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
