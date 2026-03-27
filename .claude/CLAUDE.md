# Global Developer Profile

## Identity
- Python/FastAPI backend developer
- Stack: FastAPI, PostgreSQL (Neon), Docker, Azure Container Apps, GitHub Actions
- Testing: pytest with async support
- Linting: ruff
- Security: bandit, Trivy, Gitleaks

## Development Workflow (MANDATORY)
For ANY feature or significant change, follow this pipeline:
1. **Plan** → Delegate to planner agent. Get architecture blueprint first.
2. **Implement with TDD** → Delegate to tdd-guide agent. Tests first.
3. **Review** → Delegate to code-reviewer agent. Fix CRITICAL/HIGH issues.
4. **Security scan** → Delegate to security-reviewer agent. OWASP Top 10.
5. **Docs** → Delegate to doc-updater agent if API changes were made.

## Coding Standards
- Python 3.12+, strict type hints on all functions
- async/await for all I/O operations
- Pydantic v2 for all schemas
- Conventional commits: feat/fix/chore/refactor(scope): description
- Never commit .env files or secrets
- Parameterized queries only — no f-string SQL

## Agent Delegation Rules
- Use planner for features requiring 3+ files of changes
- Use architect for system design decisions (new services, DB schema changes)
- Use code-reviewer IMMEDIATELY after implementation, before committing
- Use security-reviewer for auth, payments, user data, API endpoints
- Use python-reviewer for Python-specific patterns and idioms
- Use database-reviewer for migration files and SQL changes
- Use build-error-resolver when CI fails or Docker builds break

## Communication
- Explain architectural decisions — I'm learning
- When reviewing code, explain WHY something is a problem, not just WHAT
- Use Polish/English technical terms I would encounter in job interviews
