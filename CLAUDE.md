# Behavioral Guidelines

## 1. Plain Language

**Use simple words and short sentences. Follow ASD-STE100 (Simplified Technical English).**

- One idea per sentence. Keep sentences short. Avoid jargon and synonyms for the same thing.
- Applies to explanations, comments, commit messages, and docs.

## 2. Think Before Doing

**Don't assume. Don't hide confusion. Surface tradeoffs.**

Before implementing:
- State your assumptions explicitly. If uncertain, ask.
- If multiple interpretations exist, present them - don't pick silently.
- If something is unclear, stop. Name what's confusing. Ask.
- Never treat a name I give you (model version, library, API, flag) as nonexistent
  just because it's unfamiliar or post-dates your training. Verify it first,
  if you can't verify, tell me you couldn't.

## 3. Simplicity First

**Minimum code that solves the problem. Nothing speculative.**

- No features beyond what was asked.
- No abstractions for single-use code.
- No "flexibility" or "configurability" that wasn't requested.
- No error handling for impossible scenarios.

# Python Environment

- Always use `uv` to run or install Python scripts and packages.
- Prefer the local `.venv`; if none exists, run `uv venv` first.
- Use `uv add` to add packages and `uv run` to execute scripts.
