# Journey inventory and acceptance baseline
Every journey needs module-level Gherkin including entry/exit, permissions, errors, states, audit, tenant isolation and recovery before implementation.
| ID | Actor | Path and principal exception |
|---|---|---|
| J01 | Owner | register → tenant/station draft → identity/configuration → readiness; abandoned onboarding resumable |
| J02 | Owner | external URL → validate → activate → publish; unreachable blocks initial publication, retry |
| J03 | Admin | media → schedule → plan → node → start; invalid plan blocks start with reasons |
| J04 | Content manager | batch upload → process → classify/assign; corrupt file isolated, successful files retained |
| J05 | Programmer | draft schedule/clock → simulate daily log → resolve strict conflicts → publish version; current playback protected |
| J06 | DJ | invite/assign → prepare privately → authorized takeover → confirmed on air → end/return; disconnect policy/fallback |
| J07 | Admin/system | detect source failure → recover/fallback → verify; exhausted sources offline + notify |
| J08 | Listener | visit station → play → metadata/next → pause/reconnect; offline explicit |
| J09 | Analyst | select period → metrics with coverage → CSV; missing data identified |
| J10 | Platform admin | create/enable customer → quota/node checks → supervise/support; insufficient capacity reject without collateral damage |
| J11 | Admin | invite → accept → scoped roles → revoke; expired invite requires renewal |
| J12 | Owner | stop/archive → retain → restore draft or request deletion; dependency and retention checks |
| J13 | Admin | prepare target broadcast mode → validate → switch → confirm; failure preserve/recover old mode |
| J14 | Owner | brand/domain → private preview → publish; invalid custom domain keeps standard URL |
Cross-cutting tests: authorization, RLS, idempotency, concurrency, audit, async feedback, interruption recovery, no impact on unrelated stations.
