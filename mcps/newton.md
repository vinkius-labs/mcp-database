# Newton MCP Server

Perform advanced symbolic mathematics—simplify expressions, calculate derivatives, find integrals, and solve equations directly through your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/newton)

## Overview
**Category:** developer-tools
**Tools Count:** 15

## Description
Connect the **Newton** symbolic math engine to your AI agent to solve complex mathematical problems using natural language. From basic algebra to advanced calculus, this server provides a comprehensive suite of tools for students, engineers, and researchers.

### What you can do

- **Calculus Operations** — Calculate derivatives (`math_derive`) and indefinite integrals (`math_integrate`) for complex functions.
- **Algebraic Solving** — Simplify expressions (`math_simplify`), factor polynomials (`math_factor`), and find the roots or zeroes of functions (`math_zeroes`).
- **Geometric Analysis** — Find the area under a curve (`math_area`) between two points or determine the tangent line (`math_tangent`) at a specific x-value.
- **Trigonometry & Functions** — Access a full range of trigonometric functions including sine, cosine, tangent, and their inverses (arcsin, arccos, arctan).
- **Advanced Math** — Compute absolute values (`math_abs`) and logarithms with custom bases (`math_log`).

### How it works

1. Subscribe to this server
2. Enter your Newton API endpoint or access key
3. Start solving math problems directly in Claude, Cursor, or any MCP client

### Who is this for?

- **Students & Educators** — Quickly verify complex homework solutions or generate step-by-step mathematical context.
- **Engineers** — Perform quick symbolic derivations and integrations without leaving your technical documentation or code editor.
- **Data Scientists** — Validate mathematical models and simplify complex expressions during the research phase.


## Available Tools
- **math_abs**: Calculate the absolute value of an expression
- **math_arccos**: Calculate the inverse cosine of an expression
- **math_arcsin**: Calculate the inverse sine of an expression
- **math_arctan**: Calculate the inverse tangent of an expression
- **math_area**: Find the area under a curve (definite integral)
- **math_cos**: Calculate the cosine of an expression
- **math_derive**: Example: x^2+2x -> 2 x + 2

Find the derivative of a math expression
- **math_factor**: Example: x^2+2x -> x (x + 2)

Factor a math expression
- **math_integrate**: Example: x^2+2x -> 1/3 x^3 + x^2 + C

Find the indefinite integral of a math expression
- **math_log**: Provide the base and the value.

Calculate the logarithm of a value with a specific base
- **math_simplify**: To compute fractions, use the keyword (over) to separate the numerator and denominator (e.g., 2(over)4).

Simplify a math expression
- **math_sin**: Calculate the sine of an expression
- **math_tan**: Calculate the tangent of an expression
- **math_tangent**: Provide the x-value and the function expression.

Find the tangent line of a function at a specific x-value
- **math_zeroes**: Example: x^2+2x -> [-2, 0]

Find the roots (zeroes) of a math expression


## Installation & Usage

To install and use the **Newton** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/newton](https://vinkius.com/mcp/newton)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
