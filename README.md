# M3: A Multi-Image Multi-Modal Entity Alignment Dataset
![](https://img.shields.io/badge/version-1.0.1-blue)

>Multi-modal Entity Alignment (MMEA) aims to identify the equivalent entities in different multi-modal knowledge graphs (MMKGs), thereby facilitating the integration of multiple MMKGs and enhancing the coverage of MMKGs. However, a prominent issue is the lack of publicly available datasets and evaluation benchmarks. Existing MMEA datasets have low entity coverage, single image, high inter-image correlation, and the images are derived from a single knowledge base, which cannot mirror the real-life challenges. This limitation hinders the validation of MMEA methods in real-world settings.
To address this problem, in this work, we first construct M3, an MMEA benchmark equipped with multiple images in real-world scenarios. Additionally, we design a universal multi-image processing module (AMIA) that assigns different levels of attention weights to images associated with entities, thus effectively modeling the visual information. The experimental results validate the difficulty and effectiveness of M3, as well as the effectiveness of AMIA. Our work will be publicly available on the GitHub data repository upon acceptance.


## 📚 Dataset

>M3, an MMEA benchmark equipped with multiple images retrieved from respective search engines, which better mirrors real-life challenges. We utilize the widely used DBP15K dataset as the foundational dataset, which includes three cross-ingual datasets: Chinese-English, Japanese-English, and French-English.

>Our M3  VS the existing MMEA benchmarks. 

| Benchmarks                        | KGs         |  #Ent. |  #Rel. | #EA pairs | Coverage | Similarity |  SSIM  |
| --------------------------------- | ----------- | -------| ------ | --------- | -------- |  --------  | -----  | 
| MMKG                              | FB15K       | 14951  |  1345  |    --     |   89.9%  |            |        |
|                                   | DB15K       | 14777  |  279   |   12846   |   86.9%  |            |        |
|                                   | YAGO15K     | 15283  |  32    |   11199   |   73.2%  |            |        |
| EVA-Dataset                       |   ZH        | 19388  |  1701  |   15000   |   82.1%  |   83.0%    | 0.5721 |
|                                   |   EN        | 19572  |  1323  |           |   72.2%  |            |        |
|                                   |   JA        | 19814  |  1299  |   15000   |   64.3%  |   83.9%    | 0.6041 |
|                                   |   EN        | 19780  |  1153  |           |   69.5%  |            |        |
|                                   |   FR        | 19661  |  903   |   15000   |   72.1%  |   84.8%    | 0.6160 |
|                                   |   EN        | 19993  |  1208  |           |   69.3%  |            |        |
| EVA-Dataset                       |  EN15K(V1)  | 19388  |  267   |   15000   |   99.7%  |   75.7%    |        |
|                                   |  FR15K(V1)  | 19572  |  210   |           |   94.5%  |            |        |
|                                   |  EN100K(V1) | 19814  |  400   |   100000  |   99.6%  |   75.1%    |        |
|                                   |  FR100K(V1) | 19780  |  300   |           |   94.1%  |            |        |
| M3                                |   ZH        | 19388  |  1701  |   15000   |   98.9%  |   64.8%    | 0.2592 |
|                                   |   EN        | 19572  |  1323  |           |   99.9%  |            |        |
|                                   |   JA        | 19814  |  1299  |   15000   |   100.0% |   63.4%    | 0.1722 |
|                                   |   EN        | 19780  |  1153  |           |   100.0% |            |        |
|                                   |   FR        | 19661  |  903   |   15000   |   99.9%  |   69.8%    | 0.1880 |
|                                   |   EN        | 19993  |  1208  |           |   99.9%  |            |        |

❗NOTE: After the paper is published, we will provide details of the dataset implementation, image embedding files, and detailed code information. For now, we are presenting some of the original image information from the dataset, which can be downloaded from [`Baidu Cloud Drive`](https://pan.baidu.com/s/1BRX9qvS2bVdpS5--NEEF9A) with the pass code **`mmm3`**. We use ResNet-152 to obtain embeddings of the original images. The embedding files can be downloaded from [`Baidu Cloud Drive`](https://pan.baidu.com/s/1A7NGiwc_HMHy_1FqEDYMhw) with the pass code **`embb`**.
