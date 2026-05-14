# Changelog

All notable changes to the Proof of Insight specification are documented here. The format follows [Keep a Changelog](https://keepachangelog.com/en/1.1.0/); the protocol follows semantic-style versioning at the protocol level (see [GOVERNANCE.md](GOVERNANCE.md)).

## [0.6.2] — 2026-XX-XX (working draft)

Document and protocol version are intentionally the same. v0.6.2 supersedes v0.6.1 with backward-compatible additions and clarifications. No producer compliant with v0.6.1 is rendered non-compliant by v0.6.2.

### Added

- **L4 split.** L4 (Attested) is split into L4A (Independently Attested) and L4R (Reproducible). L4A admits R2 reasoning throughout under independent attestation; L4R requires R3 for designated high-stakes outputs. v0.6.1 L4 claims map to v0.6.2 L4R.
- **Verification basis on the manifest.** New OPTIONAL `verification_basis` field on the manifest (§2.7), with values `replay-verifiable`, `linkage-verifiable-only`, or `resolution-limited`. Verifiers MUST report the achieved basis alongside the accept/reject decision.
- **Extended `conditioned-on` edge form.** OPTIONAL `context_role` and `declared_relevance_hash` fields pin the producer's assertion about contextual relevance without making the relation replay-verifiable.
- **PoI Core Test Profile (forward reference).** Appendix B now references a planned minimal executable profile (Ed25519 signatures, RFC 3161 or mock timestamps, inline-only invocations, deterministic toy compute functions, fixed claim-type vocabulary) intended to make §3 testable end-to-end without production infrastructure.
- **Threat model addition.** §6 adds threat 10 (verification-basis overclaiming).

### Changed

- **Patent covenant interim language.** §0.3 now states that, until a conformance test suite is published for a given version, the patent non-assertion covenant applies to good-faith implementations of the normative requirements of §§1–5 at that version.

### Deferred to v0.7

- Structured digest object (`{alg, value}`) for hash agility.
- Structured signature object (`{alg, key_id, value}`) carrying explicit scheme metadata.
- Manifest-level attestations as a separately-signed sibling object type.
- Companion publication of the PoI Core Test Profile and the first version of the conformance test suite.

## [0.6.1] — earlier

Internal pre-publication draft. Not separately preserved in this repository.
