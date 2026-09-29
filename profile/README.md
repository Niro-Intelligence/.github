<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Niro-Intelligence/.github/main/profile/niro-lockup-dark.svg">
  <img alt="Niro" src="https://raw.githubusercontent.com/Niro-Intelligence/.github/main/profile/niro-lockup-light.svg" height="40">
</picture>

[![Website](https://img.shields.io/badge/Website-niro.ai-3343C3)](https://niro.ai)
[![Documentation](https://img.shields.io/badge/Docs-help.niroai.dev-3343C3)](https://help.niroai.dev)
[![npm](https://img.shields.io/badge/npm-%40niroai%2Fniro-3343C3)](https://www.npmjs.com/package/@niroai/niro)
[![Discord](https://img.shields.io/badge/Discord-Join-3343C3)](https://discord.gg/gpZdgJd5k)
[![YouTube](https://img.shields.io/badge/YouTube-%40tryniroai-3343C3)](https://www.youtube.com/@tryniroai)

> **Your AI coding agent is guessing. Niro hands it the map.**

On every question, an AI coding assistant greps for names, reads a few files, and guesses the rest of the system. Niro parses your repos into a live map of the whole system, every class, method, call, HTTP hop, event and data store, across repos and languages. Your assistant queries that map over MCP, so call chains, blast radius, root-cause analysis and reuse checks become one tool call instead of a guess.

Niro is not a replacement for Claude Code, Cursor or Copilot. It is the deterministic logic layer underneath them.

## Quick start

One command, run inside the repo you are working on:

```bash
npx @niroai/niro start
```

It signs you in, builds the graph for that folder, and connects your assistant over MCP.

## Supported assistants

Fourteen, each with a one-line install. [Full list and commands](https://help.niroai.dev/mcp/clients/).

| | | |
| --- | --- | --- |
| Claude Code | Cursor | Windsurf |
| VS Code | GitHub Copilot CLI | Codex |
| Claude Desktop | Gemini CLI | Cline |
| Kiro | Goose | OpenCode |
| Factory (droid) | Antigravity | |

## What your assistant gets

Thirty-one read-only MCP tools, grouped by the question they answer. [Reference](https://help.niroai.dev/mcp/tools/).

| Question | Tools |
| --- | --- |
| What breaks if I change this? | `get_blast_radius`, `get_impact_analysis`, `get_reverse_call_chain` |
| How does control flow? | `get_call_chain`, `trace_execution_path`, `find_entry_points`, `get_state_at_entry` |
| Which definition is the real one? | `resolve_fqn`, `find_handler`, `get_class_structure`, `get_source_code`, `code_grep`, `explain_code` |
| What crosses the wire? | `get_service_topology`, `find_api_endpoints`, `find_outbound_http_calls`, `list_events`, `get_event_producers_and_handlers` |
| Who touches this data? | `list_data_resources`, `get_data_resource_usage` |
| Does this already exist? | `find_reusable_code`, `get_config_symbols` |
| Has this bug been seen before? | `find_known_issues`, `get_bug_with_resolution`, `list_niro_bugs` |
| Is the graph current? | `list_projects`, `get_index_status`, `compare_builds`, `should_create_temp_project`, `mark_task_complete` |

## What it catches

One hundred real questions an assistant gets wrong without the graph, in ten patterns. Each one comes with the actual tool output. [Browse them](https://help.niroai.dev/use-cases/).

[Symbol resolution](https://help.niroai.dev/use-cases/find-the-real-one/) · [Blast radius](https://help.niroai.dev/use-cases/what-breaks-if-i-change-it/) · [Call tracing](https://help.niroai.dev/use-cases/how-control-flows/) · [Cross-service](https://help.niroai.dev/use-cases/across-the-wire/) · [Dead code](https://help.niroai.dev/use-cases/proof-before-delete/) · [Onboarding](https://help.niroai.dev/use-cases/the-instant-map/) · [Refactoring](https://help.niroai.dev/use-cases/safe-to-refactor/) · [Root cause](https://help.niroai.dev/use-cases/symptom-to-source/) · [Code review](https://help.niroai.dev/use-cases/grounded-review/) · [Agent accuracy](https://help.niroai.dev/use-cases/ground-the-agent/)

## Beyond the MCP server

- **Code review** that sees the whole system: security issues, dead code, missing error handling, circular dependencies, each with its impact radius. [How the gate works](https://help.niroai.dev/code-review/).
- **Root-cause analysis**: report a bug and Niro walks the real code paths to the cause, with a justification and a suggested fix.
- **Visualisation**: an interactive graph of your whole system, explored and shared from the console.

## Watch

Three walkthroughs on the help site: what Niro is, onboarding, and the graph at scale. [Watch](https://help.niroai.dev/watch/) · [YouTube](https://www.youtube.com/@tryniroai)

## Where to go

| | |
| --- | --- |
| Website | [niro.ai](https://niro.ai) |
| Documentation | [help.niroai.dev](https://help.niroai.dev) |
| Console | [console.niroai.dev](https://console.niroai.dev) |
| CLI on npm | [@niroai/niro](https://www.npmjs.com/package/@niroai/niro) |
| Community | [Discord](https://discord.gg/gpZdgJd5k) |
