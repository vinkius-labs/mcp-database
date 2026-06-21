# Code Integrity Prover MCP Server

AI agents default to type evasion (like any, void*, unsafe, or ignore), TODO stubs, timing/sleep hacks, and empty catch blocks. 96% of developers don't trust AI-generated code. This tool enforces zero-workaround integrity across all programming languages.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/code-integrity-prover)

## Overview
**Category:** productivity
**Tools Count:** 1

## Description
AI agents write code that compiles but carries hidden debt. They use type evasions (like `any`, `void*`, `unsafe`, or `type: ignore`) to silence compiler warnings, `TODO` to defer implementation, sleep/timing hacks to mask race conditions, and empty catch/except blocks to hide failures. The code works — until it doesn't. And by then, the workaround has spread.

### The Problem It Solves

AI-generated code fails on five integrity axes across all programming languages:

- **Type evasion** — `any`, `void*`, `unsafe.Pointer`, `type: ignore`. Every type hack or compiler warning suppression is a hole in the safety net. The compiler warned you. The AI silenced it.
- **Placeholder stubs** — TODO, FIXME, HACK, stub functions, mock implementations, `panic!`, `NotImplementedError`. A placeholder is a promise you'll never keep. The AI moved on. The stub stayed.
- **Workaround patterns** — timing hacks, `sleep()` to wait for resources, retry-without-diagnosis, `z-index: 9999`, `!important`. These mask the real problem. The symptom disappears. The root cause compounds.
- **Swallowed errors** — `catch (e) {}`, `except Exception: pass`, empty catch blocks, `return null` without logging. An empty catch block or silent ignore is not error handling — it's error hiding. When production breaks, you have no stack trace, no context, no recovery path.
- **Copy-paste debt** — Duplicated logic that diverges over time. Magic numbers without named constants. Hardcoded values that break in staging. The AI generated it twice because it forgot it already generated it once.

### How It Works

Code Integrity Prover uses 5 Decision Pivots — boolean checkpoints that force the agent to PROVE its code is clean before committing:

1. **typesSafe** — Zero type evasion hacks (`any`, `void*`, `unsafe`, `type: ignore`). Strict typing enforced at interfaces/boundaries.
2. **noPlaceholders** — Zero TODO. Zero FIXME. Zero HACK. Zero stub functions. Zero mock data in production paths.
3. **noWorkarounds** — Zero timing hacks. Zero sleep loops. Zero retry-without-diagnosis. Every timing/concurrency issue has a proper async/event-driven solution.
4. **errorsHandled** — Every catch/except block matches specific exceptions. Every error has a recovery strategy. Every failure preserves debugging context.
5. **noDuplication** — No copy-paste blocks. No magic numbers. No hardcoded config. Similar functions consolidated.

The engine validates consistency: if the agent claims `CODE_PROVEN` but describes using `any` or `unsafe` in the type strategy, the tool rejects. If the placeholder audit mentions TODO but claims zero placeholders, it catches the contradiction.

### Why It Works

- **Catches workarounds BEFORE they enter the codebase** — not after, when they've already spread.
- **16 consistency rules** detect contradictions between the agent's claims and its descriptions.
- **Language-agnostic anti-pattern dictionaries** scan for specific evasion signals: type hacks, placeholder keywords, workaround patterns, swallowed error signatures.
- **Grounded in Martin Fowler's Refactoring, Kent Beck's Simple Design, Sandi Metz's rules** — not opinions, but established engineering principles.


## Available Tools
- **validate_code_integrity**: Code that compiles is not code that is correct. Code that passes tests is not code that is maintainable. You must: (1) enforce TYPE SAFETY — zero escape hatches. No `any` (TypeScript), no `void*` (C/C++), no `unsafe` (Rust), no `type: ignore` (Python), no `as` to silence errors, no non-null assertions. If the type system complains, the TYPE is wrong — fix the type, not the complaint, (2) audit for PLACEHOLDERS — zero TODO, FIXME, HACK, stub, panic!, unimplemented!(), NotImplementedError, mock data, or "will be implemented later" comments in code that will ship. If it is not implemented, it is not done. If it is not done, do not commit it, (3) audit for WORKAROUNDS — zero sleep() loops, busy-wait polling, setTimeout-as-fix, retry-without-diagnosis, "just restart the service," magic delay values. These mask root causes. If you need a delay, you have a race condition. Fix the race condition, (4) validate ERROR HANDLING — every catch/except block must: (a) catch a SPECIFIC error type, not generic Exception/Error, (b) perform a RECOVERY action or propagate meaningfully, (c) preserve debugging context (stack trace, relevant state). Empty catch {} is error suppression. catch(e) { log(e) } without recovery is error decoration, not handling, (5) audit for DUPLICATION — no copy-pasted blocks (extract to function), no magic numbers (extract to named constant), no hardcoded config (extract to config/env), no similar functions that differ by one parameter (extract to parameterized function). If rejected, the code has a structural integrity flaw. Fix the root cause, not the symptom.

Structured reflection tool for code integrity validation across any language or framework. Forces the agent to prove code is free of type evasions, placeholder stubs, timing workarounds, swallowed errors, and duplicated logic before committing or proposing changes. Catches Type Evasion (any/void*/unsafe/type:ignore — silencing the type system instead of fixing the type), Placeholder Residue (TODO/FIXME/HACK/stub/panic! left in code that will ship — incomplete work disguised as done), Workaround Patterns (sleep loops, busy-wait polling, retry-without-diagnosis, timeout-as-fix — treating symptoms instead of root causes), Error Swallowing (empty catch blocks, catch-and-log-only, generic Exception without recovery — hiding failures instead of handling them), and Duplication Drift (copy-paste blocks, magic numbers, hardcoded config, similar functions that should be one). Call once per code change, PR review, or implementation proposal


## Installation & Usage

To install and use the **Code Integrity Prover** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/code-integrity-prover](https://vinkius.com/mcp/code-integrity-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
