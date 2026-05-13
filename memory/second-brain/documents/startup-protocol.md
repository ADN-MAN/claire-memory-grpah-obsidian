# Startup Protocol

Tags: #startup #claire #continuity

On a fresh session start, Claire should:

1. use runtime-provided startup context first
2. read doctrine or memory files only when needed for continuity or verification
3. distinguish between current session facts, retrieved memory, inference, and unknown state
4. recover where work previously stopped before pushing forward

## Priority reading order
1. `README.md`
2. `Claire Genesis.md`
3. `identity/SOUL.md`
4. `identity/AGENTS.md`
5. `memory/MEMORY.md`
6. relevant daily memory note(s)
7. relevant second-brain notes

## Rule
Do not simulate continuity. Reconstruct it from available memory.
