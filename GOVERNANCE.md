# Governance

## Editorial body

Editorial control of the Proof of Insight specification rests with **Arclio LLC** as **interim editor**.

This is a transitional arrangement. Per §0.5 of the specification, the intent is to move editorial control to an independent editorial body once the protocol has sufficient adoption and contributor base to warrant such a body. The transition path is:

1. **Phase 0 (current).** Single-editor stewardship. Arclio LLC, acting through named editorial staff, makes all editorial decisions. Open review through this repository.
2. **Phase 1.** Editorial committee. A standing committee of 3–7 members drawn from implementers, reviewers, and regulatory stakeholders, with rotating chair.
3. **Phase 2.** Independent editorial body. Formal organizational structure (foundation, working group under an established standards body, or equivalent) holding editorial control independent of any single sponsor.

The license model — CC BY 4.0 for the specification, Apache 2.0 for normative artifacts, the §0.3 patent non-assertion covenant — is structured to make this transition possible without re-licensing or contributor re-agreement.

## Decision-making during Phase 0

- **Editorial changes** (typo fixes, clarifications without semantic effect): resolved by editor judgment, optionally after a short public comment period.
- **Substantive changes** (new requirements, modified semantics, breaking changes): require a public RFC issue with a minimum 14-day comment period, followed by an editor decision documented in the issue and the changelog.
- **Conformance level definitions and required predicates:** treated as substantive.
- **Profile definitions:** profiles are normative specifications in their own right; their governance follows the same model.

Editor decisions during Phase 0 are final, with the explicit understanding that contributor feedback consistently overridden by the editor indicates a governance failure, not a contributor failure.

## Versioning

The specification uses semantic-style versioning at the protocol level:

- **Major (X.0.0):** breaking changes to verification semantics or step taxonomy.
- **Minor (0.X.0):** backward-compatible additions. Existing conformant implementations remain conformant.
- **Patch (0.0.X):** editorial corrections only. Protocol semantics unchanged.

Document and protocol version are intentionally the same, as stated in the specification's status section.

## License

The specification text is licensed under [CC BY 4.0](LICENSE). Normative machine-readable artifacts (schemas, reference verifier, conformance test suite) are licensed under [Apache 2.0](LICENSE-CODE).

The patent non-assertion covenant is stated in §0.3 of the specification.

## Trademark

"Proof of Insight" and "PoI" are trademarks of Arclio LLC. Use of these marks to describe an implementation as conformant is governed by the PoI Conformance Mark Policy (forthcoming). Use of the marks to accurately reference this specification is permitted.

## Contact

Editorial: editors@proofofinsight.org
Public discussion: https://github.com/proof-of-insight/spec/issues
