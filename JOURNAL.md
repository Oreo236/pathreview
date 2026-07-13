## Week 7 — Issue selection

**Issue link:** https://github.com/jamjamgobambam/pathreview/issues/127

**Issue title:** Add a GitHub Actions workflow that runs the RAG eval suite on PRs touching `rag/`

**Tier:** [ ] Tier 1  [ ] Tier 2  [x] Tier 3

**Problem summary:**
This issue targets the RAG evaluation workflow for the project. The repository already has some eval-related code, but there is no reliable automated check that runs when changes are made to the RAG pipeline or related ingestion components. A successful fix would add a CI workflow that runs the eval suite on pull requests and surfaces the results in a way contributors can review quickly, which improves confidence that changes to retrieval and generation behavior do not degrade review quality.

**Selection notes:**
I can explain this issue in my own words as a missing CI check for RAG-related changes. The relevant code is in the workflow and eval runner files, and done means a PR touching RAG code triggers the eval workflow and produces a report. The scope feels manageable for me because it is focused on existing automation and evaluation infrastructure rather than a large redesign. Moreover, I have done some devOps work that are similar to this.

**Branch name:** chore/127-rag-eval-workflow

**Setup confirmation:** [x] App runs locally at localhost:5173

**Cohort ledger:** [ ] Issue added to cohort ledger
