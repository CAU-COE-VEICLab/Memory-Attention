# Memory-Attention
This is the code base for **`"Enhancing your attention to memorize more information for multimodal medical image segmentation"`**, and the article is submitted to **`Information Fusion`**.

## Abstract
In this work, we first summarize the particular challenges of the medical image segmentation task. Secondly, summarize how deep neural network models can cope with that challenge. Finally, we give an effective solution.
The main research contents of this paper are as follows:

(i) `Inspired by WCWMM`, we propose a `human-like memory and action method` called **`Memory-Attention Mechanism (MAM)`** for the first time, using **`abstract cognitive-behavioral theories`** as the guiding idea for model design and introducing the concept of **`working memory`** into deep learning for the first time. **`see Fig1`**. 

![MAM model](pic/model.png)

(ii) MAM mimics the `human visual cognitive system at the functional level` and realizes **`the efficient coupling of the ability to extract local detailed features and establish global information dependencies in computational theory`**, thus improving the performance of multimodal medical image segmentation models. Furthermore, `incorporating memory allows` **`MAM to creatively express long-distance dependencies at the pixel level between distinct layers throughout time (see Fig2)`**.

![dependency](pic/dependency.png)

(iii) `Attention in MAM is obtained through` **`the comprehensive integration and analysis of the memory of all previous network layers with the information of the current layer`**. Thus, MAM can compensate for the precise information that may be overlooked `when building long-distance dependencies through memory recall and retrieval`. Furthermore, MAM is **`exceedingly topological`**, allowing for the seamless replacement of the Self-Attention Mechanism (SAM) in SAM-based models and **`using SAM's pre-training weights`**, effectively mitigating the issues caused by **`computational resources and model migration`**.

(iv) To adapt the Sequential Architecture and the Hierarchical Architecture Transformers, we propose the **`Sequential Transmission Strategy (STS)`**, which emphasizes memory sharing and integration, and the **`In-Stage Transmission Strategy (ISTS)`**, which emphasizes specialized processing of memories of different dimensions, respectively. It is worth noting that `ISTS` uses **`a divide-and-conquer strategy`** `that is more in line with the information-processing mechanism of the human brain.` **`see Fig3`**.

![STSandISTS](pic/STSandISTS.png)

(v) To validate the state-of-the-art of MAM, we built hybrid and pure Transformer architecture models based on MAM, and we ran controlled tests on **`2D and 3D medical image datasets`** from various modalities. Finally, we conducted a detailed ablation investigation on each important memory concept MAM gave to verify its **`scientific validity`** properly. see Tables 1 to 5.

## Results
**To learn more detail please read our paper**.
### Comparison experiments
The quantitative comparison between models that have been applied more frequently in agricultural semantic segmentation and the proposed model.

