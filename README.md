# Evyverse Authority

Private Agent OS authority root for Evyverse.

## Authority boundary

Files in this repository are authority inputs only when their provenance verifies under the Agent OS resolver rules. Location in this repo is not enough. Unsigned, wrong-signer, or unverified artifacts must be dropped by loaders.

## Phase 0 status

This repository was created for Agent OS Authority Resolver Phase 0. The initial root-doctrine.json is a prepared doctrine artifact, but Phase 0 is not complete until Evy signs the doctrine artifact and the resolver verifies that signature from provider readback.

## Required protections

- Private repository.
- Default-branch ruleset requiring signed commits, no deletion, no non-fast-forward updates, PR review, CODEOWNER review, resolved review threads, and the required semantic verifier check.
- root-authority environment requiring Evy review for grant issuance.
