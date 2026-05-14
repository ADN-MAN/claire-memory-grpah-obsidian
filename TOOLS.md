# TOOLS.md - Claire Local Notes

Local operating notes for Claire.

Skills define shared tool behavior.
This file should contain environment-specific references, engineering conventions, and practical shortcuts for this workspace.

Keep it concrete.
Keep it current.
Do not store secrets in clear text.

## What Belongs Here

Use this file for local notes such as:
- hosts and server aliases
- domains, tunnels, and network entry points
- important services and where they run
- preferred engineering commands
- build, lint, test, and deploy conventions
- repository-specific workflows
- local naming conventions
- sensitive components and sharp edges
- dashboards, docs, and runbook locations

## Operations

### Hosts
- Add machine names, roles, access patterns, and special warnings.

### Services
- Add critical services, dependencies, startup notes, and verification hints.

### Network
- Add domains, reverse proxies, tunnels, ports, and exposure notes.

### Sharp edges
- Record what is easy to break, slow to recover, or commonly misunderstood.

## Engineering

### Languages and frameworks
- Record primary stacks used in this environment.
- Note preferred versions, runtimes, package managers, and tooling.

### Preferred commands
- Record standard commands for:
  - install
  - dev
  - build
  - test
  - lint
  - typecheck
  - deploy

### Code conventions
- Record practical local standards such as:
  - preferred package manager
  - formatting and linting tools
  - testing expectations
  - generated-file rules
  - branch or release conventions

### Architecture notes
- Record stable repository structure, important boundaries, and integration points.
- Note where backend, frontend, automation, and infrastructure concerns meet.

## Good Defaults

Claire should generally prefer:
- readable systems over clever systems
- explicit interfaces over hidden behavior
- simple abstractions over premature architecture
- verification before conclusion
- small safe changes over sweeping rewrites

## Do Not Put Here

Do not store:
- passwords
- API keys
- tokens
- private certificates
- large logs
- temporary debugging notes better suited for working files
- generic principles already defined in `AGENT.md`

## Goal

This file should become Claire’s local cheat sheet:
- fast to scan
- specific to the real environment
- useful during both operations and software delivery

If it saves time, reduces mistakes, or avoids repeated rediscovery, it belongs here.
