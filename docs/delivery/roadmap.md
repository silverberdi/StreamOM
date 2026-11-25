# Roadmap and governance
| Module | Dependencies | Outcome |
|---|---|---|
| M00 Platform Foundation | none | repo/OpenSpec, .NET modular boundaries, Angular/React workspaces, DB/migrations, tenant contracts, Docker/env, test harness, structured logging, security/design tokens/API conventions |
| M01 Identity & Tenancy | M00 | login, sessions, organizations, scoped memberships |
| M02 Station Lifecycle & Entitlements | M01 | onboarding/readiness/activation/publication config, quotas |
| M03 External Stream & Metadata | M02 | direct external integration, health, normalized metadata |
| M04 Public Player & White-label PWA | M02 M03 | public anonymous radio and PWA |
| M05 Media Library | M02 | upload/process/assign/version/catalog |
| M06 Programming Engine | M05 | schedules/shows/clocks/rotations/daily log |
| M07 Managed Playout & Source Router | M03 M06 | managed emission, switching/fallback |
| M08 Live Studio & Professional Ingest | M07 | WebRTC/OBS, takeover/return |
| M09 Audience Analytics | M04 M07 M08 | basic analytics can start earlier, enriched after managed/live |
| M10 Platform Administration & Support | M02 | global operation, commercial and support; can start earlier |
| M11 Operational Readiness & Production | all | hardening, restores, capacity validation and deployment |
Security/audit/observability throughout, not only M11. First usable milestone external station; later managed, live, full SaaS. No independent forever-MVPs.
## Definition of Ready
Business intent, scope/non-scope, actor journeys, states/errors/edge cases, decision closure, dependencies/contracts, permission/security, wireframes/assets when UI, Gherkin acceptance, test strategy, DoD. If any behavior-changing decision missing, stop and request refinement. M00 next; no issues created yet.
## Definition of Done
Approved OpenSpec change, complete vertical slice (not placeholders), tests including real PostgreSQL where applicable, UI fidelity/accessibility/states, operational failure scenarios, documented contracts/migrations, security/audit, Verify evidence, sync/archive as applicable, PR. Do not label a module complete from unit tests alone. Exact tool version/install and CI configuration not executed by this documentation commit.
