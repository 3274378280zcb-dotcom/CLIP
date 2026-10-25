# MIAE01 - Reproduction of CLIP

Reproduction of *Learning Transferable Visual Models From Natural Language Supervision* (CLIP), Radford et al., ICML 2021.

| Item | Detail |
| --- | --- |
| Course | MIAE01 - Machine Learning Programming and Tools, 2026-2027 |
| Paper | arXiv:2103.00020 - https://arxiv.org/abs/2103.00020 |
| Original code | https://github.com/openai/CLIP |
| Starting commit | d05afc436d78f1c48dc0dbf8e5980a9d471f35f6 |
| Original license | MIT - see THIRD_PARTY_LICENSE |
| Author | 张崇彬, 2260032166 |

## Status

Week 1: repository initialised. Environment setup, data pipeline and evaluation scripts are in preparation.

## Team

| Name | Student ID |
| --- | --- |
| 张崇彬 | 2260032166 |

The group currently has one member. The teaching team may assign additional members before the presentation; if the group composition or the assigned paper changes, this repository will be updated accordingly.

## Planned layout

```
code/      reproduction source code, adapted from the original repository
configs/   experiment configuration files
scripts/   scripts that download data and pretrained weights
logs/      run logs, one per run, used as evidence for every reported number
results/   aggregated results, tables and figures
```

## Environment

To be completed once the environment is fixed. No value is stated here until it has been verified.

- Hardware: TBD (GPU model and memory will be recorded)
- Python: TBD
- Key libraries: PyTorch, torchvision, NumPy - versions to be pinned in requirements.txt
- Random seeds: fixed per experiment and recorded in configs/

## Reproduction plan

1. Claim 1 - zero-shot ImageNet transfer: zero-shot top-1 accuracy compared with the value reported in the paper.
2. Claim 2 - linear probe: linear-probe accuracy on a reduced set of datasets.
3. Extension - one factor changed at a time (for example a prompt-template sweep or a robustness test) with the same seeds and the same computational budget.

A reduced scale is acceptable if stated. Every deviation from the paper will be listed in a deviation table with the original setting, the setting used and the reason.

## Data and weights

Datasets and pretrained weights are not committed to this repository. They are obtained by the scripts in `scripts/`, as required by the course instructions.

## Credits and license

The starting code is the official implementation at https://github.com/openai/CLIP, released under the MIT license; the license text is kept in THIRD_PARTY_LICENSE. All files modified relative to the starting commit will be listed in MODIFICATIONS.md.
