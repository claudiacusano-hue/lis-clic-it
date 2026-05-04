
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

## 3. LLM-based Sign Language Production
https://ieeexplore.ieee.org/document/10903313

This paper proposes a novel approach to Sign Language Production (SLP) that utilizes Large Language Models (LLMs) to translate natural language text directly into motion sequences. The methodology is split into two distinct phases:
* Text-to-Pose Mapping: The researchers fine-tuned LLMs (LLaMA-7B and Vicuna-7B) using LoRA (Low-Rank Adaptation) to map spoken text to discrete pose tokens. These tokens are created using a VQ-VAE (Vector Quantized Variational Autoencoder) to represent body keypoints.
* Pose-to-Image Synthesis: The generated poses are then processed by a Conditional VAE-GAN to create realistic images of a specific person (signer) performing the signs.
The system was tested on the SynLibras-Pose (Brazilian Sign Language) and RWTH-PHOENIX-Weather (German Sign Language) datasets, demonstrating that LLMs can effectively handle the cross-modal task of translating text into coherent sign language motion sequences.

```
@inproceedings{silveira2024llm,
  title={LLM-based Sign Language Production},
  author={Silveira, Wellington and Mendon{\c{c}}a, Luca and De Bem, Rodrigo},
  booktitle={2024 International Conference on Machine Learning and Applications (ICMLA)},
  pages={1685--1690},
  year={2024},
  organization={IEEE}
}
```

## 4. Signing at Scale: Learning to Co-Articulate Signs for Large-Scale Photo-Realistic Sign Language Production
https://openaccess.thecvf.com/content/CVPR2022/html/Saunders_Signing_at_Scale_Learning_to_Co-Articulate_Signs_for_Large-Scale_Photo-Realistic_CVPR_2022_paper.html

This research addresses the limitations of traditional SLP models, which often produce "under-articulated" signs that lack the natural flow, or co-articulation, found in human signing. The authors introduce a multi-stage framework designed for unconstrained domains of discourse:
* FS-NET (Frame Selection Network): This novel component learns to create smooth transitions between signs by selecting the optimal subset of frames from dictionary signs to match a continuous signing sequence.
* SIGNGAN: A video-to-video synthesis model that generates high-resolution, photo-realistic sign language videos from skeleton poses.
* Hand Keypoint Loss: To overcome the common problem of blurred or inaccurate hand generation, the authors developed a specific loss function that focuses on hand keypoints, significantly improving the clarity and understandability of the signs.

Evaluated on the large-scale meineDGS corpus, the model proved to be significantly more understandable to native deaf signers than previous skeletal or isolated-sign approaches.


```
@inproceedings{saunders2022signing,
  title={Signing at scale: Learning to co-articulate signs for large-scale photo-realistic sign language production},
  author={Saunders, Ben and Camgoz, Necati Cihan and Bowden, Richard},
  booktitle={Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition},
  pages={5141--5151},
  year={2022}
}
```
# Risorse LIS
---
## 1. Grammatica della lingua dei segni italiana (LIS)
https://edizionicafoscari.unive.it/it/edizioni/libri/978-88-6969-645-9/

```
@book{Branchini_2022,
	doi = {10.30687/978-88-6969-645-9},
	url = {https://doi.org/10.30687%2F978-88-6969-645-9},
	year = 2022,
	month = {dec},
	publisher = {Fondazione Universit{\`{a}} Ca' Foscari},
	author = {Chiara Branchini and Lara Mantovan},
	title = {Grammatica della lingua dei segni italiana ({LIS})}
}
```
