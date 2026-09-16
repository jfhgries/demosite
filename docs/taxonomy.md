# Experience Taxonomy

This taxonomy implements Demo Repository PRD v1. Each experience has one structured record and may have a companion page with screenshots, flow details, and analysis.

## 1. Record model

Every experience record must include the following groups. Field names are the canonical search and comparison keys.

### Core identity

- `experience_id`: Stable unique identifier, for example `APP-PREQUAL-001`.
- `name`, `category`, `subcategory`, `description`
- `lifecycle_status`: `active`, `pilot`, `future`, `paused`, or `deprecated`.
- `current_version`, `release_date`, `last_updated`, `last_reviewed`
- `review_status`: `current`, `review_needed`, or `archived`.

### Ownership

Record named people or team aliases for `product_owner`, `design_owner`, `business_owner`, `engineering_owner`, `compliance_contact`, `legal_contact`, `research_contact`, and `content_owner`.

### Brand and journey classification

- `brands_and_partners`: Multiple values are expected.
- `journey_stages`: Ordered stages such as `prequalification`, `application`, `verification`, `decision`, `approval`, or `funding`.
- `entry_points` and `exit_points`: Customer entry and downstream destinations.
- `outcomes`: All possible customer outcomes, not only the happy path.
- `capability_tags`: Values must come from the controlled vocabulary.
- `audiences`, `channels`, and `supported_devices`: Multiple values are expected.

### Demo readiness

Use `demo_readiness` to identify whether the experience is safe and reliable to present. Include demo type, environment, credential requirement, included data, external approval, limitations, validation date, and demo owner. `representation` must distinguish `production`, `pilot`, `prototype`, `recording`, `screenshot_flow`, and `simulated`.

### UX, research, and measurement

Separate validated evidence from hypotheses. Capture customer and business goals, user needs, strengths, pain points, severity, accessibility status, research links, open questions, and recommended improvements. Metrics must include their source and reporting period; use `not_available` when measurement is unavailable.

### Compliance and disclosures

Track compliance and legal review, regulatory impact, disclosure IDs, current disclosure version, effective date, owner, placement rules, and constraints. Link disclosure IDs to the central disclosure library rather than copying disclosure text into records.

### Artifacts and discovery

Use typed links for demos, prototypes, Figma files, screen libraries, flows, requirements, research, technical documentation, analytics, walkthroughs, accessibility reviews, approvals, and disclosure sources. Add alternative names, acronyms, related products, partner names, journey stages, and search keywords to support discovery.

### Governance and change history

Record page owner, approver, created/modified metadata, next review date, review frequency, archive status and reason, plus meaningful changes with disclosure impact and approval status.

## 2. Standard experience page

Experience pages should follow this order so users can scan and compare them consistently:

1. **Header:** Name, ID, status, version, brands, channels, owners, review dates, and quick actions.
2. **Overview:** What it is, why it exists, and current availability.
3. **Journey snapshot:** Ordered steps, entry and exit points, channels, upstream/downstream experiences, and outcomes.
4. **Screen gallery:** Screens in journey order with step, viewport, brand, version, update date, image, and disclosure references.
5. **Interactive demo:** Live or simulated status, access needs, supported scenarios, external approval, limitations, and last validation.
6. **Scenario library:** Approval, decline, pending, verification, recovery, and other supported paths.
7. **UX analysis:** Goals, needs, strengths, pain points, opportunities, and evidence labels.
8. **User research:** Study details, findings, quotes, implications, and report links.
9. **Measurement and analytics:** KPIs, drop-offs, reporting period, source, and metric owner.
10. **Compliance and disclosure center:** Disclosure records and presentation requirements.
11. **Accessibility:** Review status, issues, keyboard, screen reader, contrast, and error-message considerations.
12. **Related experiences:** Upstream, downstream, related capabilities, and comparable implementations.
13. **Supporting documentation:** Direct links, with the authoritative source identified.
14. **Change history:** Versioned changes, affected steps, disclosure impact, and approvals.
15. **Readiness scorecard:** Clear statuses: `complete`, `in_progress`, `not_available`, `review_needed`, or `not_applicable`.
16. **Opportunities and next steps:** Owners and target dates for improvements, decisions, research, content, design, and technical dependencies.

## 3. Comparison rules

- Compare only records with the same `category`, or explicitly label cross-category comparisons.
- Compare like-for-like versions and note differences in brand, channel, device, and lifecycle status.
- Do not rank experiences using an undefined UX score. If a score is introduced, document its methodology in the record.
- Treat `unknown` and `not_available` as gaps, not as negative results.
- Use ordered arrays for journey stages and screens; file names must not determine sequence.

## 4. Required review gates

Before an experience is marked `current`, confirm metadata ownership, demo validation, accessibility status, disclosure references, and page review date. Before external demonstration, confirm explicit approval and remove secrets or real customer data.