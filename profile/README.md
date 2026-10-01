# Enthym

**AI learning research, starting with coding and the quality of verification feedback.**

We study how models and agents can learn reliably from experience. Increasingly
general models, world models, and AGI are research goals. The public work below
provides inspectable interfaces, selected specifications, audit tools, and
labelled evidence; it does not establish frontier-model capability.

Our GitHub work remains in the **verifiablelabs** organization and retains
Verifiable Labs repository and package identifiers.

[Research direction and public evidence](https://github.com/verifiablelabs/vlabs-docs/blob/main/docs/product-overview.md) ·
[Public repository map](https://github.com/verifiablelabs/vlabs-docs/blob/main/docs/repository-map.md) ·
[Contributing](https://github.com/verifiablelabs/.github/blob/main/CONTRIBUTING.md)

## Explore the public work

| Repository | Start here for |
|---|---|
| [vlabs-docs](https://github.com/verifiablelabs/vlabs-docs) | Research direction, scope, public navigation, and local setup |
| [vlabs-sdk](https://github.com/verifiablelabs/vlabs-sdk) | Typed contracts, dummy provider, and supplied-evidence promotion-gate CLI |
| [vlabs-formal](https://github.com/verifiablelabs/vlabs-formal) | Selected Lean specifications and a hand-maintained Python mirror |
| [vlabs-integrity](https://github.com/verifiablelabs/vlabs-integrity) | Known-deviation audit tooling with explicit reference and execution requirements |
| [vlabs-evidence](https://github.com/verifiablelabs/vlabs-evidence) | Historical public-benchmark reports and separately labelled synthetic evidence |
| [vlabs-examples](https://github.com/verifiablelabs/vlabs-examples) | Synthetic SDK examples; check compatibility with the current card schema |
| [vlabs-demo](https://github.com/verifiablelabs/vlabs-demo) | Offline terminal mechanism on constructed toy cases |

Historical verifier reports and synthetic examples are different evidence from
an independently reproduced model release. Read their provenance and limits
before citing a result. Internal research findings and protected evaluation
content remain in access-controlled records.

## Formal scope

Selected mathematical properties behind the contamination-resistant promotion
gate are machine-verified in Lean 4. A hand-maintained Python mirror has property
tests derived from selected definitions; no mechanized code-to-proof parity is
claimed. These results do not prove model generalization or the surrounding
service, and tool reports are not independent certifications.

[Try the public SDK locally](https://github.com/verifiablelabs/vlabs-docs/blob/main/docs/sdk-and-cli.md) ·
[Security reporting](https://github.com/verifiablelabs/.github/blob/main/SECURITY.md)
