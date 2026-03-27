# Automated Hazard Detection on Construction Sites Using Contrastive Language–Image Pre-training (CLIP): A Zero-Shot Learning Approach with Human-Centric Evaluation

---

## Overview  

This repository contains the code for our study on automated hazard detection in construction environments using CLIP. The project leverages zero-shot learning to identify hazards by aligning images with textual descriptions, eliminating the need for task-specific training. to detect hazards directly from natural language descriptions.

---

## Model  

| Model | Type | Description |
|------|------|------------|
| **CLIP (ViT-based)** | Pretrained | Learns joint image-text embeddings and enables zero-shot hazard detection using cosine similarity |

---

## Methodology  

### Data Preparation  
- Construction site images collected from OSHA prevention videos  
- Images preprocessed using CLIP pipeline  
- Hazard descriptions created based on OSHA safety guidelines  

### Model Setup  
- Load pretrained CLIP model  
- Encode:
  - Images → visual embeddings  
  - Text → language embeddings  
- Map into a shared embedding space  

### Zero-Shot Hazard Detection  
- Compute cosine similarity between image and text embeddings  
- Rank hazard descriptions  
- Assign top matching hazard labels  

### Evaluation  
- Inspection-based human evaluation  
- Metrics:
  - Precision  
  - Recall  
  - F1 Score  

---

## Repository Structure  
```
Hazard_Detection_CLIP_Zero-Shot/
├── data/
├── scripts/
├── utils/
├── results/
├── requirements.txt
└── README.md
```

## Key Results
- 70% accuracy on preliminary dataset
- Correct hazard identified in most images
- Strong performance on visually distinct hazards
- Challenges with ambiguous or overlapping hazard types

## Citation
@incollection{samsami2025automated,
  title={Automated Hazard Detection on Construction Sites Using Contrastive Language--Image Pre-Training (CLIP): A Zero-Shot Learning Approach with Human-Centric Evaluation},
  author={Samsami, Reihaneh and Bahdan, Sharmin},
  booktitle={Computing in Civil Engineering 2025: Computational and Intelligent Technologies},
  pages={538--542}
}
## Publication

Samsami, Reihaneh, and Sharmin Badhan. "Automated Hazard Detection on Construction Sites Using Contrastive Language–Image Pre-Training (CLIP): A Zero-Shot Learning Approach with Human-Centric Evaluation." Computing in Civil Engineering 2025: Computational and Intelligent Technologies. 2025. 538-542.
- [Read the full paper](https://ascelibrary.org/doi/abs/10.1061/9780784486436.057)

## Authors
- Sharmin Jahan Badhan
- Reihaneh Samsami
