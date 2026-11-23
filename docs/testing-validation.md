# Testing and validation

> This portfolio reports a bounded, evidence-based engineering snapshot rather than a claim of deployment readiness.

## Known engineering stack
The private project includes React/Vite, Node.js, the `pg` PostgreSQL client, ESLint, Playwright and Node.js test scripts spanning unit, backend, database, QA, contracts, boundaries and end-to-end workflows.

## Isolated portfolio run — agent report (2026-11-23)
- Host: isolated LuxVPS QA machine, not the Hetzner production host
- Base commit: `e7a9669`
- Isolated branch: `portfolio/burhward-visual-polish`
- Reported worktree commit: `0d1c55b` (**not pushed**)
- Portfolio frontend: separate build served on loopback port 5192
- Original QA frontend: continued on port 5191
- Backend and isolated PostgreSQL: health/ready checks reportedly passed
- **345 of 345 unit tests reportedly passed**
- ESLint reportedly passed
- Default and portfolio builds reportedly passed
- Playwright E2E: **not run**
- Wazuh: stored alert shown via demo ingestion; no full Wazuh-to-executor integration claimed
- Approval and audit APIs: 403 for analyst role; fixture view only

These facts are transcribed from the execution agent's report; this public repository has **not independently reproduced the tests or reviewed raw test output**.

## Publication and provenance policy
- Separate **measured outcome** from unverified interpretation.
- Show real Wazuh evidence only after redaction.
- Clearly describe synthetic cases as synthetic.
- Never imply that a preview executed a firewall, endpoint, SQL or other action.
- Record test scope and untested areas.
