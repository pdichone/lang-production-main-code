# Production AI Agents with LangChain & LangGraph: Course Code

> **Heads up: this repo is no longer maintained.**
> Use **[github.com/pdichone/production-course-main-code](https://github.com/pdichone/production-course-main-code)** instead.
> It has the same lectures plus the latest fixes, a full setup guide, and a `.env.example`.
>
> ```bash
> git clone https://github.com/pdichone/production-course-main-code.git
> ```

This copy only gets critical fixes, such as the Claude model update below.

## Model update (2026-11)

Claude Sonnet 4.5 retires on 2026-11-30. The Claude examples now use `claude-sonnet-5-5`
and no longer pass `temperature` (Sonnet 5.5 rejects non-default values). Look for comments
that start with `# NOTE (2026-11):`, and see `HOTFIX-NOTES.md` for every difference from the videos.

## Quick start

```bash
uv sync
uv run python main.py
```

Put `OPENAI_API_KEY` and `ANTHROPIC_API_KEY` in a `.env` file (optional: `LANGSMITH_API_KEY`,
`LANGSMITH_PROJECT`, `LANGSMITH_TRACING`).
