<div align="center">

![Cyranth banner](assets/banner.svg)

### AI-assisted development, agent-ready repositories, and production systems.

I build practical software for real repositories: coding-agent context workflows, deterministic developer tooling, secure automation, admin systems, and production-grade web platforms.

<p>
  <a href="https://github.com/Cynrath/agent-context-kit"><img alt="Featured project" src="https://img.shields.io/badge/featured-ACKit-0f172a?logo=npm&logoColor=white"></a>
  <img alt="ACKit vNext" src="https://img.shields.io/badge/ACKit-vNext%200.1.0--dev-111827?logo=typescript&logoColor=white">
  <img alt="Runtime" src="https://img.shields.io/badge/runtime-Node.js%20%3E%3D22-111827?logo=nodedotjs&logoColor=white">
</p>

</div>

---

## Featured Project

### [ACKit — AgentContextKit](https://github.com/Cynrath/agent-context-kit)

**Turn any repository into an agent-ready repository.**

ACKit is an offline-first, deterministic developer tool for preparing repositories for AI coding agents. The active vNext rebuild lives on [`rebuild/ackit-vnext`](https://github.com/Cynrath/agent-context-kit/tree/rebuild/ackit-vnext) and is being rebuilt around Node.js, TypeScript, an `ackit` CLI, and the official Model Context Protocol SDK.

Current vNext package identity: `@cynrath/agent-context-kit` `0.1.0`. It requires Node.js `>=22` and uses pnpm 11 for development. **The npm package is not published yet; publishing, tags, and releases remain separate explicit actions.**

**ACKit vNext focuses on:**

- Instruction graph analysis across Codex, Claude, Gemini, Copilot, nested scopes, overrides, and `applyTo` rules.
- Agent Skills parsing, validation, installation, and synchronization without executing embedded scripts.
- Secret and repository-hygiene scanning with redacted evidence and deterministic findings.
- Token-budgeted context packs with transparent ranking and exclusion reasons.
- Docs-first task workflows under `docs/tasks` with machine-checkable gates.
- Offline policy-as-code, locked rules, suppressions, baselines, and incremental scans.
- Terminal, JSON, SARIF 2.1.0, Markdown, HTML, and loopback report outputs.
- pnpm/npm/yarn/generic monorepo awareness with path-scoped semantics.
- Read-only MCP exposure for agent integrations.

```bash
# vNext is currently run from a checkout
pnpm install --frozen-lockfile
pnpm build
alias ackit="node $(pwd)/dist/cli/index.js"

ackit scan --ci
ackit instructions
ackit pack --max-tokens 50000
ackit task create "Describe the focused change"
ackit mcp serve
```

---

## Current Focus

| Area | Direction |
| --- | --- |
| Agent-ready repositories | Instruction graphs, context budgeting, agent skills, deterministic handoffs |
| Secure developer tooling | Secret/hygiene scanning, policy-as-code, redacted evidence, offline-first defaults |
| Agent workflows | Docs-first tasks, machine-readable contracts, MCP, CI-friendly outputs |
| Production web systems | ASP.NET Core MVC, admin panels, RBAC, audit logs, SEO, deployment |
| Operations | GitHub Actions, Docker, Linux, Cloudflare, MSSQL, deployment workflows |

---

## Tech Stack

` TypeScript ` ` Node.js ` ` pnpm ` ` MCP ` ` Vitest ` ` Biome ` ` Zod ` ` YAML ` ` GitHub Actions ` ` Docker ` ` Linux ` ` Cloudflare ` ` .NET ` ` ASP.NET Core ` ` C# ` ` MSSQL ` ` EF Core ` ` Git `

---

## Engineering Principles

| Principle | Meaning |
| --- | --- |
| Docs first | Changes start with context, scope, constraints, tests, and rollback notes. |
| Task first | Work is decomposed into focused, traceable tasks before implementation. |
| Deterministic by default | Tool output should be explainable, reproducible, and machine-checkable. |
| Offline first | Repository analysis should not require uploading source code to a remote AI service. |
| Security-aware | Secrets, permissions, leakage risk, filesystem boundaries, and safe defaults matter. |
| Production-ready | Changes are validated with build, tests, lint/type checks, CI, and explicit evidence. |
| Maintainable | Prefer readable contracts and predictable behavior over unnecessary complexity. |

---

## ACKit vNext Development

The current rebuild intentionally replaces the frozen .NET/NuGet implementation with a smaller Node.js/TypeScript architecture aimed at easier installation, broader ecosystem reach, and direct `npx`/npm-style distribution once publication is authorized.

Development validation on the vNext branch is defined around:

```bash
pnpm lint
pnpm format:check
pnpm typecheck
pnpm build
pnpm test
pnpm smoke:cli
pnpm run smoke:package
```

Repository: [github.com/Cynrath/agent-context-kit](https://github.com/Cynrath/agent-context-kit)

vNext branch: [rebuild/ackit-vnext](https://github.com/Cynrath/agent-context-kit/tree/rebuild/ackit-vnext)

---

## Contact

Open an issue or discussion on any public repository.
