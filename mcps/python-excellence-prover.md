# Python Excellence Prover MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/python-excellence-prover)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

AI agents generate Python with no type hints, bare except blocks, mutable defaults, print() in production, and os.path everywhere. This tool forces excellence: Pydantic for boundaries, structured logging, pathlib, async I/O, and proper architecture. Zero tolerance for un-Pythonic code.

## Description
AI agents producing Python consistently write code that works but violates every principle an experienced Pythonista upholds.

### The Problem

- **No type hints** — Functions without param/return types. No Pydantic for validation. No mypy in CI.
- **Workarounds** — String concatenation instead of f-strings, os.path instead of pathlib, manual file handling instead of context managers, mutable default arguments.
- **Bare except** — Catches SystemExit and KeyboardInterrupt. except Exception: pass swallows everything silently.
- **Architecture decay** — God classes, circular imports, global mutable state, no dependency injection.
- **Performance traps** — Synchronous requests inside async, loading entire files into memory, no generators, no caching.

### How It Works

5 Decision Pivots force the agent to prove excellence:

1. **typesSafe** — Type hints everywhere, Pydantic for external data, dataclasses for DTOs, mypy --strict
2. **noWorkarounds** — f-strings, pathlib, context managers, no mutable defaults, no magic values
3. **errorsHandled** — Specific exceptions, custom hierarchy, structured logging, no bare except
4. **architectureClean** — Protocol-based DI, Repository+Service, no circular imports, abc.ABC
5. **performanceOptimized** — async I/O, generators, __slots__, lru_cache, bulk DB, N+1 prevention


## Available Tools (1)
- **validate_python_excellence**: PILLAR I — PYTHONIC: type hints on EVERY function (params + return + generics). Pydantic BaseModel for external data (API, forms, files). dataclasses for internal DTOs. Protocol for structural subtyping. f-strings, pathlib, context managers, match/case, EAFP over LBYL, comprehensions over loops where readable, enumerate() over range(len()). PILLAR II — PERFORMANCE: async/await for ALL I/O (httpx, asyncpg, aiofiles). Generators/itertools for large data (never materialize 1M rows into a list). __slots__ on data-heavy classes. functools.lru_cache for pure functions. Bulk DB operations (executemany, COPY). N+1 prevention (select_related, joinedload). PILLAR III — ZERO TOLERANCE: no bare except (catches SystemExit). No mutable defaults (def f(x=[])). No print() (use structlog/loguru). No os.path (use pathlib). No magic values (use Enum/StrEnum/Settings). No global mutable state. No # type: ignore without specific error code. If rejected, fix the gap before shipping.

Structured reflection tool for Python code excellence — forces type safety with Pydantic/mypy, Pythonic idiom enforcement, structured error handling, async-first I/O patterns, and zero-tolerance for anti-patterns before any Python code ships. Grounded in PEP 8, PEP 484 (type hints), PEP 557 (dataclasses), PEP 3156 (asyncio), and Python 3.12+ best practices. Catches Type Erosion (untyped functions that silently pass wrong data — def process_order(data, user, amount):     # What type is data? dict? OrderModel? str?     # What type is user? User object? user_id string? email?     # What type is amount? float? Decimal? int (cents)? str ("$49.99")?     result = calculate(amount * 1.08)  # Tax calculation on... what? If amount is passed as "$49.99" (string from form submission): amount * 1.08 raises TypeError at runtime — in production, on a Saturday. Fix: def process_order(data: OrderRequest, user: User, amount: Decimal) -> OrderResult: mypy catches the string×float multiplication at commit time, not production. External data (API, forms, files) MUST pass through Pydantic validation: class OrderRequest(BaseModel): amount: Decimal = Field(ge=0, description="Order total in USD") Internal data uses @dataclass for zero-overhead DTOs. Protocol for structural subtyping. Never Any. Never untyped), Anti-Pattern Blindness (using Python like Java instead of writing Pythonic code — Java-in-Python: for i in range(len(items)): item = items[i]; process(item) Pythonic: for item in items: process(item) Java-in-Python: result = ""; for s in parts: result = result + s Pythonic: result = "".join(parts) Java-in-Python: if x != None: ... Pythonic: if x is not None: ... Java-in-Python: try: d[key] except KeyError: d[key] = default Pythonic: d.setdefault(key, default) or defaultdict os.path.join("data", "file.csv") → pathlib.Path("data") / "file.csv" "Hello, " + name + "!" → f"Hello, {name}!" open(f); try: ... finally: f.close() → with open(f) as handle: ... Every non-Pythonic pattern is a readability tax on every future reader), Error Swallowing (catching exceptions without handling them — try: process_payment(order) except Exception: pass This catches EVERYTHING: ValueError (bad data), ConnectionError (Stripe is down), KeyboardInterrupt (operator pressing Ctrl+C), SystemExit (server shutting down). The payment silently fails. The order shows "completed." The customer is charged $0. Nobody knows until the finance team runs reconciliation 3 days later. Fix: specific exception classes, structured logging, re-raise or return typed error. try: result = stripe.Charge.create(amount=order.total_cents) except stripe.CardError as e: logger.warning("card_declined", order_id=order.id, reason=str(e)); raise PaymentDeclined(order.id, str(e)) except stripe.APIConnectionError: logger.error("stripe_unreachable", order_id=order.id); raise ServiceUnavailable("Payment processor") Custom exception hierarchy: AppError → PaymentError → PaymentDeclined | PaymentTimeout), Sync I/O in Async Context (blocking the event loop with synchronous operations — async def fetch_user_data(user_id: str):     response = requests.get(f"https://api.example.com/users/{user_id}")  # BLOCKS event loop     data = json.loads(open("config.json").read())  # BLOCKS event loop     db_result = cursor.execute("SELECT * FROM users WHERE id = %s", (user_id,))  # BLOCKS event loop Every synchronous I/O call in an async function blocks ALL concurrent coroutines. 100 concurrent requests become sequential — throughput drops from 100 req/s to 3 req/s. Fix: httpx.AsyncClient for HTTP. aiofiles for file I/O. asyncpg/databases for DB. async with httpx.AsyncClient() as client: response = await client.get(url) async with aiofiles.open("config.json") as f: data = json.loads(await f.read()) result = await conn.fetch("SELECT * FROM users WHERE id = $1", user_id)), and Mutable Default Trap (Python's most infamous gotcha — shared mutable defaults — def add_item(item: str, items: list = []):     items.append(item); return items add_item("a") → ["a"]. add_item("b") → ["a", "b"]. The default list is created ONCE at function definition, then SHARED across ALL calls. This is not a bug — it is Python's object model. But it is a trap. Fix: def add_item(item: str, items: list | None = None) -> list:     if items is None: items = []; items.append(item); return items Same applies to dict defaults, set defaults, and any mutable object. Rule: default arguments must be immutable (None, str, int, float, tuple, frozenset)). Call once per Python module, function, or feature implementation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Python Excellence Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I'll parse the API response with a dict, validate manually with if-statements, catch any errors with except Exception: pass, and log with print()."

**🤖 AI Agent:**
> Verdict: TYPE_UNSAFE. Use Pydantic BaseModel for API response validation — not manual if-checks on dicts. except Exception: pass silently swallows ALL errors including SystemExit. Use specific exceptions with structlog/loguru, not print().

---

**👤 You:**
> "OrderSchema (Pydantic) validates input. OrderService.create() uses asyncpg with DB transaction. Custom OrderError hierarchy. structlog with request context. async httpx for payment API. Generators for batch export. mypy --strict in CI."

**🤖 AI Agent:**
> Verdict: CODE_PROVEN. Types strict (Pydantic + mypy). No workarounds. Errors typed (OrderError hierarchy + structlog). Architecture clean (Service layer + DI). Performance optimized (asyncpg, httpx async, generators). Ship it.

---

**👤 You:**
> "I'll use os.path.join for file paths, def process(items=[]) with a mutable default, string concatenation for SQL queries, and requests.get inside an async function."

**🤖 AI Agent:**
> Verdict: WORKAROUND_DETECTED. Four violations: (1) os.path → use pathlib.Path. (2) def f(items=[]) shares list across calls → use None default. (3) String concat for SQL → use parameterized queries. (4) requests.get blocks async → use httpx.AsyncClient.


## ❓ FAQ

**Q: Does it generate Python code?**
No. The agent writes the code. The tool VALIDATES that it meets senior Python standards — type hints + Pydantic, structured error handling, clean architecture, and optimized async patterns. It catches five failure modes before code is committed.

**Q: Why is type safety checked first?**
Because untyped Python is a shell script. Without type hints, mypy can't catch bugs, IDEs can't autocomplete, and Pydantic can't validate data boundaries. Type safety is the foundation — error handling, architecture, and performance all depend on knowing what types flow through the code.

**Q: What Python-specific anti-patterns does it catch?**
23 consistency rules catching: bare except (catches SystemExit), mutable default args (def f(x=[])), os.path instead of pathlib, string concatenation instead of f-strings, print() instead of structured logging, open() without context manager, sync I/O in async context, global mutable state, blanket # type: ignore, and magic values.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/python-excellence-prover](https://vinkius.com/mcp/python-excellence-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Python Excellence Prover** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `python-excellence-prover` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Python Excellence Prover** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "python-excellence-prover": {
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
