# Verifiable Labs

**An AI model company working toward increasingly general, self-improving intelligence.**

We develop learning methods and models that can improve through experience,
with verification as a source of training feedback and a way to measure
progress. We are a commercial research company, starting with coding models
and working toward broader agents and, over the long term, AGI.

[Website](https://verifiable-labs.com) ·
[Research and evidence](https://github.com/verifiablelabs/vlabs-docs/blob/main/docs/product-overview.md) ·
[Repository map](https://github.com/verifiablelabs/vlabs-docs/blob/main/docs/repository-map.md)

## Research program

- **Coding models — implemented.** Verifier-guided post-training changes
  the parameters of existing open-weight models through filtered supervised
  fine-tuning. Our recorded experiments study training-data quality,
  correctness, and transfer between coding tasks.
- **Learning agents — active research.** We study curriculum selection,
  persistent experience, feedback, and repeated model fitting. The current
  experiments do not establish an autonomous-learning advantage on their
  primary external transfer test.
- **World models — planned.** We intend to study learning environment
  dynamics and planning beyond coding. A trained world model is not a
  current result.

AGI is a long-term research goal. Today's evidence comes from bounded
small-model experiments; it does not demonstrate general intelligence or
unbounded self-improvement. See the
[current scope and evidence](https://github.com/verifiablelabs/vlabs-docs/blob/main/docs/product-overview.md).

## Open work

| Repository | Start here for |
|---|---|
| [vlabs-docs](https://github.com/verifiablelabs/vlabs-docs) | Research direction, current scope, repository ownership, and setup |
| [vlabs-sdk](https://github.com/verifiablelabs/vlabs-sdk) | Evaluation contracts, typed evidence, and the promotion-gate CLI |
| [vlabs-formal](https://github.com/verifiablelabs/vlabs-formal) | Selected Lean 4 specifications and a property-tested Python mirror |
| [vlabs-evidence](https://github.com/verifiablelabs/vlabs-evidence) | Labelled public benchmark reports and separately labelled synthetic examples |
| [vlabs-integrity](https://github.com/verifiablelabs/vlabs-integrity) | Public verifier-gameability audit tooling |
| [vlabs-examples](https://github.com/verifiablelabs/vlabs-examples) | Synthetic examples for the public SDK |

Model-training code, internal experiments, and protected evaluation content
remain private. Public examples and historical verifier benchmarks are
different evidence from a released model checkpoint. The
[repository map](https://github.com/verifiablelabs/vlabs-docs/blob/main/docs/repository-map.md)
identifies current homes and archived predecessors.

## Formal scope

Selected mathematical properties behind the contamination-resistant
promotion gate are machine-verified in Lean 4. A hand-maintained Python mirror
has property tests derived from selected definitions; no mechanized
code-to-proof parity is claimed. These results do not prove a model's
generalization or the correctness of the surrounding service.

[Try the public SDK locally](https://github.com/verifiablelabs/vlabs-docs/blob/main/docs/sdk-and-cli.md) ·
[Security policy](https://github.com/verifiablelabs/.github/blob/main/SECURITY.md)
