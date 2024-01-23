# Awesome LLM for NLG Evaluation Papers
[![Awesome](https://awesome.re/badge.svg)]() 
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
![](https://img.shields.io/badge/PRs-Welcome-red) 
<!-- ![](https://img.shields.io/github/last-commit/zjunlp/Prompt4ReasoningPapers?color=green)  -->

## 💡 News
- **2024-1-13**: 📃 We release a survey paper on LLM for NLG/text generation evaluation. "[Leveraging Large Language Models for NLG Evaluation: A Survey](https://arxiv.org/abs/2401.07103)". Welcome to read and cite it. We are looking forward to your feedback and suggestions.

## 📒 Table of Contents
- [⭐ Introduction](#-introduction)
- [📃 Papers](#awesome-llm-for-nlg-evaluation-papers)
    - [Generative Evaluation](#generative-evaluation)
        - [Prompt-based](#prompt-based)
            - [Score-based](#score-based)
            - [Probability-based](#probability-based)
            - [Likert-style](#likert-style)
            - [Pairwise Comparison](#pairwise-comparison)
            - [Ensemble](#ensemble)
            - [Advanced](#advanced)
        - [Tuning-based](#tuning-based)
            - [Probability-based](#t-probability-based)
            - [Likert-style](#t-likert-style)
            - [Pairwise Comparison](#t-pairwise-comparison)
            - [Advanced](#t-advanced)
    - [Meta-Evaluation Benchmarks](#meta-evaluation-benchmarks)
        - [Machine Translation](#machine-translation)
        - [Text Summarization](#text-summarization)
        - [Dialogue Generation](#dialogue-generation)
        - [Image Caption](#image-caption)
        - [Data-to-Text](#data-to-text)
        - [Story Generation](#story-generation)
        - [General Generation](#general-generation)
- [🔍 Resources](#-resources)
    - [Tools](#tools)
- [🚩 Citation](#-citation)

--- 

<a id="-introduction"></a>
## ⭐ Introduction
In the rapidly evolving domain of Natural Language Generation (NLG) evaluation, introducing Large Language Models (LLMs) has opened new avenues for assessing generated content quality, e.g., coherence, creativity, and context relevance. This survey aims to provide a thorough overview of leveraging LLMs for NLG evaluation, a burgeoning area that lacks a systematic analysis. We propose a coherent taxonomy for organizing existing LLM-based evaluation metrics, offering a structured framework to understand and compare these methods. Our detailed exploration includes critically assessing various LLM-based methodologies, as well as comparing their strengths and limitations in evaluating NLG outputs. By discussing unresolved challenges, including bias, robustness, domain-specificity, and unified evaluation, this survey seeks to offer insights to researchers and advocate for fairer and more advanced NLG evaluation techniques.
<!-- 
We hope this repository can help researchers and practitioners to get a better understanding of this emerging field. If this repository is helpful for you, please help us by citing this paper:
```bash
@misc{li2024leveraging,
      title={Leveraging Large Language Models for NLG Evaluation: A Survey}, 
      author={Zhen Li and Xiaohan Xu and Tao Shen and Can Xu and Jia-Chen Gu and Chongyang Tao},
      year={2024},
      eprint={2401.07103},
      archivePrefix={arXiv},
      primaryClass={cs.CL}
}
``` -->

## Generative Evaluation
### Prompt-based
#### Score-based
- Large Language Models Are State-of-the-Art Evaluators of Translation Quality [[paper]](https://aclanthology.org/2023.eamt-1.19/)
- LLM-Eval: Unified Multi-Dimensional Automatic Evaluation for Open-Domain Conversations with Large Language Models [[paper]](https://arxiv.org/abs/2305.13711)
- Evaluate What You Can't Evaluate: Unassessable Quality for Generated Response [[paper]](https://arxiv.org/abs/2305.14658)
- Is ChatGPT a Good NLG Evaluator? A Preliminary Study [[paper]](https://arxiv.org/abs/2303.04048)
- Multi-Dimensional Evaluation of Text Summarization with In-Context Learning [[paper]](https://arxiv.org/abs/2306.01200)

#### Probability-based
- BARTScore: Evaluating Generated Text as Text Generation [[paper]](https://arxiv.org/abs/2106.11520)
- GPTScore: Evaluate as You Desire [[paper]](https://arxiv.org/abs/2302.04166)
- Zero-shot Faithfulness Evaluation for Text Summarization with Foundation Language Model [[paper]](https://aclanthology.org/2023.emnlp-main.679/)

#### Likert-style
- Large Language Models Are State-of-the-Art Evaluators of Translation Quality [[paper]](https://aclanthology.org/2023.eamt-1.19/)
- ChatGPT as a Factual Inconsistency Evaluator for Text Summarization [[paper]](https://arxiv.org/abs/2303.15621)
- Human-like summarization evaluation with chatgpt [[paper]](https://arxiv.org/abs/2304.02554)
- Towards Better Evaluation of Instruction-Following: A Case-Study in Summarization [[paper]](https://arxiv.org/abs/2310.08394)
- Investigating Table-to-Text Generation Capabilities of LLMs in Real-World Information Seeking Scenarios [[paper]](https://arxiv.org/abs/2305.14987)
- Automatic Evaluation of Attribution by Large Language Models [[paper]](https://arxiv.org/abs/2305.06311)
- Exploring the use of large language models for reference-free text quality evaluation: A preliminary empirical study [[paper]](https://arxiv.org/abs/2304.00723)
- ChatGPT Outperforms Crowd-Workers for Text-Annotation Tasks [[paper]](https://export.arxiv.org/abs/2303.15056v2)
- Benchmarking Foundation Models with Language-Model-as-an-Examiner [[paper]](https://arxiv.org/abs/2306.04181)
- Is ChatGPT better than Human Annotators? Potential and Limitations of ChatGPT in Explaining Implicit Hate Speech [[paper]](https://arxiv.org/abs/2302.07736)
- Less is More for Long Document Summary Evaluation by LLMs [[paper]](https://arxiv.org/abs/2309.07382)
- Judging LLM-as-a-Judge with MT-Bench and Chatbot Arena [[paper]](https://arxiv.org/abs/2306.05685)
- Large Language Models Are State-of-the-Art Evaluators of Code Generation [[paper]](https://arxiv.org/abs/2304.14317)
- Evaluation Metrics in the Era of GPT-4: Reliably Evaluating Large Language Models on Sequence to Sequence Tasks [[paper]](https://arxiv.org/abs/2310.13800)
- Text Style Transfer Evaluation Using Large Language Models [[paper]](https://arxiv.org/abs/2308.13577)
- Calibrating LLM-Based Evaluator [[paper]](https://arxiv.org/abs/2309.13308)
- Can Large Language Models Be an Alternative to Human Evaluations? [[paper]](https://aclanthology.org/2023.acl-long.870/)

#### Pairwise Comparison
- ChatGPT as a Factual Inconsistency Evaluator for Text Summarization [[paper]](https://arxiv.org/abs/2303.15621)
- Human-like summarization evaluation with chatgpt [[paper]](https://arxiv.org/abs/2304.02554)
- Large Language Models are not Fair Evaluators [[paper]](https://arxiv.org/abs/2305.17926)
- Exploring ChatGPT's Ability to Rank Content: A Preliminary Study on Consistency with Human Preferences [[paper]](https://arxiv.org/abs/2303.07610)
- Judging LLM-as-a-Judge with MT-Bench and Chatbot Arena [[paper]](https://arxiv.org/abs/2306.05685)
- EvalLM: Interactive Evaluation of Large Language Model Prompts on User-Defined Criteria [[paper]](https://arxiv.org/abs/2309.13633)
- Benchmarking Foundation Models with Language-Model-as-an-Examiner [[paper]](https://arxiv.org/abs/2306.04181)
- Exploring the use of large language models for reference-free text quality evaluation: A preliminary empirical study [[paper]](https://arxiv.org/abs/2304.00723)
- Automated Evaluation of Personalized Text Generation using Large Language Models [[paper]](https://arxiv.org/abs/2310.11593)

#### Ensemble
- Large Language Models are Diverse Role-Players for Summarization Evaluation [[paper]](https://arxiv.org/abs/2303.15078)
- Wider and Deeper LLM Networks are Fairer LLM Evaluators [[paper]](https://arxiv.org/abs/2308.01862)
- ChatEval: Towards Better LLM-based Evaluators through Multi-Agent Debate [[paper]](https://arxiv.org/abs/2308.07201)
- PRD: Peer Rank and Discussion Improve Large Language Model based Evaluations [[paper]](https://arxiv.org/abs/2307.02762)

#### Advanced
- Error Analysis Prompting Enables Human-Like Translation Evaluation in Large Language Models: A Case Study on ChatGPT [[paper]](https://arxiv.org/abs/2303.13809)
- G-Eval: NLG Evaluation using GPT-4 with Better Human Alignment [[paper]](https://arxiv.org/abs/2303.16634)
- FActScore: Fine-grained Atomic Evaluation of Factual Precision in Long Form Text Generation [[paper]](https://arxiv.org/abs/2305.14251)
- ALLURE: A Systematic Protocol for Auditing and Improving LLM-based Evaluation of Text using Iterative In-Context-Learning [[paper]](https://arxiv.org/abs/2309.13701v1)
- Not All Metrics Are Guilty: Improving NLG Evaluation with LLM Paraphrasing [[paper]](https://arxiv.org/abs/2305.15067)

### Tuning-based

<a id="t-probability-based"></a>
#### Probability-based
- Automatic Machine Translation Evaluation in Many Languages via Zero-Shot Paraphrasing [[paper]](https://aclanthology.org/2020.emnlp-main.8/)
- T5Score: Discriminative Fine-tuning of Generative Evaluation Metrics [[paper]](https://arxiv.org/abs/2212.05726)

<a id="t-likert-style"></a>
#### Likert-style
- TrueTeacher: Learning Factual Consistency Evaluation with Large Language Models [[paper]](https://arxiv.org/abs/2305.11171)
- Learning Personalized Story Evaluation [[paper]](https://arxiv.org/abs/2310.03304)
- Automatic Evaluation of Attribution by Large Language Models [[paper]](https://arxiv.org/abs/2305.06311)
- Generative Judge for Evaluating Alignment [[paper]](https://arxiv.org/abs/2310.05470)
- Prometheus: Inducing Fine-grained Evaluation Capability in Language Models [[paper]](https://arxiv.org/abs/2310.08491)
- CritiqueLLM: Scaling LLM-as-Critic for Effective and Explainable Evaluation of Large Language Model Generation [[paper]](https://arxiv.org/abs/2311.18702)
- X-Eval: Generalizable Multi-aspect Text Evaluation via Augmented Instruction Tuning with Auxiliary Evaluation Aspects [[paper]](https://arxiv.org/abs/2311.08788)

<a id="t-pairwise-comparison"></a>
#### Pairwise Comparison
- PandaLM: An Automatic Evaluation Benchmark for LLM Instruction Tuning Optimization [[paper]](https://arxiv.org/abs/2306.05087)
- Generative Judge for Evaluating Alignment [[paper]](https://arxiv.org/abs/2310.05470)
- Judging LLM-as-a-Judge with MT-Bench and Chatbot Arena [[paper]](https://arxiv.org/abs/2306.05685)
- Learning Personalized Story Evaluation [[paper]](https://arxiv.org/abs/2310.03304)
- Prometheus: Inducing Fine-grained Evaluation Capability in Language Models [[paper]](https://arxiv.org/abs/2310.08491)

<a id="t-advanced"></a>
#### Advanced
- INSTRUCTSCORE: Towards Explainable Text Generation Evaluation with Automatic Feedback [[paper]](https://aclanthology.org/2023.emnlp-main.365/)
- TIGERScore: Towards Building Explainable Metric for All Text Generation Tasks [[paper]](https://arxiv.org/abs/2310.00752)

## Meta-Evaluation Benchmarks 
### Machine Translation

- Experts, Errors, and Context: A Large-Scale Study of Human Evaluation for Machine Translation [[paper]](https://aclanthology.org/2021.tacl-1.87) 
- Results of the WMT20 Metrics Shared Task [[paper]](https://aclanthology.org/2020.wmt-1.77)
- Results of the WMT21 Metrics Shared Task: Evaluating Metrics with Expert-based Human Evaluations on TED and News Domain [[paper]](https://aclanthology.org/2021.wmt-1.73)
- Results of the WMT22 Metrics Shared Task: Stop Using BLEU -- Neural Metrics Are Better and More Robust [[paper]](https://aclanthology.org/2022.wmt-1.2)

### Text Summarization

- Newsroom: A Dataset of 1.3 Million Summaries with Diverse Extractive Strategies [[paper]](https://aclanthology.org/N18-1065)
- SAMSum Corpus: A Human-annotated Dialogue Dataset for Abstractive Summarization [[paper]](https://arxiv.org/abs/1911.12237)
- Re-evaluating Evaluation in Text Summarization [[paper]](https://aclanthology.org/2020.emnlp-main.751/)
- Asking and Answering Questions to Evaluate the Factual Consistency of Summaries [[paper]](https://aclanthology.org/2020.acl-main.450/)
- Understanding Factuality in Abstractive Summarization with {FRANK}: A Benchmark for Factuality Metrics [[paper]](https://aclanthology.org/2021.naacl-main.383/)
- SummEval: Re-evaluating Summarization Evaluation [[paper]](https://aclanthology.org/2021.tacl-1.24/)
- SummaC: Re-Visiting NLI-based Models for Inconsistency Detection in Summarization [[paper]](https://aclanthology.org/2022.tacl-1.10/)
- RiSum: Towards Better Evaluation of Instruction-Following: A Case-Study in Summarization [[paper]](https://arxiv.org/abs/2310.08394)
- OpinSummEval: Revisiting Automated Evaluation for Opinion Summarization [[paper]](https://arxiv.org/abs/2310.18122)

### Dialogue Generation

- Unsupervised Evaluation of Interactive Dialog with DialoGPT [[paper]](https://aclanthology.org/2020.sigdial-1.28/)
- Topical-Chat: Towards Knowledge-Grounded Open-Domain Conversations [[paper]](https://arxiv.org/abs/2308.11995)
- Personalizing Dialogue Agents: I have a dog, do you have pets too? [[paper]](https://arxiv.org/abs/1801.07243)

### Image Caption

- Framing Image Description as a Ranking Task: Data, Models and Evaluation Metrics [[paper]](https://www.jair.org/index.php/jair/article/view/10833)
- From Images to Sentences Through Scene Description Graphs Using Commonsense Reasoning and Knowledge [[paper]](https://arxiv.org/abs/1511.03292)
- Cider: Consensus-based Image Description Evaluation [[paper]](https://www.cv-foundation.org/openaccess/content_cvpr_2015/papers/Vedantam_CIDEr_Consensus-Based_Image_2015_CVPR_paper.pdf)
- Learning to Evaluate Image Captioning [[paper]](https://openaccess.thecvf.com/content_cvpr_2018/papers/Cui_Learning_to_Evaluate_CVPR_2018_paper.pdf)

### Data-to-Text

- Phrase-Based & Neural Unsupervised Machine Translation [[paper]](https://aclanthology.org/P10-1157)
- Semantically Conditioned LSTM-based Natural Language Generation for Spoken Dialogue Systems [[paper]](https://aclanthology.org/D15-1199)
- The 2020 Bilingual, Bi-Directional WebNLG+ Shared Task: Overview and Evaluation Results (WebNLG+ 2020) [[paper]](https://aclanthology.org/2020.webnlg-1.7/)

### Story Generation

- OpenMEVA: A Benchmark for Evaluating Open-Ended Story Generation Metrics [[paper]](https://aclanthology.org/2021.acl-long.500)
- StoryER: Automatic Story Evaluation via Ranking, Rating and Reasoning [[paper]](https://aclanthology.org/2022.emnlp-main.114)
- Learning Personalized Story Evaluation [[paper]](https://arxiv.org/abs/2310.03304)

### General Generation

- AlpacaEval: An Automatic Evaluator of Instruction-following Models [[Github]](https://github.com/tatsu-lab/alpaca_eval)
- Judging LLM-as-a-judge with MT-Bench and Chatbot Arena [[paper]](https://arxiv.org/abs/2306.05685)
- Large Language Models are not Fair Evaluators [[paper]](https://arxiv.org/abs/2305.17926)
- Shepherd: A Critic for Language Model Generation [[paper]](https://arxiv.org/abs/2308.04592)
- Evaluating Large Language Models at Evaluating Instruction Following [[paper]](https://arxiv.org/abs/2310.07641)
- Wider and Deeper LLM Networks are Fairer LLM Evaluators [[paper]](https://arxiv.org/abs/2308.01862)
- Automatic Evaluation of Attribution by Large Language Models [[paper]](https://arxiv.org/abs/2305.06311)
- AlignBench: Benchmarking Chinese Alignment of Large Language Models [[paper]](https://arxiv.org/abs/2311.18743)

<a id="-resources"></a>
## 🔍 Resources
### Tools

<a id="-citation"></a>
## 🚩 Citation
If this survey is helpful for you, please help us by citing this paper:
```bash
@misc{li2024leveraging,
      title={Leveraging Large Language Models for NLG Evaluation: A Survey}, 
      author={Zhen Li and Xiaohan Xu and Tao Shen and Can Xu and Jia-Chen Gu and Chongyang Tao},
      year={2024},
      eprint={2401.07103},
      archivePrefix={arXiv},
      primaryClass={cs.CL}
}
```
