# Verifiable Labs

> Verifiable Labs builds clean feedback and promotion gates for increasingly general AI agents.

AI agents are getting better at passing the tests they were tuned on.
Verifiable Labs helps agents improve through **generated clean feedback
loops**, then verifies whether those improvements **truly generalize**
before promotion — on hidden, out-of-distribution, and adversarial
scenarios the agent has never seen.

[![Website](https://img.shields.io/badge/website-verifiable--labs.com-blueviolet)](https://verifiable-labs.com)
[![PyPI](https://img.shields.io/pypi/v/vlabs-sdk?label=pypi%3Avlabs-sdk&color=4c1)](https://pypi.org/project/vlabs-sdk/)
[![Zenodo DOI](https://img.shields.io/badge/Zenodo%20DOI-10.5281%2Fzenodo.19786415-blue)](https://doi.org/10.5281/zenodo.19786415)
[![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/verifiablelabs/verifiable-labs-envs/blob/main/LICENSE)

## What we build

- **Evaluate** — compile an evaluation contract from your agent's goal,
  generate public / hidden / OOD / adversarial scenarios, and score clean
  performance with contamination and hack-risk analysis.
- **Gate** — a contamination-resistant promotion gate: clean
  verified-generalization score (CleanVGS), generalization gap, and an
  ACCEPT / REJECT / LIMITED_ROLLOUT decision with an assurance card.
- **Improve** — human-reviewed improvement suggestions and candidate agent
  configs, re-verified by the gate. Improvements are never auto-applied.
- **Substrate** — clean feedback records, transfer metrics, failure memory,
  and generated curriculum for teams building increasingly general agents.

The privacy-preserving default is evaluate-only: nothing is exported,
nothing is reused for training, and human review is required.

## Formal foundation

Selected mathematical properties behind the contamination-resistant promotion gate are machine-verified in Lean 4. The implementation is property-tested against the formal specification.

The Lean 4 development and its Python property-test mirror are open source
in [verifiable-labs-envs](https://github.com/verifiablelabs/verifiable-labs-envs)
(`formal/` and `src/verifiable_labs_envs/formal_spec/`).

## Open core

| Repository | What it holds |
|---|---|
| [verifiable-labs-envs](https://github.com/verifiablelabs/verifiable-labs-envs) | SDK, 25 procedurally generated environments, formal track, CLI (Apache-2.0) |
| [vlabs-sdk](https://github.com/verifiablelabs/vlabs-sdk) | SDK contracts: run modes, provider interface, schemas (pointer) |
| [vlabs-formal](https://github.com/verifiablelabs/vlabs-formal) | Lean 4 formal track + property-test mirror (pointer) |
| [vlabs-examples](https://github.com/verifiablelabs/vlabs-examples) | Public-safe examples and quickstarts |
| [vlabs-evidence](https://github.com/verifiablelabs/vlabs-evidence) | Redacted sample assurance cards and aggregate metrics |
| [vlabs-docs](https://github.com/verifiablelabs/vlabs-docs) | Product and positioning documentation |

The evaluation platform (scenario generation, contamination firewall,
anti-hack engine, billing, API) is private. Hidden evaluation content, gold
answers, detection details, customer data, and raw traces are never
published — that separation is what keeps the feedback clean.

## Published evidence

Public, **synthetic / redacted** demo evidence:

- **Hugging Face dataset** — <https://huggingface.co/datasets/verifiablelabs/vlabs-clean-gate-evidence>
- **Weights & Biases** (entity `verifiable-labs`): [clean-generalization-gate](https://wandb.ai/verifiable-labs/clean-generalization-gate) · [contamination-firewall](https://wandb.ai/verifiable-labs/contamination-firewall) · [anti-hack-engine](https://wandb.ai/verifiable-labs/anti-hack-engine) · [scenario-compiler](https://wandb.ai/verifiable-labs/scenario-compiler) · [runpod-costs](https://wandb.ai/verifiable-labs/runpod-costs)

All published evidence is **synthetic / redacted** and is **not a training
dataset**. It contains **no** customer data, hidden evaluations, gold
answers, raw traces, private anti-hack traps, or private engine internals.

Install the SDK: `pip install "vlabs-sdk==0.0.2"`

## Links

- Website: <https://verifiable-labs.com>
- Security policy: see `SECURITY.md` in this repository
