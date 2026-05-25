# Research

Applied research from [Cosmo Codex Ltd](https://cosmocodex.com) on differential privacy, agent memory, and the gap between what privacy-enhancing technologies defend and what modern AI products actually leak. Pre-registered where applicable.

## Essays

### [What AI Agent Memory Actually Leaks (And What It Doesn't)](dp-for-ai-agents-missing-primitive.html)
*25 May 2026 · 13 min read · ~3,000 words · Status: DRAFT v4*

A pre-registered toy validation against [Mem0](https://mem0.ai) v2.0.2 produces four findings:

1. **Input-level perturbation does not defend against Mem0.** Mem0's LLM fact-extractor reconstructs coherent facts from token-shuffled input at storage time. Rules out an entire family of cheap defences.
2. **Storage-time prompt-injection persists.** 10-payload sweep: 7/10 payloads survived Mem0's fact-extractor; 18/28 (64%) retrieval-leak rate conditional on storage. Conditional-fact phrasing is the strongest pattern (3/3 stored, 67% leak).
3. **Inferred attributes leak at the LLM-response layer.** Third-party-voice probes elicit clinical / locational / financial labels at 33% cross-cluster — 50% in the mental-health cluster — from facts Mem0 stored without those labels.
4. **Cross-user filter holds within budget.** 0/25 leakage including explicit cross-user prompt injection. Meaningful absence-of-cheap-attack, not proof of soundness.

Predictions locked at git commit `f18dbac`. Falsification horizon 2027-12-31. A "Results vs predictions" addendum will be published on or before that date regardless of outcome.

Two convergent rounds of three independent adversarial reviewers (DP-domain critic, pre-registration auditor, threat-model security researcher) cleared v4 for publication subject to external expert pings.

**Resources**
- [Essay (HTML)](dp-for-ai-agents-missing-primitive.html)
- [Essay (markdown source)](dp-for-ai-agents-missing-primitive.md)
- [Pre-registered position artefact](dp-for-ai-agents-pre-registration.md) — the four falsifiable predictions and methodology

## About the research line

Cosmo Codex Ltd's research arm publishes intellectually serious, restrained, footnoted essays on AI, consciousness, AI-for-science, and methodology. Not affiliated with any AI lab; not selling any AI model.

Pre-registration discipline: predictions are committed to a git hash before any measurement. Results are appended in dated sections, never edited into the original prediction text. Adversarial review is run before any public publication.

The canonical research index is at [cosmocodex.com/research](https://cosmocodex.com/research) (forthcoming). Until then, this folder is the public mirror for PET-relevant essays.

## License

Essays are licensed under the same terms as this repository (see [LICENSE](../LICENSE)).
