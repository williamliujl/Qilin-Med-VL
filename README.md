# Qilin-Med-VL: Towards Chinese Large Vision-Language Model for General Healthcare

> Junling Liu, Ziming Wang, Qichen Ye, Dading Chong, Peilin Zhou, Yining Hua

## 📖 Introduction
Large Language Models (LLMs) have introduced a new era of proficiency in comprehending complex healthcare and biomedical topics. However, there is a noticeable lack of models in languages other than English and models that can interpret multi-modal input, which is crucial for global healthcare accessibility. In response, this study introduces Qilin-Med-VL 1 , the first Chinese large vision-language model designed to integrate the analysis of textual and visual data. Qilin-Med-VL combines a pre-trained Vision Transformer (ViT) with a foundational LLM. It undergoes a thorough two-stage curriculum training process that includes feature alignment and instruction tuning. This method enhances the model's ability to generate medical captions and answer complex medical queries. We also release ChiMed-VL, a dataset consisting of more than 1M image-text pairs. This dataset has been carefully curated to enable detailed and comprehensive interpretation of medical data using various types of images.

![overview](docs/flowchart.png)


## ✅ Todo

- [x] training scripts
- [x] training data
- [x] models
- [ ] downstream task validation

## 📚 Datasets

Chinese Medicine - Vision Language Dataset (ChiMed-VL), the first large-scale Chinese Vision-Language dataset for general healthcare, designed to facilitate multistage training. This dataset has two subsets: vision-language feature alignment and instruction tuning.

### ChiMed-VL-Alignment dataset
ChiMed-VL-Alignment consists of 580,014 image-text couplings, each pair falling into one of two categories: context information of an image or descriptions of an image. The context category contains 167M tokens, presenting a median text length of 435 (Q1: 211, Q3: 757). Conversely, descriptions, more concise and image-specific, contain inline descriptions and captions. They comprise 63M tokens, with median lengths settling at 59 (Q1: 45, Q3: 83).

### ChiMed-VL-Instruction dataset
ChiMed-VL-Instruction comprises 469,441 question-answer pairs. Within this subset, the questions section contains 10M tokens with a median length of 20 (Q1: 16, Q3: 25), posing a concise inquiry reflective of medical queries. The answers consist of 13M tokens with a median length slightly longer at 22 (Q1: 12, Q3: 34), providing clear, direct, and informative responses.

### Data Acquire
Our prompt data is provided on HuggingFace and Baidu Yun.

- HuggingFace: https://huggingface.co/datasets/williamliu/ChiMed-VL

- Baidu Yun: https://pan.baidu.com/s/1TBwdKLZbaYIxZy_DLMZrXQ 提取码: fkma

## 👨‍ Models

### Model Access
We have open-sourced the weights of the Qilin-Med-VL model, which can be downloaded through the following link.
- HuggingFace: https://huggingface.co/williamliu/Qilin-Med-VL

- Baidu Yun: https://pan.baidu.com/s/1lZs53EWb9kOtsIN5BB34Jw 提取码: muab 


## Cite Us
```
@inproceedings{Liu2023QilinMedVLTC,
  title={Qilin-Med-VL: Towards Chinese Large Vision-Language Model for General Healthcare},
  author={Junling Liu and Ziming Wang and Qichen Ye and Dading Chong and Peilin Zhou and Yining Hua},
  year={2023},
  url={https://arxiv.org/abs/2310.17956}
}
```


## Acknowledgement

Many thanks to the following awesome works!

- [LLaVA](https://github.com/haotian-liu/LLaVA)
- [Transformers](https://github.com/huggingface/transformers)
