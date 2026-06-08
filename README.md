# Beyond Universality: The GCC-FER Dataset and Culture-Aware Adaptation

## 📌 Overview
Dynamic Facial Expression Recognition (DFER) systems often assume that emotional expressions are universally consistent across populations. However, systematic variability in facial muscle activation patterns across cultures significantly influences cross-cultural performance. To address this limitation, we propose a Culture-Aware Facial Expression Recognition (CA-FER) system designed to mitigate cultural bias by adaptively recalibrating latent facial representations.

## 📊 The GCC-FER Dataset
To overcome the scarcity of culturally diverse benchmark datasets, we introduce the Global Cross-Cultural Facial Expression Recognition (GCC-FER) dataset. 
* It is a large-scale, hybrid multicultural video dataset.
* The dataset comprises a total of 23,934 video samples.
* The video samples span four major cultural groups: African, Caucasian, East Asian, and South Asian.
* The dataset covers seven basic facial expression categories: Angry, Disgust, Fear, Happy, Neutral, Sad, and Surprise.
* **Note on DFEW subset:** For the video samples adopted from the DFEW dataset, the corresponding ethnicity annotations will be provided as a separate JSON file (video samples will not be provided).

## 🛠️ Methodology (CA-FER)
The proposed Culture-Aware Facial Expression Recognition (CA-FER) framework operates in two main stages:
* The system first derives behaviorally grounded cultural priors.
* Next, these learned behavioral priors are used to adapt latent spatio-temporal representations extracted by a Video Vision Transformer (ViViT) backbone.
* In the absence of explicit cultural labels during practical deployment, the system can utilize a global AU-grounded cultural prior.

## 📈 Performance Results
Extensive cross-cultural experiments demonstrate the effectiveness of the proposed system:
* On the newly introduced GCC-FER dataset, the CA-FER system achieves 61.70% Unweighted Average Recall (UAR) and 64.80% Weighted Average Recall (WAR).
* On the publicly available DFEW benchmark dataset, the system achieves 63.93% UAR, which outperforms state-of-the-art non-pretrained method.

## 📝 Citation
If you utilize the GCC-FER dataset or the CA-FER system in your research, please consider citing our work:

```bibtex
@misc{singh2026universalitygccferdatasetcultureaware,
      title={Beyond Universality: The GCC-FER Dataset and Culture-Aware Adaptation for Dynamic Facial Expression Recognition}, 
      author={Sonalika Singh and Jyotirindra Dandapat and Avishi Razdan and Kshipra V. Moghe and Puneet Gupta and Lalan Kumar},
      year={2026},
      eprint={2606.07063},
      archivePrefix={arXiv},
      primaryClass={eess.IV},
      url={https://arxiv.org/abs/2606.07063}, 
}
