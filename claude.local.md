# CLAUDE.local.md — Personal Overrides

> ⚠️ This file is GITIGNORED. Personal preferences only — do not commit.

---

## 👤 My Preferences

- Give **verbose explanations** when generating new code (explain what and why)
- Always suggest **alternative approaches** before implementing
- When fixing bugs, show the **root cause** first, then the fix
- Add **inline comments** for non-obvious logic
- I prefer **functional style** — pure functions, no side effects where possible

---

## 🛠️ Local Dev Setup

- Python: 3.11 (managed via `pyenv`)
- Virtual env: `.venv/` in project root (`python -m venv .venv`)
- Package manager: `pip` with `pyproject.toml` / or `uv` if available
- Local DB: PostgreSQL via Docker (`docker compose up -d db`)
- Env file: `.env` (never commit)
- Run server: `uvicorn app.main:app --reload`

---

## 🔑 Env Var Reference (never paste real values here)

```
DATABASE_URL=postgresql+asyncpg://user:pass@localhost:5432/dbname
SECRET_KEY=...
ANTHROPIC_API_KEY=...
ENVIRONMENT=development
```

---

## 📝 Personal Notes

- Always explain **Pydantic v2** changes if coming from v1 patterns
- Prefer `asyncpg` driver for PostgreSQL
- Use `uv` instead of pip when suggesting install commands if available
- I use Ruff + Black in VS Code — format suggestions accordingly