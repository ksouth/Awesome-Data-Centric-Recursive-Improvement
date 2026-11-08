# Candidate mapping onto the survey's stages (v1)

Version v1 · 8 November 2026 · Author: Claude (Haiku 5.5)

The survey's inclusion test is: the work uses evaluation feedback to update a data-related object, introduces a reusable data, evaluation or control operator, or analyses closed-loop risk. The fit column applies that test. None of these papers is cited in the survey README, as checked on 8 November 2026.

| Candidate | Link | Survey stage | Fit | Status |
|---|---|---|---|---|
| LLM2LLM (ACL 2024) | https://arxiv.org/abs/2403.15042 · code https://github.com/SqueezeAILab/LLM2LLM | Execution: SFT data augmentation, from the student's failures | Strong: failures drive new data | Paper checked; code page checked (MIT, 196 stars, 3 commits) |
| SEAL (NeurIPS 2025) | https://arxiv.org/abs/2506.10943 · code https://github.com/Continual-Intelligence/SEAL | Execution: self-generated edits trained with RL on downstream reward | Strong: reward updates the edit generator | Paper checked; repo link from search snippet, page not opened. Paper reports catastrophic forgetting under repeated edits, a closed-loop risk. |
| I-SHEEP (arXiv 2408.08072) | https://arxiv.org/abs/2408.08072 · code https://github.com/multimodal-art-projection/I-SHEEP | Execution (SFT), with self-assessment as the filter signal | Strong: self-assessment decides data retention | Paper checked; code page checked (17 stars, licence not shown) |
| Loong (camel-ai) | https://github.com/camel-ai/loong | Signal: verifier outcomes. Execution: verifiable synthetic data for SFT or RL | Strong: verifier labels drive data | Page checked (Apache-2.0 code, 509 stars) |
| Meta-Rewarding (Wu et al., 2024) | https://papers.lunadong.com/paper/2256 | Signal: judge rationales. Orchestration: a meta-judge governs the judge. Failure modes: verbosity reward hacking | Strong: covers both judge and data loops | Paper checked via summaries; no code link captured |
| Self-Judge (arXiv 2402.11253) | https://www.arxiv.org/pdf/2402.11253 · code https://github.com/oddqueue/self-judge | Signal: pairwise self-judgment. Execution: on-policy preference tuning | Moderate: judge and update are joined | Paper checked; repo not opened |
| LANCE (EMNLP 2025) | https://aclanthology.org/anthology-files/pdf/emnlp/2025.emnlp-main.914.pdf · code https://github.com/Control-derek/LANCE | Execution: model curates its own post-training data | Moderate: check how much the signal drives curation | Paper checked; repo not opened |
| Test-time Recursive Thinking (arXiv 2602.03094) | https://papers.cool/arxiv/2602.03094 | Execution: context and memory at inference | Moderate: no weight update | Paper checked |
| LLM-as-a-judge survey (arXiv 2411.16594) | https://arxiv.org/abs/2411.16594 | Signal: judge reliability, background reading | Reference rather than entry | Paper checked |

## Not included here

- ICLR 2026 recursive self-improvement workshop papers, such as the self-play titles. Individual papers not checked, so they stay as leads.
- meta-n (arXiv 2608.24735): repo page failed to load twice, so it stays unverified.
- Preprint surveys from 2026 (preprints.org and the hyper.ai summary). Not peer reviewed, and the summaries disagree on paper counts.

## Before any upstream submission

Confirm each entry's canonical link against its venue page, add the short venue names the list uses, and place each paper only once in its primary stage. Then submit through the repo's pull request process, not from this branch.
