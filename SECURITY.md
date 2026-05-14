# Security Policy

Proof of Insight is a verification protocol whose value depends on the integrity of the cryptographic and procedural mechanisms it specifies. Reports of security-relevant defects are welcomed.

## Reporting a vulnerability

Send reports privately to <editors@proofofinsight.org>. Please do not file public issues for unpatched vulnerabilities.

A useful report includes:

- The version of the specification or schema affected (e.g., `v0.6.2`, `schema/v0.6.2/step.json`)
- The section, predicate, or field involved (cite by `§` number where applicable)
- A clear description of the failure mode and, where applicable, a proof construction that exhibits it
- Your assessment of severity and which conformance level(s) are affected

You may use any common cryptographic protocol (PGP, age, Signal) to encrypt sensitive material; request a key by email if needed.

## Scope

In scope:

- Defects in the normative protocol text (§§1–5) that would allow a producer to construct a proof passing verification while violating one or more stated guarantees of §4 (traceability, reproducibility, reviewability, robustness, regulatability).
- Defects in the JSON schema(s) under `schema/` that diverge from the prose definition in a way that would admit ill-formed proofs as schema-valid, or reject well-formed proofs as schema-invalid.
- Ambiguities in normative text that two reasonable implementers could resolve in mutually incompatible ways with security consequence.
- Errors in the regulatory mappings of Appendix C that would lead an implementer to overclaim regulatory adequacy.

Out of scope:

- Defects in the source data ingested by an `observe` step. PoI explicitly delegates source-data integrity to upstream standards (§§1.3, 2.2.1).
- Defects in any specific implementation, deployment, signing key infrastructure, timestamp authority, or hosting environment. Implementations are not part of this specification.
- Defects in third-party documents referenced informatively (e.g., RFCs, the Contributor Covenant text).
- Issues with the Arclio LLC corporate infrastructure or with the canonical-URL hosting. Report those to Arclio LLC directly through normal channels.

## Disclosure

The interim editor will acknowledge receipt within five business days and aim to communicate a remediation plan (specification revision, schema fix, errata note, or — where appropriate — public clarification without spec change) within 30 days.

A coordinated public disclosure will follow remediation. Where the defect affects an unreleased working draft, the fix may land directly in the next draft cycle without separate disclosure; the changelog and Appendix D will identify the change.

Where the defect affects a published version of the specification, the editor will publish an erratum at the canonical URL and reference it from the next minor or patch revision.

## Acknowledgement

Reporters who wish to be credited will be acknowledged in the changelog entry that records the fix, unless they request anonymity.
