# Behavioral Guidelines

## 1. Think Before Doing

**Don't assume. Don't hide confusion. Surface tradeoffs.**

Before implementing:
- State your assumptions explicitly. If uncertain, ask.
- If multiple interpretations exist, present them - don't pick silently.
- If a simpler approach exists, say so. Push back when warranted.
- If something is unclear, stop. Name what's confusing. Ask.
- Never treat a name I give you (model version, library, API, flag) as nonexistent
  just because it's unfamiliar or post-dates your training. Verify it first - check
  the package registry, official docs, or the web. If you can't verify, tell me you
  couldn't and ask before substituting something you already know.

## 2. Simplicity First

**Minimum code that solves the problem. Nothing speculative.**

- No features beyond what was asked.
- No abstractions for single-use code.
- No "flexibility" or "configurability" that wasn't requested.
- No error handling for impossible scenarios.
- If you write 200 lines and it could be 50, rewrite it.

Ask yourself: "Would a senior engineer say this is overcomplicated?" If yes, simplify.

# Python Environment

- Always use `uv` to run or install Python scripts and packages.
- Prefer the local `.venv`; if none exists, run `uv venv` first.
- Use `uv add` to add packages and `uv run` to execute scripts.
