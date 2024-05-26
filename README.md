# M3: A Multi-Image Multi-Modal Entity Alignment Dataset
![](https://img.shields.io/badge/version-1.0.1-blue)

>Multi-modal Entity Alignment (MMEA) aims to identify the equivalent entities in different multi-modal knowledge graphs (MMKGs), thereby facilitating the integration of multiple MMKGs and enhancing the coverage of MMKGs. However, a prominent issue is the lack of publicly available datasets and evaluation benchmarks. Existing MMEA datasets have low entity coverage, single image, high inter-image correlation, and the images are derived from a single knowledge base, which cannot mirror the real-life challenges. This limitation hinders the validation of MMEA methods in real-world settings.
To address this problem, in this work, we first construct M3, an MMEA benchmark equipped with multiple images in real-world scenarios. Additionally, we design a universal multi-image processing module (AMIA) that assigns different levels of attention weights to images associated with entities, thus effectively modeling the visual information. The experimental results validate the difficulty and effectiveness of M3, as well as the effectiveness of AMIA. Our work will be publicly available on the GitHub data repository upon acceptance.


## 📚 Dataset

>M3, an MMEA benchmark equipped with multiple images retrieved from respective search engines, which better mirrors real-life challenges. We utilize the widely used DBP15K dataset as the foundational dataset, which includes three cross-ingual datasets: Chinese-English, Japanese-English, and French-English.

>Our M3 benchmarks vs the existing MMEA benchmarks. 



❗NOTE: After the paper is published, we will provide details of the dataset implementation, image embedding files, and detailed code information. For now, we are presenting some of the original image information from the dataset, which can be downloaded from [`Baidu Cloud Drive`](https://pan.baidu.com/s/1BRX9qvS2bVdpS5--NEEF9A) with the pass code **`mmm3`**. We use ResNet-152 to obtain embeddings of the original images. The embedding files can be downloaded from [`Baidu Cloud Drive`](https://pan.baidu.com/s/1BRX9qvS2bVdpS5--NEEF9A) with the pass code **`embb`**.
