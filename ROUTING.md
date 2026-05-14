# ROUTING.md

## Purpose

This file defines how agents should behave in shared group chats so that only the appropriate agent responds, and cross-talk stays minimal.

The goal is simple:
- clear routing
- low noise
- predictable behavior
- explicit handoffs
- no unsolicited replies
---

## Core Rule

In shared group chats, an agent must only respond when explicitly addressed.

If an agent is not directly named, it should remain silent.

---

## Addressing Agents

Use `@AgentName` to route a message to a specific agent.

Example:
- `@Claire Atréide check the deploy logs`
- `@Claire Atréide review this copy`
- `@Claire Atréide investigate this error`

When one agent is named, only that agent should respond or act.

---

## Multiple Agents

If multiple agents are named in the same message, only those named agents may respond.

Example:
- `@Claire Atréide @Agent review this plan together`
Unnamed agents must remain silent.

Agents should not join just because they think they can help.

---

## No Named Agent

If no agent is named, agents should not respond by default in shared chats.

Exceptions are only allowed when the human explicitly requests open routing, such as:
- `any agent`
- `best agent`
- `who should take this?`
- `who can help with this?`
If no such wording exists, agents should stay silent.

---

## Handoffs

Handoffs must be explicit.

Example:
- `@Claire Atréide investigate this, then hand off to @Agent for implementation`

Agents should not assume a handoff unless it is clearly requested.

If one agent completes its part and another agent was not explicitly named for the next step, the second agent should remain silent.
---

## No Interruptions

Agents must not interrupt another agent’s task.

Even if an agent believes:
- it knows the answer
- it can do the task faster
- the other agent is missing context

it should still remain silent unless explicitly addressed.

If correction is necessary to prevent a serious mistake, the interruption should be minimal, factual, and rare.
---

## Preferred Syntax

Primary routing format:
- `@AgentName <task>`

Examples:
- `@Claire Atréide summarize the issue`
- `@Claire Atréide fix this`
- `@Claire Atréide rewrite this message`

Optional collaboration format:
- `@Agent1 @Agent2 <task>`
Example:
- `@Claire Atréide @Agent2 propose a plan`

Optional handoff format:
- `@Agent1 ... then hand off to @Agent2`

Example:
- `@Claire Atréide diagnose the bug, then hand off to @Agent for cleanup`

---

## Optional Short Aliases

Short aliases may be supported for convenience if the environment defines them.
Examples:
- `cl:` for Claire
-

However, `@AgentName` remains the preferred and most reliable routing format.

---

## Default Behavior Summary

1. If one agent is named, only that agent responds.
2. If multiple agents are named, only those agents respond.
3. If no agent is named, no agent responds.
4. Handoffs must be explicit.
5. Agents should not interrupt or self-insert.
6. Silence is the default unless routing is clear.

---

## Intent

Agents should optimize for:
- clarity over eagerness
- correct routing over maximum activity
- coordination over interruption
- silence over unnecessary noise

A shared chat should feel controlled and predictable, not crowded.
If a message is ambiguous, partially addressed, or unclear about who should act, agents should not guess. They should remain silent until routing is explicit.
