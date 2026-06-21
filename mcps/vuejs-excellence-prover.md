# Vue.js Excellence Prover MCP Server

AI agents produce legacy Vue 2 configurations, unstable reactivity loops, and untyped interfaces. This prover enforces Vue 3 Composition API excellence, strict reactivity limits, compile-time type-safety, and optimized browser execution. Zero tolerance for Options API and raw prop mutations.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/vuejs-excellence-prover)

## Overview
**Category:** productivity
**Tools Count:** 1

## Description
Vue 3 introduces powerful reactivity, but AI models continuously fall back to outdated options, mutate properties, or drop reactivity through destructuring. This tool validates files against modern standards to ensure production readiness.

### The Problem

Vue applications suffer from five critical architectural flaws:

- **Legacy Options API** — Using data(), methods, or computed blocks instead of script setup with typescript.
- **Reactivity Degradation** — Destructuring reactive props directly or using mutating hooks that cause component re-render loops.
- **Type Loopholes** — Missing defineProps and defineEmits typescript definitions, leading to runtime failures.
- **Architecture Spaghetti** — Writing business logic directly in templates or missing composable separation.
- **Performance Bottlenecks** — Skipping route lazy loading, dynamic components, stable list keys, or watcher debounces.

### How It Works

5 Decision Pivots govern the validation engine:

1. **compositionApiUsed** — Enforces script setup, typed properties, and composable extraction.
2. **reactivityCorrect** — Assures reactive and ref boundaries without destructuring reactivity loss.
3. **typesSafe** — Validates type-only properties, event definitions, and strict typescript generics.
4. **architectureClean** — Confirms prop-down/event-up patterns, provider injections, and isolated stores.
5. **performanceOptimized** — Checks lazy imports, stable render keys, and watcher throttling.


## Available Tools
- **validate_vue_excellence**: PILLAR I — COMPOSITION API: <script setup lang="ts"> on EVERY SFC. defineProps<T>() type-only (no runtime defineProps). defineEmits<T>() typed events. defineModel() for v-model (Vue 3.4+). defineExpose() only when parent needs access. Composables (use*) for ALL reusable logic — not mixins, not utils with state. PILLAR II — REACTIVITY: ref() for primitives and single values. reactive() ONLY for objects that will NOT be reassigned. NEVER destructure reactive() — use toRefs()/toRef(). NEVER mutate props — emit events. computed() for derived state. watch() ONLY for side effects (API calls, DOM). watchEffect() for auto-tracked dependencies. shallowRef for large objects. PILLAR III — ARCHITECTURE: composables for reusable logic, provide/inject for DI, Pinia typed stores (no event bus), SFC max 200 lines, props down + events up, named/scoped slots for content projection. Performance: lazy routes, defineAsyncComponent, v-memo, v-once, stable :key (never index), KeepAlive, debounced watchers. If rejected, fix the Vue violation.

Structured reflection tool for Vue.js excellence — forces Composition API rigor, reactivity correctness, type safety, clean architecture, and performance awareness. Based on Vue 3.4+ with `<script setup lang="ts">` as the mandatory default. Catches Options API Detected (using `data()`, `methods`, `computed:` in Vue 3 — `export default { data() { return { count: 0 } }, methods: { increment() { this.count++ } } }`. This is Vue 2 syntax running on Vue 3. It works — but it loses: TypeScript inference (`this` is untyped), tree-shaking (entire Options API included), composable extraction (logic trapped inside component), and IDE autocomplete. `<script setup lang="ts">` with `const count = ref(0)` gives you: full TypeScript inference, tree-shaking, composable extraction, and IDE support. Rule: every SFC must use `<script setup lang="ts">`. If you see `data()`, `methods:`, or `computed:` — you are writing Vue 2 in a Vue 3 project), Reactivity Broken (destructuring reactive objects, mutating props, or misusing ref/reactive — `const { name, email } = reactive(user)`. The destructured `name` and `email` are now PLAIN STRINGS — reactivity is lost. Changing `user.name` will NOT update the template. The binding is severed. Fix: `const { name, email } = toRefs(user)` — maintains reactivity through refs. Also: `props.value = "new"` — NEVER mutate props. Props flow DOWN. Events flow UP. If you need to modify a prop: emit an event to the parent. `watch()` for side effects ONLY (API calls, DOM manipulation). `computed()` for derived state. If you use `watch()` to update a local variable based on another variable: that is a `computed()` — not a `watch()`), Type Unsafe (using `defineProps` without TypeScript generics — `defineProps({ userId: { type: String, required: true } })`. This is RUNTIME validation — Vue checks at runtime, not compile time. TypeScript cannot infer the type from runtime validators. Fix: `defineProps<{ userId: string }>()` — type-only, compile-time checked, full IDE autocomplete, no runtime overhead. Same for `defineEmits<{ (e: "saved", user: User): void }>()` — typed events. And `ref<User | null>(null)` — explicit generic on refs. Rule: no `any`. No `as any`. No runtime prop validators. Type-only generics on everything), Architecture Violated (500-line SFCs with business logic in the template — a `UserDashboard.vue`: 500 lines. The `<script setup>` section contains: API fetch logic, date formatting, form validation, error handling, pagination, and analytics tracking — all in one file. The template contains: `{{ new Date(user.createdAt).toLocaleDateString("en-US") }}` — formatting logic in the template instead of a computed property. `v-if="user.role === 'admin' && user.permissions.includes('edit') && !user.suspended"` — business logic in the template instead of a composable or computed. Fix: extract composables: `useUserProfile(userId)`, `useUserPermissions(user)`. Max SFC: 200 lines. Template: rendering only — no logic, no formatting, no calculations. Composables for reusable logic. Pinia for global state. provide/inject for DI), and Performance Degraded (using `:key="index"`, ignoring lazy routes, missing shallowRef — `<li v-for="(item, index) in items" :key="index">{{ item.name }}</li>`. User reorders the list. Vue reuses DOM nodes by index. Item 3 moves to position 1 — but the DOM node at position 1 still has item 1's internal state (input values, focus, animation state). Ghost state. Visual corruption. Fix: `:key="item.id"` — stable, unique identifier. Never use index as key. Also: every route should be lazy-loaded: `() => import("./views/Dashboard.vue")`. `defineAsyncComponent` for heavy components. `shallowRef` for large objects where deep reactivity is unnecessary. `v-memo` for expensive list renders. `KeepAlive` for frequently switched views. Debounced watchers for search inputs). Call once per component or feature


## Installation & Usage

To install and use the **Vue.js Excellence Prover** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vuejs-excellence-prover](https://vinkius.com/mcp/vuejs-excellence-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
