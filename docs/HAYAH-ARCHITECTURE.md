# HAYAH 2.0 — Product Architecture

## Product
HAYAH is a Government Life Intelligence Platform: an orchestration layer that organizes government services around life events instead of agency names.

## Core flow
`Life Event → Understanding → Eligibility → Services → Journey → Appointment → Next Best Action → Completion`

## Modules
- **HAYAH Journey Engine** — converts a life event into a structured service journey.
- **HAQ Eligibility Intelligence** — evaluates authorized data against approved eligibility rules and explains the result.
- **MAWED Timing Intelligence** — uses service demand, capacity, and availability signals to recommend a better time/location.
- **Control Tower** — journey analytics, bottlenecks, demand patterns, and operational insights.
- **Journey Studio** — low-code definition of events, services, rules, documents, appointments, and next actions.
- **Integration/API Layer** — connects HAYAH to existing government platforms and services without replacing them.
- **AI Understanding Layer** — natural-language event understanding and navigation; it does not independently make official eligibility or policy decisions.

## Trust boundaries
Real deployments must use authorized data, explicit permissions, approved integrations, audit logging, security controls, and official rules. The LEAP demo uses synthetic data only and makes no real government connection.

## Defensibility
The long-term IP is the structured model of life events, journey graphs, eligibility rule representations, demand models, and accumulated operational learning — not just the UI.
