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

## Weakly-supervised

## Other-Modality

## LLMs-based

