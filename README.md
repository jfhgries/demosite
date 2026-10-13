# Credit Experience Demo Repository

This repository is the searchable source of truth for credit application experiences across brands, partners, and channels. It is designed to accelerate discovery, support cross-brand comparison, reduce duplicate analysis, and make demo readiness visible.

## Repository structure

- [`docs/taxonomy.md`](docs/taxonomy.md): Metadata model, page structure, governance rules, and status semantics.
- [`templates/experience.yml`](templates/experience.yml): Copyable record template for every experience.
- [`taxonomy/controlled-vocabularies.yml`](taxonomy/controlled-vocabularies.yml): Approved values for filters, tags, statuses, and comparisons.

## Adding an experience

1. Copy `templates/experience.yml` into `experiences/<experience-id>/experience.yml`.
2. Use values from `taxonomy/controlled-vocabularies.yml` for controlled fields.
3. Add the experience page, screens, and supporting links under the same experience directory.
4. Keep customer data, credentials, secrets, and unapproved disclosure text out of the repository.
5. Set `review_status` and `last_reviewed` honestly; do not infer current performance from missing metrics.

## Public demo

The Apply prequalification prototype is configured for publication at [jfhgries.github.io/demosite](https://jfhgries.github.io/demosite/). It will be available after the GitHub Actions workflow in `.github/workflows/deploy-demo.yml` runs on `main`.

## Design principles

- Metadata is structured for search and comparison; narrative pages explain the experience.
- Evidence, hypotheses, and recommendations are labeled separately.
- Production experiences, prototypes, recordings, and simulated demos are explicitly distinguished.
- Disclosures link to a centralized source instead of being duplicated in experience pages.
- Missing information is represented as `not_available`, `not_applicable`, or `unknown`, never as an implied positive.