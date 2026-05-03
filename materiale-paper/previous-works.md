
# Synthetic Data for Low-resource Languages

## 1. Transcending Language Boundaries: Harnessing LLMs for Low-Resource Language Translation
https://arxiv.org/abs/2411.11295

This paper explores the challenges of using Large Language Models (LLMs) like GPT-4o and LLaMA 3.1 to translate English into three low-resource languages: Cherokee, Tibetan, and Manchu. The authors highlight that while LLMs excel in high-resource languages, they often struggle with low-resource ones due to limited training data, leading to hallucinations and inaccurate translations.
To address this, the study introduces a retrieval-based method (Retrieval-Augmented Generation or RAG) that uses a dual mechanism—keyword-based lookup for exact matches and vector-based retrieval for semantic similarity—to pull relevant context from existing linguistic resources like dictionaries and the New Testament. Their findings demonstrate that this RAG approach significantly improves word-level accuracy and semantic understanding over zero-shot models, although capturing deep cultural and contextual nuances remains a hurdle, particularly for the Cherokee language.

```
@misc{shu2024transcendinglanguageboundariesharnessing,
      title={Transcending Language Boundaries: Harnessing LLMs for Low-Resource Language Translation}, 
      author={Peng Shu and Junhao Chen and Zhengliang Liu and Hui Wang and Zihao Wu and Tianyang Zhong and Yiwei Li and Huaqin Zhao and Hanqi Jiang and Yi Pan and Yifan Zhou and Constance Owl and Xiaoming Zhai and Ninghao Liu and Claudio Saunt and Tianming Liu},
      year={2024},
      eprint={2411.11295},
      archivePrefix={arXiv},
      primaryClass={cs.CL},
      url={https://arxiv.org/abs/2411.11295}, 
}
```

## 2. InstructLR: A Scalable Approach to Create Instruction Dataset for Under-Resourced Languages
https://arxiv.org/abs/2512.02213

This study presents InstructLR, a novel framework designed to create high-quality instruction-tuning datasets for under-represented African languages, specifically Zarma, Bambara, and Fulfulde. The authors argue that traditional machine translation and purely synthetic data generation often fail to capture linguistic nuances and cultural awareness.
The InstructLR pipeline works by generating seed instructions in a high-resource language (e.g., French) and then using an LLM to generate corresponding instruction-response pairs in the target language. The framework features a dual-layer quality filtering mechanism:
* Layer 1: An automated RAG-based checker that uses grammar rules and glossaries to flag or correct drafts.
* Layer 2: A human-in-the-loop validation layer where native speakers review flagged content.
The approach successfully created three 50k-scale multi-domain benchmarks and reduced dataset creation costs by 88% while significantly improving model performance compared to traditional translation baselines.

```
@misc{keita2026instructlrscalableapproachcreate,
      title={InstructLR: A Scalable Approach to Create Instruction Dataset for Under-Resourced Languages}, 
      author={Mamadou K. Keita and Sebastien Diarra and Christopher Homan and Seydou Diallo},
      year={2026},
      eprint={2512.02213},
      archivePrefix={arXiv},
      primaryClass={cs.LG},
      url={https://arxiv.org/abs/2512.02213}, 
}
```
