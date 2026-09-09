# Virtual Classroom Watch intent

## What this product is

Virtual Classroom Watch is a structured, version-controlled reference for virtual meeting and classroom platforms, their vendors, and their feature capabilities. It publishes a generated static website and JSON API at https://VirtualClassroom.watch/.

## Why it exists

Platform features, availability, and vendor relationships change over time. This repository keeps those claims in inspectable Markdown and YAML source so readers and machine consumers can review the evidence, compare implementations, and propose corrections.

## Design invariants

1. `project.yml` and `data/examples/` own the project model and reference data.
2. `scripts/build.js` generates the public `docs/` website and JSON API from repository source.
3. The ontology remains feature-first: vendors produce platforms, and platform capabilities implement stable features.
4. Factual updates retain source evidence and a valid `last_verified` date.
5. Native cross-reference validation must pass before publication; it does not establish complete schema coverage or factual freshness.
6. The build and validation path uses Node.js built-ins and has no package installation step.
7. Commits, pushes, deployment, and external console actions remain separate from local source maintenance.

## Scope boundaries

This repository owns the platform, vendor, feature, and capability corpus; the project ontology; the static-site generator; the generated public site and JSON API; and repository-specific validation and discovery contracts.

It does not provide professional advice, guarantee that vendor features or prices remain current between reviews, operate the third-party platforms it describes, or authorize publication through a local documentation change.

## Conformance philosophy

N/A because Virtual Classroom Watch is a reference application, not an open specification. Its public data and generated surfaces remain testable through the repository's validators and current evidence.

## Admission criteria for changes

N/A as an open-spec requirement. Data changes follow the existing contributor path: update repository source, preserve evidence and verification dates, pass cross-reference validation, rebuild the generated artifact, and pass the local search contract.

## Relationships to other PAICE standards

Virtual Classroom Watch is a Snap Synapse reference rather than a PAICE standard. It publishes a GuideCheck assistant guide for bounded data maintenance and uses the portfolio accessibility and search-audit methods. These integrations do not expand the product's scope or establish conformance by themselves.

The optional [repository standards declaration](repo-standards.yaml) records applicability, source and delivery maps, and existing verification expectations. This intent remains authoritative for purpose, boundaries, and exceptions. Declaration validation does not establish conformance or authorize command execution.

## Exceptions to Repo Standards

No owner-approved exceptions are recorded. Unresolved applicability and adoption questions remain unresolved in `repo-standards.yaml` rather than being treated as exceptions.

## Changelog

- 2026-09-08: Consolidated existing repository purpose, source and generation boundaries, and validation expectations; linked the optional repository standards declaration without changing product or publication behavior.
