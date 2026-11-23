# Security model

## Intent
BURHWARD explores **controlled incident-response automation** with a human approval boundary.

| Concern | Engineering approach |
|---|---|
| Untrusted SIEM content | Treat alerts, logs and model-readable text as untrusted evidence |
| AI hallucination / prompt injection | AI may explain or summarize, not authorize execution |
| Privileged operations | Separate preview, authorization and execution |
| Approval integrity | Bind decisions to exact requests; check time limits and roles |
| Auditability | Record decision and actual executor/verifier outcome |
| Data privacy | Redact logs, identifiers and evidence before public sharing |

## Threats considered
Prompt injection, replayed approval, stale permissions, confused-deputy access, misleading success claims, and leakage through screenshots or logs.

## Status
These are principles and review targets, **not a certification** that every control is operational today.
