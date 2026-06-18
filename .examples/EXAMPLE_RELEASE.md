# Example Release: v1.2.0

## Release Metadata
- Release date: 2026-06-20
- Target branch: main
- Release owner: @release-manager

## Summary
User authentication improvements and several bug fixes.

## Included changes
- Add user login (feat)
- Fix session expiry edge case (fix)
- Improve logging for auth errors (chore)

## Changelog entries
- Users can now log in with username/password and maintain sessions.
- Fixed session expiry bug causing unexpected logouts.

## Upgrade / Migration Notes
- None expected for this release.

## Smoke Tests (pre-release)
- [x] Deploy to staging
- [x] Run smoke tests
- [x] Verify migrations applied
- [x] QA sign-off

## Rollout Plan
- Deploy to 10% of hosts, monitor errors for 30 minutes, then proceed to full rollout.

## Rollback Plan
- Revert the release tag and deploy previous stable image; run rollback smoke tests.

## Communication
- Notify #releases channel with release notes and link to changelog.
