# Awesome-Robotics-Foundation-Model-How-To [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of tools, needed to train robotics foundation models from scratch.

## Table of Contents

- [Awesome-Robotics-Foundation-Model-How-To ](#awesome-robotics-foundation-model-how-to-)
  - [Table of Contents](#table-of-contents)
  - [How to build a foundation model from scratch?](#how-to-build-a-foundation-model-from-scratch)
    - [Technical Background](#technical-background)
    - [Models (e.g. Vision Language Models, Robotics Foundation Models)](#models-eg-vision-language-models-robotics-foundation-models)
    - [Datasets and Benchmarks](#datasets-and-benchmarks)
    - [Training Pipeline and deployment](#training-pipeline-and-deployment)
    - [Simulators and Environments](#simulators-and-environments)
    - [Tools](#tools)
  - [Contribute](#contribute)

## How to build a foundation model from scratch?

### Technical Background

|  Date  |       keywords       |    Institute    | Paper | Publication |
| :-----: | :------------------: | :--------------: | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :---------: |
| 2017-06 |     Transformers     |      Google      | [Attention Is All You Need](https://arxiv.org/pdf/1706.03762.pdf)                                                                                                                      |   NeurIPS<br>  ![Dynamic JSON Badge](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fapi.semanticscholar.org%2Fgraph%2Fv1%2Fpaper%2F204e3073870fae3d05bcbc2f6a8e263d9b72e776%3Ffields%3DcitationCount&query=%24.citationCount&label=citation) |
| 2018-06 |       GPT 1.0       |      OpenAI      | [Improving Language Understanding by Generative Pre-Training](https://www.cs.ubc.ca/~amuham01/LING530/papers/radford2018improving.pdf)                                                 |  ![Dynamic JSON Badge](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fapi.semanticscholar.org%2Fgraph%2Fv1%2Fpaper%2Fcd18800a0fe0b668a1cc19f2ec95b5003d0a5035%3Ffields%3DcitationCount&query=%24.citationCount&label=citation)          |

### Models (e.g. Vision Language Models, Robotics Foundation Models)

|  Date  |       keywords       |    Institute    | Paper                                                                                                                                                                               | Publication |
| :-----: | :------------------: | :--------------: | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :---------: |
| 2022-12 |     VLA     |      Google      | [RT-1: Robotics Transformer for Real-World Control at Scale](https://arxiv.org/abs/2212.06817)                                                                                                                      |   ![Dynamic JSON Badge](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fapi.semanticscholar.org%2Fgraph%2Fv1%2Fpaper%2Ffd1cf28a2b8caf2fe29af5e7fa9191cecfedf84d%3Ffields%3DcitationCount&query=%24.citationCount&label=citation) |
| 2023-07 |     VLA     |      Google DeepMind      | [RT-2: Vision-Language-Action Models Transfer Web Knowledge to Robotic Control](https://arxiv.org/abs/2307.15818)                                                                                                                      |   ![Dynamic JSON Badge](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fapi.semanticscholar.org%2Fgraph%2Fv1%2Fpaper%2F38939304bb760473141c2aca0305e44fbe04e6e8%3Ffields%3DcitationCount&query=%24.citationCount&label=citation) |
| 2023-10 |     VLA     |      Google et al.      | [Open X-Embodiment: Robotic Learning Datasets and RT-X Models](https://arxiv.org/abs/2310.08864)                                                                                                                      |   ![Dynamic JSON Badge](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fapi.semanticscholar.org%2Fgraph%2Fv1%2Fpaper%2Fef7d31137ef06c5be8c2824ecc5af6ce3358cc8f%3Ffields%3DcitationCount&query=%24.citationCount&label=Citations) |
| 2024-05 |     VLA     |      UC Berkley et al.      | [Octo: An Open-Source Generalist Robot Policy](https://arxiv.org/abs/2310.08864)                                                                                                                      |   ![Dynamic JSON Badge](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fapi.semanticscholar.org%2Fgraph%2Fv1%2Fpaper%2F1d2753d74025e7a71594506623be81f18b073adb%3Ffields%3DcitationCount&query=%24.citationCount&label=Citations) |


### Datasets and Benchmarks

|  Date  |       keywords       |    Institute    | Paper                                                                                                                                                                               | Publication |
| :-----: | :------------------: | :--------------: | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :---------: |
| 2024-02 |  Dataset | Stanford et al. | [Pushing the Limits of Cross-Embodiment Learning for Manipulation and Navigation](https://arxiv.org/abs/2402.19432) | RSS 2024 |
| 2024-05 |     Simulation     |      UCSD et al.      | [Evaluating Real-World Robot Manipulation Policies in Simulation](https://arxiv.org/pdf/2405.05941)                                                                                                                      |   ![Dynamic JSON Badge](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fapi.semanticscholar.org%2Fgraph%2Fv1%2Fpaper%2F202cc3fcea588cee37ffabcb0b5e145567109a66%3Ffields%3DcitationCount&query=%24.citationCount&label=Citations) |
| 2024-03 |     Dataset     |      UCB et al.      | [DROID: A Large-Scale In-The-Wild Robot Manipulation Dataset](https://arxiv.org/abs/2403.12945)                                                                                                                      |   ![Dynamic JSON Badge](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fapi.semanticscholar.org%2Fgraph%2Fv1%2Fpaper%2Fee5070fe52fd17da9a89d3f342fb07cc9ae51afe%3Ffields%3DcitationCount&query=%24.citationCount&label=Citations) |
| 2023-10 |     Dataset     |     Google et al.      | [Open X-Embodiment: Robotic Learning Datasets and RT-X Models](https://arxiv.org/abs/2310.08864)                                                                                                                      |   ![Dynamic JSON Badge](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fapi.semanticscholar.org%2Fgraph%2Fv1%2Fpaper%2Fef7d31137ef06c5be8c2824ecc5af6ce3358cc8f%3Ffields%3DcitationCount&query=%24.citationCount&label=Citations) |
| 2023-06 |     Simulation     |   Meta AI      | [HomeRobot: Open-Vocabulary Mobile Manipulation](https://arxiv.org/abs/2306.11565)                                                                                                                      |   ![Dynamic JSON Badge](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fapi.semanticscholar.org%2Fgraph%2Fv1%2Fpaper%2F3b0c02955e88f5862e61b560c7f70ba8cf235b1d%3Ffields%3DcitationCount&query=%24.citationCount&label=Citations) |
| 2023-09 |     Dataset     |   Stanford et al.     | [Physically Grounded Vision-Language Models for Robotic Manipulation](https://arxiv.org/abs/2309.02561)                                                                                                                      |   ![Dynamic JSON Badge](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fapi.semanticscholar.org%2Fgraph%2Fv1%2Fpaper%2F316f980cfd2e217234386166a46eb080bf027cdd%3Ffields%3DcitationCount&query=%24.citationCount&label=Citations) |
| 2023-11 |     Dataset     |   Google DeepMind     | [RoboVQA: Multimodal Long-Horizon Reasoning for Robotics](https://arxiv.org/abs/2311.00899)                                                                                                                      |   ![Dynamic JSON Badge](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fapi.semanticscholar.org%2Fgraph%2Fv1%2Fpaper%2F0b47356f17aea1de66e39e5f182a105c96af8dd3%3Ffields%3DcitationCount&query=%24.citationCount&label=Citations) |

### Training Pipeline and deployment

|  Date  |       keywords       |    Institute    | Paper                                                                                                                                                                               | Publication |
| :-----: | :------------------: | :--------------: | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :---------: |
| 2018-06 |       GPT 1.0       |      OpenAI      | [Improving Language Understanding by Generative Pre-Training](https://www.cs.ubc.ca/~amuham01/LING530/papers/radford2018improving.pdf)                                                 |  ![Dynamic JSON Badge](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fapi.semanticscholar.org%2Fgraph%2Fv1%2Fpaper%2Fcd18800a0fe0b668a1cc19f2ec95b5003d0a5035%3Ffields%3DcitationCount&query=%24.citationCount&label=citation)          |
| 2024-08 |       LLM       |      Lightning AI et al.      | [Build a Large Language Model (From Scratch)](https://www.manning.com/books/build-a-large-language-model-from-scratch)                                                 |           |

### Simulators and Environments

|  Date  |       keywords       |    Institute    | Paper                                                                                                                                                                               | Publication |
| :-----: | :------------------: | :--------------: | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :---------: |
|  |     Mujoco     |      Google      | [Attention Is All You Need](https://arxiv.org/pdf/1706.03762.pdf)                                                                                                                      |   NeurIPS<br>  ![Dynamic JSON Badge](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fapi.semanticscholar.org%2Fgraph%2Fv1%2Fpaper%2F204e3073870fae3d05bcbc2f6a8e263d9b72e776%3Ffields%3DcitationCount&query=%24.citationCount&label=citation) |
| |       Calcin       |      OpenAI      | [Improving Language Understanding by Generative Pre-Training](https://www.cs.ubc.ca/~amuham01/LING530/papers/radford2018improving.pdf)                                                 |   |

### Tools

|  Date  |       keywords       |    Institute    | Paper                                                                                                                                                                               | Publication |
| :-----: | :------------------: | :--------------: | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :---------: |
|  |     Fog-RT-X     |      BerkleyAutomation      | [Fog-RT-X](https://github.com/BerkeleyAutomation/fog_x/)                                                                                                                      |    |

## Contribute

Contributions welcome! Read the [contribution guidelines](contributing.md) first.

This list was generated with the help of [generator-awesome-list](https://github.com/dar5hak/generator-awesome-list).
