# Apply prequalification

## Header

- **ID:** `APP-PREQUAL-001`
- **Status:** Pilot prototype
- **Version:** `0.1.0`
- **Brands or partners:** AAA, Academy Sports, Burlington, Dell, Ford, HP, Loft, Ross
- **Channels:** Desktop web, mobile web, embedded experience
- **Product owner:** TBD
- **Design owner:** TBD
- **Last updated:** 2026-10-13
- **Last reviewed:** 2026-09-16
- **Review status:** Review needed

### Quick actions

- Demo: [Open live coded prototype](https://jfhgries.github.io/demosite/)
- Prototype: [Open live coded prototype](https://jfhgries.github.io/demosite/)
- Complete user flow: [Journey snapshot](#journey-snapshot)
- Research: Not available
- Disclosures: Approved for external demo; IDs not linked
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

The prototype includes the standard prequalification journey and an enhanced Bread Pay path. The Bread Pay path is available when the scenario is set to EDS, Prequalification with Bread Pay, and Approved.
The scenario selector includes logos for AAA, Academy Sports, Burlington, Dell, Ford, HP, Loft, and Ross; each logo has descriptive alternative text.
The EDS Bread Pay flow uses the URBrand logo in its header; desktop headers have 24px horizontal insets. Form fields throughout the demo use the Figma default prompt and float/highlight on focus or when populated.

| Screen | Journey step | Viewport | Description | Disclosures |
| --- | --- | --- | --- | --- |
| Product entry | Awareness | Desktop and mobile | Sets expectations and starts prequalification. | Placeholder, review needed |
| Personal details | Prequalification | Desktop and mobile | Collects the minimum simulated inputs. | Placeholder, review needed |
| Verification | Verification | Desktop and mobile | Demonstrates one-time passcode entry and recovery. | Placeholder, review needed |
| Result | Decision | Desktop and mobile | Shows an offer, pending state, or decline path. | Placeholder, review needed |
| Bread Pay product entry | Awareness | Desktop and mobile | Introduces the credit card, installment, and SplitPay options; each option expands to show details. | Placeholder, review needed |
| Bread Pay email | Prequalification | Desktop and mobile | Collects an email address before mobile verification. | Placeholder, review needed |
| Bread Pay mobile verification | Verification | Desktop and mobile | Collects a mobile number and presents the consent and contact disclosures. | Placeholder, review needed |
| Bread Pay billing address | Prequalification | Desktop and mobile | Collects the applicant’s physical billing address and marketing opt-out preference. | Placeholder, review needed |
| Bread Pay eligibility | Prequalification | Desktop and mobile | Collects date of birth and full SSN before a simulated eligibility check. | Placeholder, review needed |
| Bread Pay eligible offer | Decision | Desktop and mobile | Presents a simulated credit-card offer and installment and SplitPay options. | Placeholder, review needed |

## Interactive demo

- **Demo type and link:** [Coded local prototype](./demo/index.html)
- **Sections:** Use the Admin tab to choose brand, capability type, capability, device, and viewport settings. Brand search opens a scrollable list of all brands and filters predictively as you type. The live preview sits between the viewport controls and capability tags, and its active-settings summary updates immediately; the Demo tab displays that same experience at the selected viewport width.
- **Preview actions:** In Demo, copy a direct link (including the selected scenario and viewport settings) or copy the active demo image; confirmation toasts indicate successful copies.
- **Presentation:** The demo flow omits the introductory title/status header, and the personal-details start screen has no soft-inquiry checkbox.
- **Live or simulated:** Simulated
- **Credentials required:** No
- **External demonstration approved:** Yes
- **Supported scenarios:** Offer available, more verification needed, no offer
- **Enhanced Bread Pay scenario:** Choose EDS → Prequalification with Bread Pay → Approved to open the responsive product-selection and offer flow.
- **Known limitations:** No real services, no disclosure IDs or version metadata, no production analytics, and no completed accessibility review.
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

No disclosure IDs are linked in this repository. The disclosure copy is approved for external demonstration; keep the simulated result clearly distinguished from a final credit decision.

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
