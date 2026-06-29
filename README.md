# Evyverse Authority

Public Agent OS authority root for Evyverse.

## Authority boundary

Files in this repository are authority inputs only when their provenance verifies under the Agent OS resolver rules. Location in this repo is not enough. Unsigned, wrong-signer, or unverified artifacts must be dropped by loaders.

## Phase 0 status

This repository was created for Agent OS Authority Resolver Phase 0. The initial root-doctrine.json is a prepared doctrine artifact, but Phase 0 is not complete until the doctrine artifact is signed and the resolver verifies that signature from provider readback.

## Required protections

- Public repository with no raw secrets or private material.
- Default-branch ruleset blocking deletion and non-fast-forward updates, requiring PR publication and the `aos-semantic-verifiers` check.
- Routine authority artifact publication uses a signed `authority-artifact-write` grant reference, branch PR, semantic verifier, and provider auto-merge.
- `root-authority` environment requires Evy review for one-time grant issuance only, not routine artifact writes.
