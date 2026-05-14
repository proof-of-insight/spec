# Contributing

Proof of Insight is an open specification under active review. Contributions are welcome from anyone with relevant domain expertise: cryptographic provenance, regulated AI, standards development, clinical informatics, model risk management, workflow provenance, or related fields.

## Filing an issue

The issue tracker is the primary forum for substantive discussion. Issue templates cover:

- **Spec comment** — feedback on specific spec text, requests for clarification, scope concerns
- **Ambiguity** — places where the specification could be read more than one way
- **Conformance question** — questions about what is or is not required at each conformance level
- **Profile proposal** — suggestions for new domain profiles or extensions to existing ones

When filing an issue, please cite the spec section by number (§2.3, §5.1, etc.) where applicable.

## Proposing changes

For small editorial fixes (typos, broken links, minor formatting), open a pull request directly.

For substantive changes, open an issue first describing the proposal. After discussion, if there is rough consensus to proceed, open a pull request that references the issue.

Substantive changes that affect protocol semantics require an RFC-style issue with a minimum 14-day comment period. See [GOVERNANCE.md](GOVERNANCE.md).

## Pull request process

1. Fork the repository.
2. Create a branch with a descriptive name.
3. Make your changes. If you are changing normative content, update the changelog.
4. Sign off your commits using the Developer Certificate of Origin: `git commit -s`.
5. Open a pull request referencing any related issue.
6. Address review feedback.
7. Once approved, an editor will merge.

## Commit and changelog discipline

This is a normative protocol document under active review. The commit history is part of the editorial record: a regulator, implementer, or future editor must be able to identify when and why each substantive change to the specification was made. Apply the following discipline from the first commit, not from v1.0.

**One commit, one logical change, one (or zero) changelog bullets.** A logical change may span multiple files — a normative change to the spec text typically also updates Appendix D and `CHANGELOG.md`, all in one commit. Do not bundle two unrelated edits into one commit even when made in the same sitting.

In practice:

- If a commit needs more than one CHANGELOG bullet, split it into two commits.
- If a CHANGELOG bullet describes work that landed across two commits, re-stage the work as a single commit.
- Editorial cleanups with no normative effect (typo passes, link fixes, formatting) MAY be bundled by session into a single commit, with no CHANGELOG entry.
- Pure clarifications that do not change normative meaning still warrant a CHANGELOG bullet (under "Changed") and a corresponding Appendix D entry, even when they do not bump the version. The version-bump decision is separate from the changelog-entry decision.

**Commit message style.** Follow the prefix convention already in the repository history: `spec:` for normative or in-document changes, `docs:` for repository-level documentation (README, GOVERNANCE, CONTRIBUTING), `chore:` for tooling and process files, `refactor:` for restructuring without semantic effect. Use the imperative mood, lowercase after the prefix, and keep the subject line under ~70 characters. Use the body to explain *why* the change was made and to record the version-bump judgment when relevant.

## Developer Certificate of Origin

Contributions are made under the [DCO](https://developercertificate.org/). By signing off on your commits, you assert that you have the right to contribute the work under the project's license.

## Code of Conduct

This project follows the [Contributor Covenant Code of Conduct](CODE_OF_CONDUCT.md). By participating, you agree to abide by its terms.

## Communication

- Issues and discussion: <https://github.com/proof-of-insight/spec/issues>
- Editorial contact: <editors@proofofinsight.org>

For sensitive matters (security disclosures, policy concerns, conduct issues), contact the editor directly rather than via the public tracker.
