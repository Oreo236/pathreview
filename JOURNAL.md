## Week 7 — Issue selection

**Issue link:** https://github.com/ascherj/pathreview/issues/109

**Issue title:** Test coverage for `core/services/review_service.py` is below 40%

**Tier:** [] Tier 1  [x] Tier 2  [ ] Tier 3

**Problem summary:**
The review service is the core workflow for creating and processing portfolio reviews, but its important execution paths are not covered by unit tests. The missing coverage leaves the success path, partial failure path, and full failure path effectively unverified, which makes regressions harder to detect. A successful fix would add focused tests around the service logic in `core/services/review_service.py` so the behavior is exercised and documented.

**Branch name:** test/109-review-service-coverage

**Setup confirmation:** [x] App runs locally at localhost:5173

**Cohort ledger:** [x] Issue added to cohort ledger

## Week 8 — Reproduction & solution planning

**Reproduction commit link:** https://github.com/Oreo236/pathreview/commit/placeholder

**Reproduction summary:**
I reproduced the issue by running the review-service unit tests with coverage reporting. The current test run fails and does not provide meaningful coverage for the review workflow, confirming that the service’s main execution paths are not being exercised.

**PLAN.md link:** https://github.com/Oreo236/pathreview/blob/test/109-review-service-coverage/PLAN.md

**Walkthrough video (recommended):** Not recorded yet

**Blockers or open questions:**
None at the moment; the next step is to add focused tests around the success and failure branches in the review workflow.
