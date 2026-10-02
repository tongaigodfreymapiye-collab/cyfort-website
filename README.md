# CyFort Platform V3 — GitHub-ready prototype

Cyber Fortress Technologies (Pvt) Ltd — Building Stronger Digital Defences.

## Included
- Original CyFort branded multi-page website
- About page based on the public Cyber Fortress Strikingly site
- Penetration Testing + Vulnerability Assessment
- Zimbabwe-focused solution catalogue
- Free/Professional Risk Profile UX with AI interpretation concept
- Branded risk-report print/PDF workflow
- CyFort GRC product concept
- CyFort Lab hands-on training concept
- Paid CyFort Academy with instructor upload UI
- 50-question assessment demo and 50% pass threshold
- Certificate print/PDF workflow
- Careers CV upload UI
- Marketplace/service hooks from V2 concept

## Important: prototype vs production
This repository is intentionally a static GitHub-ready prototype. GitHub Pages can host the UI but must not be used as the security boundary for passwords, payments, private CVs, paid course entitlements, private software, OSINT API keys, AI provider keys, lab infrastructure or employee/admin operations.

### Production services required
1. Authentication: customer, learner, employee, instructor, HR, GRC admin roles; MFA for privileged roles.
2. Database: users, orders, shipments, courses, lessons, attempts, certificates, risks, controls, evidence, vendors, assessments and OSINT findings.
3. Object storage: private CVs, course files, evidence, paid software and generated reports using signed/expiring URLs.
4. Payments: hosted checkout + verified server-side webhooks. Never unlock paid content from browser-only payment state.
5. OSINT integration service: server-side API adapters with provenance, timestamps, confidence, caching, rate limits, legal/terms controls and source-level permissions.
6. AI risk agent: retrieval from collected evidence only; citations to evidence; prompt-injection defenses; no unsupported legitimacy/fraud conclusions.
7. PDF service: server-rendered reports/certificates with CyFort logo, unique report/certificate ID and verification URL/QR.
8. Training engine: question bank, randomization, attempt policy, server-side grading, progress tracking and certificate issuance.
9. Lab orchestrator: isolated per-user environments, time limits, reset/snapshot, network restrictions, abuse prevention, logging and trainer controls.
10. Notifications: email/SMS/push events for orders, shipments, training, certificates and risk-report completion.

## Suggested OSINT categories
Use documented APIs/feeds rather than arbitrary scraping. Categories include RDAP/domain registration, DNS, certificate transparency, TLS posture, public vulnerability/security advisories, authorised reputation/threat feeds, public company registries, regulator records and other lawful public sources. Each result should record source, query, retrieval time and confidence.

## Risk Profile tiers
**Free:** lightweight domain hygiene + public web trust indicators + summary.
**Professional:** deeper organisation verification, infrastructure exposure, breach/reputation signals where licensed, registry checks, vendor/third-party context, analyst/AI narrative and branded report.

## CyFort GRC
This is an original CyFort product concept, not ServiceNow code or UI. It uses common IRM/GRC capabilities: risk registers, qualitative/quantitative scoring, controls, policies, assessments, KRIs, issue/remediation workflow, third-party risk, audit, business continuity and executive dashboards.

## CyFort Lab
The concept is inspired by the category of hands-on cyber ranges (labs, scenarios, trainer oversight, CTF and progress tracking), but the implementation, branding and scenarios are CyFort-specific. Do not copy proprietary Cyberium/ThinkCyber code, content, scenarios, scoring algorithms, UI assets or trademarks.

## GitHub Pages
Upload this folder to a repository and enable Settings > Pages. Static pages will render. Production backend capabilities should be deployed separately and called over authenticated HTTPS APIs.

## Source note
Public About/Mission/Vision/service wording was adapted from Cyber Fortress Technologies' own Strikingly page at cyberfortresstechnologies.mystrikingly.com as requested by the owner. The public page retrieved during this build did not expose individual leadership credentials, so credentials were not invented in this package.

## V4 additions — cloud-ready, cross-platform and managed monitoring

The UI is standards-based responsive HTML/CSS/JavaScript and is designed for current Windows browsers (Edge/Chrome/Firefox) and iOS/iPadOS Safari. A web-app manifest, mobile navigation, safe-area support and responsive breakpoints are included. Native Windows/iOS apps can later consume the same cloud API.

### Cloud boundary
The static GitHub build contains no secrets. Production features should be attached behind `/api/*` endpoints so hosting can move to Azure, AWS, Cloudflare, Supabase/Firebase or another approved platform without rewriting the UI. Recommended services: authentication + MFA, PostgreSQL/managed database, object storage, background job queue, email/SMS/push provider, payment provider, audit logging, secrets manager and monitoring.

### Remote customer monitoring (CyFort Shield)
Only onboard systems under explicit written customer authorisation. Use per-tenant isolation and connectors for customer-approved EDR/XDR, Microsoft 365/Entra, SIEM, cloud, firewall/network and external attack-surface telemetry. Recommended flow: connector -> secure ingestion API -> normalization -> detection/risk engine -> incident/ticket -> customer dashboard -> notification. Never deploy hidden agents or collect data outside the contracted scope.

### Live cybersecurity news
`news.html` calls `GET /api/news`. The backend should aggregate approved RSS/API sources (for example CISA advisories and licensed cybersecurity news feeds), normalize `{title, source, date, url, summary}`, cache results, deduplicate headlines, preserve attribution and original URLs, and enforce publisher/API terms. Do not put paid API keys in browser JavaScript.

### Visitor analytics
The static prototype records only the current browser's visit count with localStorage. Accurate global visitors, unique visitors, logged-in users, sessions and repeat-visit history require server-side analytics/authentication. Suggested events: `session_started`, `page_view`, `login`, `logout`, `purchase`, `enquiry`, `course_started`, `course_completed`. Display aggregate statistics publicly only if desired; keep personally identifiable analytics private and comply with applicable privacy/cookie requirements.

### Feedback and testimonials
The prototype previews submitted feedback. Production flow: submit -> database -> spam/abuse checks -> CyFort moderation -> approve/reject -> publish. Never automatically publish unreviewed submissions. Store consent for use of customer names/company names with testimonials.

## V5 competitive homepage upgrade
- Cinematic, lightweight cybersecurity motion graphics on the homepage using Canvas/CSS (no copied competitor assets or proprietary animation code).
- Motion respects `prefers-reduced-motion` for accessibility and remains responsive on Windows browsers and iOS Safari.
- Expanded service lifecycle: Managed SOC/MDR, Identity/Zero Trust, email/phishing defence, backup/cyber recovery, vCISO, network/cloud defence, forensics/incident response, and cyber-physical security, in addition to VAPT, GRC, risk intelligence, Academy, Lab, monitoring and marketplace.
- Production recommendation: replace/augment the canvas with licensed original motion/video assets only if needed; optimize AVIF/WebM fallbacks and lazy-load below-the-fold media.

## V6 — Live Defence Desk
The homepage now includes a cinematic global threat-activity visual, ThreatWire headline panel, vulnerability-intelligence ticker and an organisation risk-search entry point. The world map is deliberately labelled demo telemetry until a cloud threat-intelligence backend is connected; it must not fabricate real attacks. `/api/news` is the integration boundary for live, source-attributed feeds. Recommended production inputs include CISA KEV/advisories and licensed/permitted cybersecurity RSS/API sources. Add server-side caching, deduplication, provenance, timestamps, rate limiting and source links. Never expose vendor/API secrets in browser JavaScript.

## Legal & Compliance Centre (V7)
`legal.html` provides the public legal/document centre. Formal PDF and editable DOCX templates are stored under `/legal-documents/`.

Before production launch, replace all bracketed placeholders with the final registered CyFort legal entity, company registration details, physical/service address, privacy/DPO contact, data-controller details where applicable, production domain, commercial response commitments and signed-service information. Obtain Zimbabwe-qualified legal review before relying on templates for live contracts.

Production workflows should require affirmative acceptance of the Terms/Privacy Notice with version + timestamp logging, and a signed SOW/Authorisation to Test or Monitor before security access is enabled. Careers should record applicant privacy consent separately.


## V8 - Compliance Framework Hub
CyFort GRC now presents assessment/mapping support for MITRE ATT&CK, NIST CSF 2.0, ISO/IEC 27001:2022, GDPR, Zimbabwe Cyber and Data Protection Act [Chapter 12:07], DORA and ITIL-based service management. These are carefully described as frameworks, standards or laws/regulations as appropriate; no accreditation/certification is implied.

## V9 - CyFort Local Vulnerability Snapshot
Adds a customer-facing "Scan This Computer" workflow with explicit device-authorisation and privacy consent, scan-agent launch architecture, vulnerability snapshot UI, severity/CVSS presentation and finding-driven service recommendations.

Important: the static website does not and cannot perform a Nessus/Qualys-style host scan from browser JavaScript. Production requires a separately installed, code-signed CyFort Scan Agent plus authenticated backend APIs. The agent should collect only authorised security posture, use least privilege, encrypt results, authenticate the tenant/device, log consent and scope, and support secure signed updates. Packet capture is a separate opt-in diagnostic function and is not part of the standard vulnerability snapshot.
