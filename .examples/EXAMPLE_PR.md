# Example PR: Add user login (feat)

### Summary
Add basic username/password login flow with session tokens and client-side validation.

### Sprint & Estimate
- Sprint: Sprint 4
- Estimate: 3d (1 engineer)

### Related Issue
Closes: #42

### Changes
- Add `/auth/login` endpoint
- Store session tokens in secure, HTTP-only cookies
- Add frontend login form and basic validation
- Add unit tests for auth utilities

### Acceptance Criteria
- Users can log in with valid credentials and receive a session cookie
- Invalid credentials produce proper error messages
- Tests cover happy path and error cases

### Testing
- Run unit tests: `./scripts/test` or `pytest tests/test_auth.py`
- Manual QA: open login page, attempt valid and invalid logins, verify cookie set

### Reviewer
- Primary reviewer: @alice

### Labels
- Type: feat
- Priority: P1

### Checklist
- [x] Commit message follows Conventional Commits
- [x] Code follows project style and linters
- [x] Unit tests added/updated
- [x] Integration tests added/updated
- [x] All tests pass locally
- [x] CI checks are green
- [x] Documentation updated (if needed)

### Deployment / Rollout
- Deploy to staging, smoke test login flow, then schedule production deploy during low-traffic window.
