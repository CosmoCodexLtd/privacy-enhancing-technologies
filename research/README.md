# Research — temporarily withdrawn

**Withdrawn 2026-05-25 pending vendor notification and ethics fixes.**

A draft essay ("What AI Agent Memory Actually Leaks") was published to this folder earlier today. A subsequent paper-grade adversarial review identified three issues that require resolution before re-publication:

1. The empirical work demonstrates real attacks against a deployed product (Mem0). Coordinated vulnerability disclosure to the vendor was not completed before public release.
2. Some of the "fabricated" ground-truth facts (notably the postcode) inadvertently overlap with real-world identifiers.
3. The pre-registration's own commitment to external expert review before public publication was breached.

The essay will be re-published after:
- Mem0 has been privately notified through coordinated-disclosure channels (target: 30-90 day standard CVD window)
- The ground-truth facts have been substituted with verified-fictional values and the affected tests re-run
- The three pre-registered expert pings (Damien Desfontaines / Anthropic Clio team / OpenDP maintainer) have had a chance to land

The underlying pre-registered position artefact (predictions immutable from `autoresearch` repo commit `f18dbac`; falsification horizon 2027-12-31) and the experiment code remain on record in the upstream `autoresearch` repository. They are not deleted; only the public-facing essay is withdrawn while the fixes land.

If you are from Mem0 (or any party with a stake in the underlying findings) and want to be notified privately as part of the coordinated disclosure, please contact Cosmo Codex Ltd via the channels on the [cosmocodex.com](https://cosmocodex.com) contact page.
