# Upstream provenance

- Source: https://github.com/GoogleCloudPlatform/microservices-demo
- Release: v0.10.7 (commit 5b608cb1dfe317d05e4f1bb8c99b7618452fde87)
- License: Apache-2.0 (see LICENSE). Copyright belongs to the original authors.
- Imported: 2026-11-25 as a single baseline commit (not a GitHub fork).

## Removed at import (KAVERI does not use them)
- .github/ (Google's CI workflows) - KAVERI CI is added in this repo separately.
- terraform/ - infrastructure is managed only in kaveri-platform.
- cloudbuild.yaml, .deploystack/ - Google Cloud Build / DeployStack tooling.

## DEV scope
- Deployed: 10 core services + Redis (standard set). Not deployed: shoppingassistantservice (needs Vertex AI/AlloyDB),
  loadgenerator (test tool, Phase 4).

## Upgrading
- New upstream release -> ticket -> branch -> import the new tag the same way -> review diff -> CI -> PR -> merge.
