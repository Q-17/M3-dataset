# M3: A Multi-Image Multi-Modal Entity Alignment Dataset
![](https://img.shields.io/badge/version-1.0.0-blue)

>Multi-modal Entity Alignment (MMEA) aims to identify equivalent entities across different multi-modal knowledge graphs (MMKGs), facilitating their integration and enhancing coverage. However, current MMEA datasets have limitations, including low entity coverage, a single image per entity, high inter-image correlation, and reliance on a single search engine, which do not reflect real-world challenges. These oversimplified scenarios may impede the fair comparison and development of the alignment solutions. To address this problem, in this work, we first construct M3, an MMEA benchmark equipped with multiple images from different data sources in real-world scenarios. Additionally, we design a simple and universal multi-image processing module (AMIA), which assigns varying attention weights to images associated with entities to effectively model visual information. Experimental results validate the difficulty of M3, as well as the effectiveness of AMIA. Despite the superior performance of AMIA, there is still room for developing more advanced solutions to address these difficulties. Our code will be released after acceptance.


## 📚 Dataset

>M3, an MMEA benchmark equipped with multiple images retrieved from respective search engines, which better mirrors real-life challenges. We utilize the widely used DBP15K dataset as the foundational dataset, which includes three cross-ingual datasets: Chinese-English, Japanese-English, and French-English.

>Our M3  VS the existing MMEA benchmarks. 

| Benchmarks                        | KGs         |  #Ent. |  #Rel. | #EA pairs | Coverage | Similarity |  SSIM  |
| --------------------------------- | ----------- | -------| ------ | --------- | -------- |  --------  | -----  | 
| MMKG                              | FB15K       | 14951  |  1345  |           |   89.9%  |            |        |
|                                   | DB15K       | 14777  |  279   |   12846   |   86.9%  |            |        |
|                                   | YAGO15K     | 15283  |  32    |   11199   |   73.2%  |            |        |
| EVA-Dataset                       |   ZH        | 19388  |  1701  |   15000   |   82.1%  |   0.830    | 0.5721 |
|                                   |   EN        | 19572  |  1323  |           |   72.2%  |            |        |
|                                   |   JA        | 19814  |  1299  |   15000   |   64.3%  |   0.839    | 0.6041 |
|                                   |   EN        | 19780  |  1153  |           |   69.5%  |            |        |
|                                   |   FR        | 19661  |  903   |   15000   |   72.1%  |   0.848    | 0.6160 |
|                                   |   EN        | 19993  |  1208  |           |   69.3%  |            |        |
| Multi-OpenEA                      |  EN15K(V1)  | 15000  |  267   |   15000   |   99.7%  |   0.757    | 0.3338 |
|                                   |  FR15K(V1)  | 15000  |  210   |           |   94.5%  |            |        |
|                                   |  DBP15K(V1) | 15000  |  248   |   15000   |   99.8%  |   0.829    |        |
|                                   |  WD15K(V1)  | 15000  |  169   |           |   99.8%  |            |        |
| M3                                |   ZH        | 19388  |  1701  |   15000   |   98.9%  |   0.648    | 0.2592 |
|                                   |   EN        | 19572  |  1323  |           |   99.9%  |            |        |
|                                   |   JA        | 19814  |  1299  |   15000   |   100.0% |   0.634    | 0.1722 |
|                                   |   EN        | 19780  |  1153  |           |   100.0% |            |        |
|                                   |   FR        | 19661  |  903   |   15000   |   99.9%  |   0.698    | 0.1880 |
|                                   |   EN        | 19993  |  1208  |           |   99.9%  |            |        |

❗NOTE: After the paper is published, we will provide details of the dataset implementation, image embedding files, and detailed code information. For now, we are presenting some of the original image information from the dataset, which can be downloaded from [`Baidu Cloud Drive`](https://pan.baidu.com/s/1BRX9qvS2bVdpS5--NEEF9A) with the pass code **`mmm3`**. We use ResNet-152 to obtain embeddings of the original images. The embedding files can be downloaded from [`Baidu Cloud Drive`](https://pan.baidu.com/s/1A7NGiwc_HMHy_1FqEDYMhw) with the pass code **`embb`**.
