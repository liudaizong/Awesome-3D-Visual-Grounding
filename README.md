# Awesome-3D-Visual-Grounding [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)
A **continual** collection of papers related to Text-guided 3D Visual Grounding (T-3DVG).

Text-guided 3D visual grounding (T-3DVG) aims to locate a specific object that semantically corresponds to a language query from a complicated 3D scene, has drawn increasing attention in the 3D research community over the past few years.
T-3DVG presents great potential and challenges due to its closer proximity to the real world and the complexity of data collection and 3D point cloud source processing.

In the T-3DVG community, we've summarized existing T-3DVG methods in our survey paper👍.


> If you find some important work missed, it would be super helpful to let me know (`dzliu@stu.pku.edu.cn`). Thanks!

> If you find our survey useful for your research, please consider citing:

```
@article{liu2024survey,
  title={A Survey on Text-guided 3D Visual Grounding: Elements, Recent Advances, and Future Directions},
  author={Liu, Daizong and Liu, Yang and Huang, Wencan and Hu, Wei},
  journal={arXiv preprint arXiv},
  year={2024}
}
```

**Table of Contents**
- [Fully-supervised approach](#Fully-supervised)
- [Weakly-supervised approach](#Weakly-supervised)
- [Approaches using No Point Cloud Input](#Other-Modality)
- [Approaches using LLMs](#LLMs-based)
---

## Fully-supervised
* **ScanRefer: 3D Object Localization in RGB-D Scans using Natural Language** | [Github](https://github.com/daveredrum/ScanRefer)
  * Dave Zhenyu Chen, Angel X. Chang, Matthias Nießner
  * Technical University of Munich, Simon Fraser University
  * [ECCV2020] https://arxiv.org/abs/1912.08830
  * A dataset, two-stage approach, proposal-then-selection
* **ReferIt3D: Neural Listeners for Fine-Grained 3D Object Identification in Real-World Scenes** | [Github](https://github.com/referit3d/referit3d)
  * Panos Achlioptas, Ahmed Abdelreheem, Fei Xia, Mohamed Elhoseiny, Leonidas Guibas
  * Stanford University, King Abdullah University of Science and Technology
  * [ECCV2020] https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123460409.pdf
  * A dataset, two-stage approach, proposal-then-selection
* **Free-form Description Guided 3D Visual Graph Network for Object Grounding in Point Cloud** | [Github](https://github.com/PNXD/FFL-3DOG)
  * Mingtao Feng, Zhen Li, Qi Li, Liang Zhang, XiangDong Zhang, Guangming Zhu, Hui Zhang, Yaonan Wang, Ajmal Mian
  * Xidian University, Hunan University, The University of Western Australia
  * [ICCV2021] https://openaccess.thecvf.com/content/ICCV2021/papers/Feng_Free-Form_Description_Guided_3D_Visual_Graph_Network_for_Object_Grounding_ICCV_2021_paper.pdf
  * Two-stage approach, proposal-then-selection, graph neural network
* **InstanceRefer: Cooperative Holistic Understanding for Visual Grounding on Point Clouds through Instance Multi-level Contextual Referring** | [Github](https://github.com/CurryYuan/InstanceRefer)
  * Zhihao Yuan, Xu Yan, Yinghong Liao, Ruimao Zhang, Sheng Wang, Zhen Li, Shuguang Cui
  * The Chinese University of Hong Kong (Shenzhen), Southern University of Science and Technology
  * [ICCV2021] https://openaccess.thecvf.com/content/ICCV2021/papers/Yuan_InstanceRefer_Cooperative_Holistic_Understanding_for_Visual_Grounding_on_Point_Clouds_ICCV_2021_paper.pdf
  * Two-stage approach, proposal-then-selection, segmentation
* **Text-Guided Graph Neural Networks for Referring 3D Instance Segmentation** | [Github](https://github.com/hanhung/TGNN)
  * Pin-Hao Huang, Han-Hung Lee, Hwann-Tzong Chen, Tyng-Luh Liu
  * Academia Sinica, National Tsing Hua University, Taiwan AI Labs, Aeolus Robotics
  * [AAAI2021] https://ojs.aaai.org/index.php/AAAI/article/view/16253
  * Two-stage approach, proposal-then-selection, segmentation
* **LanguageRefer: Spatial-Language Model for 3D Visual Grounding** | [Github](https://github.com/rohjunha/language-refer)
  * Junha Roh, Karthik Desingh, Ali Farhadi, Dieter Fox
  * University of Washington
  * [CoRL2021] https://openreview.net/pdf?id=dgQdvPZnH-t
  * Two-stage approach, proposal-then-selection, spatial embedding, positional encoding
* **TransRefer3D: Entity-and-Relation Aware Transformer for Fine-Grained 3D Visual Grounding** | [Github](https://github.com/luo-junyu/TransRefer3D)
  * Dailan He, Yusheng Zhao, Junyu Luo, Tianrui Hui, Shaofei Huang, Aixi Zhang, Si Liu
  * Beihang University, Chinese Academy of Sciences, Alibaba Group
  * [ACMMM2021] https://arxiv.org/abs/2108.02388
  * Two-stage approach, proposal-then-selection, entity-and-relation
* **3DJCG: A Unified Framework for Joint Dense Captioning and Visual Grounding on 3D Point Clouds** | [Github](https://github.com/zlccccc/3DVL_Codebase)
  * Daigang Cai, Lichen Zhao, Jing Zhang, Lu Sheng, Dong Xu
  * Beihang University, The University of Sydney
  * [CVPR2022] https://openaccess.thecvf.com/content/CVPR2022/papers/Cai_3DJCG_A_Unified_Framework_for_Joint_Dense_Captioning_and_Visual_CVPR_2022_paper.pdf
  * Two-stage approach, proposal-then-selection, joint 3D captioning and grounding 
* **3DRefTransformer: Fine-Grained Object Identification in Real-World Scenes Using Natural Language** | 
  * Ahmed Abdelreheem, Ujjwal Upadhyay, Ivan Skorokhodov, Rawan Al Yahya, Jun Chen, Mohamed Elhoseiny
  * King Abdullah University of Science and Technology
  * [WACV2022] https://openaccess.thecvf.com/content/WACV2022/papers/Abdelreheem_3DRefTransformer_Fine-Grained_Object_Identification_in_Real-World_Scenes_Using_Natural_Language_WACV_2022_paper.pdf
  * Two-stage approach, proposal-then-selection
* **D3Net: A Unified Speaker-Listener Architecture for 3D Dense Captioning and Visual Grounding** | [Github](https://github.com/daveredrum/D3Net)
  * Dave Zhenyu Chen, Qirui Wu, Matthias Nießner, Angel X. Chang
  * Technical University of Munich, Simon Fraser University
  * [ECCV2022] https://arxiv.org/abs/2112.01551
  * Two-stage approach, proposal-then-selection, joint 3D captioning and grounding 
* **Language Conditioned Spatial Relation Reasoning for 3D Object Grounding** | [Github](https://github.com/cshizhe/vil3dref)
  * Shizhe Chen, Pierre-Louis Guhur, Makarand Tapaswi, Cordelia Schmid, Ivan Laptev
  * PSL Research University, IIIT Hyderabad
  * [NeurIPS2022] https://arxiv.org/abs/2211.09646
  * Two-stage approach, proposal-then-selection, spatial relation 
* **3D-VisTA: Pre-trained Transformer for 3D Vision and Text Alignment** | [Github](https://github.com/3d-vista/3D-VisTA)
  * Ziyu Zhu, Xiaojian Ma, Yixin Chen, Zhidong Deng, Siyuan Huang, Qing Li
  * Tsinghua University, BIGAI
  * [ICCV2023] https://arxiv.org/pdf/2308.04352
  * Two-stage approach, proposal-then-selection, pre-training 
* **3D-VisTA: Pre-trained Transformer for 3D Vision and Text Alignment** | [Github](https://github.com/3d-vista/3D-VisTA)
  * Ziyu Zhu, Xiaojian Ma, Yixin Chen, Zhidong Deng, Siyuan Huang, Qing Li
  * Tsinghua University, BIGAI
  * [ICCV2023] https://arxiv.org/pdf/2308.04352
  * Two-stage approach, proposal-then-selection, pre-training 


## Weakly-supervised

## Other-Modality

## LLMs-based

