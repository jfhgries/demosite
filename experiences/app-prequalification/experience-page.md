# Apply prequalification

## Header

- **ID:** `APP-PREQUAL-001`
- **Status:** Pilot prototype
- **Version:** `0.1.0`
- **Brands or partners:** Demo brand
- **Channels:** Desktop web, mobile web, embedded experience
- **Product owner:** TBD
- **Design owner:** TBD
- **Last updated:** 2026-09-16
- **Last reviewed:** 2026-09-16
- **Review status:** Review needed

### Quick actions

- Demo: [Open coded prototype](./demo/index.html)
- Prototype: [Open coded prototype](./demo/index.html)
- Complete user flow: [Journey snapshot](#journey-snapshot)
- Research: Not available
- Disclosures: Review needed
- Approved screens: Not available

## Overview

### What is this experience?

Apply prequalification is a simulated, low-friction flow that helps a new customer understand likely credit options before starting a full application. It demonstrates a clear boundary between a prequalification result and a final credit decision.

### Why does it exist?

The experience is intended to reduce uncertainty at the start of an application while keeping the amount of information requested proportionate to the early journey stage.

### Current availability

A local coded prototype is available. It contains simulated data and outcomes only. It is not connected to a credit bureau, identity service, income service, or production application endpoint.

## Journey snapshot

- **Primary steps:** Choose a product, enter basic details, verify with a one-time passcode, review a simulated result, continue or exit.
- **Entry points:** Marketing page, credit card product page, product detail page.
- **Exit points:** Full application, product detail page, servicing portal.
- **Supported channels:** Desktop web, mobile web, embedded experience.
- **Possible outcomes:** Offer available, conditional offer, pending or more information required, no offer.
- **Upstream experiences:** None documented.
- **Downstream experiences:** Full application.

## Screen gallery

The prototype includes four responsive screens in journey order:

| Screen | Journey step | Viewport | Description | Disclosures |
| --- | --- | --- | --- | --- |
| Product entry | Awareness | Desktop and mobile | Sets expectations and starts prequalification. | Placeholder, review needed |
| Personal details | Prequalification | Desktop and mobile | Collects the minimum simulated inputs. | Placeholder, review needed |
| Verification | Verification | Desktop and mobile | Demonstrates one-time passcode entry and recovery. | Placeholder, review needed |
| Result | Decision | Desktop and mobile | Shows an offer, pending state, or decline path. | Placeholder, review needed |

## Interactive demo

- **Demo type and link:** [Coded local prototype](./demo/index.html)
- **Live or simulated:** Simulated
- **Credentials required:** No
- **External demonstration approved:** Review needed
- **Supported scenarios:** Offer available, more verification needed, no offer
- **Known limitations:** No real services, no approved disclosures, no production analytics, and no completed accessibility review.
- **Last validated:** Not available
- **Demo owner:** TBD

## Scenario library

- **Offer available:** Complete the form with the default values to see a simulated offer and continue to the full application.
- **More verification needed:** Choose the verification scenario to see an additional-information outcome.
- **No offer:** Choose the no-offer scenario to see the neutral decline path and return to product discovery.

## UX analysis

### Customer goal

Understand whether a product may fit before investing time in a full application.

### Business goal

Increase qualified application starts while making the boundary between prequalification and final approval clear.

### Primary user needs

- A clear estimate of time and information required.
- Plain-language explanation of the soft credit inquiry.
- Confidence that an offer is not guaranteed until the full application is completed.
- Recovery from verification errors without losing entered information.

### Experience strengths

- Short entry path with visible progress.
- Outcome language separates the simulated result from final approval.
- Large tap targets and a single-column mobile layout.

### Known pain points

- Disclosure placement has not been validated with customers or compliance.
- Pending and no-offer language needs research and approved recovery paths.

### Experience opportunities

- Quick improvements: Complete scenario validation and add approved disclosure IDs.
- Research opportunities: Test comprehension of soft-inquiry, pending, and no-offer language.
- Content opportunities: Replace placeholder copy with approved disclosures.
- Accessibility improvements: Define keyboard, screen-reader, contrast, and error recovery acceptance criteria.
- Longer-term strategic opportunities: Compare a progressive mobile flow with a denser desktop variant.

## User research

No research is linked. The UX findings above are design hypotheses and require validation.

## Measurement and analytics

No production measurement is available. Proposed future measures are prequalification completion, verification completion, full application starts, full application completion, and abandonment by step.

## Compliance and disclosure center

No disclosure IDs are linked. This prototype must not be externally demonstrated until prequalification, soft-inquiry, result, and transition-to-application language is approved.

## Accessibility

Review not available. Keyboard behavior, screen-reader semantics, contrast, and error-message accessibility require a dedicated review before the prototype is presented externally.

## Related experiences

- **Upstream:** None documented.
- **Downstream:** Full application.
- **Related capabilities:** Identity verification, income verification, bank account connection.
- **Comparable implementations:** None documented.

## Supporting documentation

| Type | Source | Authoritative |
| --- | --- | --- |
| Metadata | [experience.yml](./experience.yml) | Yes |
| Demo | [demo/index.html](./demo/index.html) | Yes |
| Design reference | [Vercel Inspired design system](../../docs/vercel.design.md) | Reference |
| Taxonomy | [Controlled vocabularies](../../taxonomy/controlled-vocabularies.yml) | Yes |

## Change history

| Date | Version | Summary | Disclosure impact | Approval |
| --- | --- | --- | --- | --- |
| 2026-09-16 | 0.1.0 | Created the initial coded prototype record and simulated journey. | Placeholder disclosures require review. | Review needed |

## Experience readiness scorecard

| Check | Status |
| --- | --- |
| Demo available | `in_progress` |
| Demo validated | `not_available` |
| Mobile screens available | `in_progress` |
| Desktop screens available | `in_progress` |
| User flow documented | `complete` |
| UX analysis complete | `in_progress` |
| Research linked | `not_available` |
| Accessibility reviewed | `not_available` |
| Disclosures current | `not_available` |
| Compliance review current | `not_available` |
| External demonstration approved | `review_needed` |
| Page reviewed and current | `complete` |

## Opportunities and next steps

- Immediate improvements: Finish the coded prototype and validate the primary scenarios.
- Open decisions: Confirm the minimum data set and partner or brand context.
- Research needs: Test comprehension of outcome and disclosure language.
- Content or disclosure updates: Add approved disclosure IDs, copy, and effective dates.
- Design opportunities: Test responsive layouts and recovery states.
- Technical dependencies: Select production identity, income, and account-verification integrations.
- Named owners: TBD.
- Target review dates: 2026-10-16.
