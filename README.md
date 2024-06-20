# Awesome-3D-Visual-Grounding [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)
A **continual** collection of papers related to Text-guided 3D Visual Grounding (T-3DVG).

Text-guided 3D visual grounding (T-3DVG) aims to locate a specific object that semantically corresponds to a language query from a complicated 3D scene, has drawn increasing attention in the 3D research community over the past few years.
T-3DVG presents great potential and challenges due to its closer proximity to the real world and the complexity of data collection and 3D point cloud source processing.

In the T-3DVG community, we've summarized existing T-3DVG methods in our survey paper👍.

[A Survey on Text-guided 3D Visual Grounding: Elements, Recent Advances, and Future Directions](https://arxiv.org/abs/2406.05785).


> If you find some important work missed, it would be super helpful to let me know (`dzliu@stu.pku.edu.cn`). Thanks!

> If you find our survey useful for your research, please consider citing:

```
@article{liu2024survey,
  title={A Survey on Text-guided 3D Visual Grounding: Elements, Recent Advances, and Future Directions},
  author={Liu, Daizong and Liu, Yang and Huang, Wencan and Hu, Wei},
  journal={arXiv preprint arXiv:2406.05785},
  year={2024}
}
```

**Table of Contents**
- [Fully-supervised two-stage approach](#Fully-Supervised-Two-Stage)
- [Fully-supervised one-stage approach](#Fully-Supervised-One-Stage)
- [Weakly-supervised approach](#Weakly-supervised)
- [Approaches using No Point Cloud Input](#Other-Modality)
- [Approaches using LLMs](#LLMs-based)
- [Approaches tackling Outdoor Scenes](#Outdoor-Scenes)
---

## Fully-Supervised-Two-Stage
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
* **SAT: 2D Semantics Assisted Training for 3D Visual Grounding** | [Github](https://github.com/zyang-ur/SAT)
  * Zhengyuan Yang, Songyang Zhang, Liwei Wang, Jiebo Luo
  * University of Rochester, The Chinese University of Hong Kong
  * [ICCV2021] https://arxiv.org/pdf/2105.11450
  * Two-stage approach, proposal-then-selection, additional multi-modal input
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
* **Multi-View Transformer for 3D Visual Grounding** | [Github](https://github.com/sega-hsj/MVT-3DVG)
  * Shijia Huang, Yilun Chen, Jiaya Jia, Liwei Wang
  * The Chinese University of Hong Kong
  * [CVPR2022] https://openaccess.thecvf.com/content/CVPR2022/papers/Huang_Multi-View_Transformer_for_3D_Visual_Grounding_CVPR_2022_paper.pdf
  * Two-stage approach, proposal-then-selection, additional multi-view input 
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
* **Look Around and Refer: 2D Synthetic Semantics Knowledge Distillation for 3D Visual Grounding** | [Github](https://github.com/eslambakr/LAR-Look-Around-and-Refer)
  * Eslam Mohamed Bakr, Yasmeen Alsaedy, Mohamed Elhoseiny
  * King Abdullah University of Science and Technology
  * [NeurIPS2022] https://arxiv.org/abs/2211.14241
  * Two-stage approach, proposal-then-selection, additional multi-modal input
* **Context-aware Alignment and Mutual Masking for 3D-Language Pre-training** | [Github](https://github.com/leolyj/3D-VLP)
  * Zhao Jin, Munawar Hayat, Yuwei Yang, Yulan Guo, Yinjie Lei
  * Sichuan University, Monash University, Sun Yat-sen University
  * [CVPR2023] https://openaccess.thecvf.com/content/CVPR2023/papers/Jin_Context-Aware_Alignment_and_Mutual_Masking_for_3D-Language_Pre-Training_CVPR_2023_paper.pdf
  * Two-stage approach, proposal-then-selection, pre-training
* **NS3D: Neuro-Symbolic Grounding of 3D Objects and Relations** | [Github](https://github.com/joyhsu0504/NS3D)
  * Joy Hsu, Jiayuan Mao, Jiajun Wu
  * Stanford University, Massachusetts Institute of Technology
  * [CVPR2023] https://arxiv.org/abs/2303.13483
  * Two-stage approach, proposal-then-selection, semantic learning
* **3D-VisTA: Pre-trained Transformer for 3D Vision and Text Alignment** | [Github](https://github.com/3d-vista/3D-VisTA)
  * Ziyu Zhu, Xiaojian Ma, Yixin Chen, Zhidong Deng, Siyuan Huang, Qing Li
  * Tsinghua University, BIGAI
  * [ICCV2023] https://arxiv.org/pdf/2308.04352
  * Two-stage approach, proposal-then-selection, pre-training
* **Multi3DRefer: Grounding Text Description to Multiple 3D Objects** | [Github](https://github.com/3dlg-hcvc/M3DRef-CLIP)
  * Yiming Zhang, ZeMing Gong, Angel X. Chang
  * Simon Fraser University, Alberta Machine Intelligence Institute
  * [ICCV2023] https://3dlg-hcvc.github.io/multi3drefer/
  * A dataset, Two-stage approach, proposal-then-selection, multiple-object grounding
* **UniT3D: A Unified Transformer for 3D Dense Captioning and Visual Grounding** | 
  * Dave Zhenyu Chen, Ronghang Hu, Xinlei Chen, Matthias Nießner, Angel X. Chang
  * Technical University of Munich, Meta AI, Simon Fraser University
  * [ICCV2023] https://arxiv.org/abs/2212.00836
  * Two-stage approach, proposal-then-selection, joint 3D captioning and grounding
* **ViewRefer: Grasp the Multi-view Knowledge for 3D Visual Grounding with GPT and Prototype Guidance** | [Github](https://github.com/Ivan-Tang-3D/ViewRefer3D)
  * Zoey Guo, Yiwen Tang, Ray Zhang, Dong Wang, Zhigang Wang, Bin Zhao, Xuelong Li
  * Shanghai Artificial Intelligence Laboratory, The Chinese University of Hong Kong, Northwestern Polytechnical University
  * [ICCV2023] https://arxiv.org/pdf/2303.16894
  * Two-stage approach, proposal-then-selection, additional multi-view input
* **ARKitSceneRefer: Text-based Localization of Small Objects in Diverse Real-World 3D Indoor Scenes** | [Github](https://github.com/ku-nlp/ARKitSceneRefer)
  * Shunya Kato, Shuhei Kurita, Chenhui Chu, Sadao Kurohashi
  * Kyoto University, RIKEN
  * [EMNLP2023] https://aclanthology.org/2023.findings-emnlp.56.pdf
  * A dataset, Two-stage approach, proposal-then-selection, small object
* **Reimagining 3D Visual Grounding: Instance Segmentation and Transformers for Fragmented Point Cloud Scenarios** | 
  * Zehan Tan, Weidong Yang, Zhiwei Wang
  * Fudan University, GREE ELECTRIC APPLIANCES
  * [ACMMMAsia2023] https://dl.acm.org/doi/10.1145/3595916.3626405
  * Two-stage approach, proposal-then-selection, additional multi-modal input
* **HAM: Hierarchical Attention Model with High Performance for 3D Visual Grounding** | 
  * Jiaming Chen, Weixin Luo, Xiaolin Wei, Lin Ma, and Wei Zhang
  * Shandong University, Meituan
  * [Arxiv2023] https://arxiv.org/abs/2210.12513
  * One-stage approach, proposal-then-selection, point detection
* **Three Ways to Improve Verbo-visual Fusion for Dense 3D Visual Grounding** | 
  * Ozan Unal, Christos Sakaridis, Suman Saha, Fisher Yu, Luc Van Gool
  * ETH Zurich
  * [Arxiv2023] https://arxiv.org/abs/2309.04561
  * Two-stage approach, proposal-then-selection, segmentation
* **ScanERU: Interactive 3D Visual Grounding based on Embodied Reference Understanding** | 
  * Ziyang Lu, Yunqiang Pei, Guoqing Wang, Yang Yang, Zheng Wang, Heng Tao Shen
  * University of Electronic Science and Technology of China
  * [Arxiv2023] https://arxiv.org/abs/2303.13186
  * Two-stage approach, proposal-then-selection, additional multi-modal input
* **ScanEnts3D: Exploiting Phrase-to-3D-Object Correspondences for Improved Visio-Linguistic Models in 3D Scenes** | [Github](https://github.com/ScanEnts3D/ScanEnts3D.github.io)
  * Ahmed Abdelreheem, Kyle Olszewski, Hsin-Ying Lee, Peter Wonka, Panos Achlioptas
  * King Abdullah University of Science and Technology, Snap Inc.
  * [WACV2024] https://openaccess.thecvf.com/content/WACV2024/papers/Abdelreheem_ScanEnts3D_Exploiting_Phrase-to-3D-Object_Correspondences_for_Improved_Visio-Linguistic_Models_in_3D_WACV_2024_paper.pdf
  * Two-stage approach, proposal-then-selection
* **COT3DREF: Chain-of-Thoughts Data-Efficeint 3D Visual Grounding** | [Github](https://github.com/CoT3DRef/COT3DRef)
  * Eslam Mohamed Bakr, Mohamed Ayman, Mahmoud Ahmed, Habib Slim, Mohamed Elhoseiny
  * King Abdullah University of Science and Technology
  * [ICLR2024] https://arxiv.org/abs/2310.06214
  * Two-stage approach, proposal-then-selection, Chain-of-Thoughts 
* **Exploiting Contextual Objects and Relations for 3D Visual Grounding** | [Github](https://github.com/yangli18/CORE-3DVG)
  * Li Yang, Chunfeng Yuan, Ziqi Zhang, Zhongang Qi, Yan Xu, Wei Liu, Ying Shan, Bing Li, Weiping Yang, Peng Li, Yan Wang, Weiming Hu
  * CASIA, Tencent PCG, The Chinese University of Hong Kong, Ministry of Education, Alibaba Group, Zhejiang Linkheer Science And Technology Co., Ltd., University of Chinese Academy of Sciences, ShanghaiTech University
  * [NeurIPS2024] https://papers.nips.cc/paper_files/paper/2023/hash/9b91ee0da3bcd61905fcd89e770168fc-Abstract-Conference.html
  * Two-stage approach, proposal-then-selection
* **Cross3DVG: Cross-Dataset 3D Visual Grounding on Different RGB-D Scans** | [Github](https://github.com/ATR-DBI/Cross3DVG)
  * Taiki Miyanishi, Daichi Azuma, Shuhei Kurita, Motoaki Kawanabe
  * ATR, Kyoto University, RIKEN AIP
  * [3DV2024] https://arxiv.org/abs/2305.13876
  * Two-stage approach, proposal-then-selection, additional multi-modal input
* **A Transformer-based Framework for Visual Grounding on 3D Point Clouds** | 
  * Ali Solgi, Mehdi Ezoji
  * Babol Noshirvani University of Technology
  * [AISP2024] https://ieeexplore.ieee.org/abstract/document/10475280/
  * Two-stage approach, proposal-then-selection
* **MiKASA: Multi-Key-Anchor & Scene-Aware Transformer for 3D Visual Grounding** | 
  * Chun-Peng Chang, Shaoxiang Wang, Alain Pagani, Didier Stricker
  * DFKI Augmented Vision
  * [CVPR2024] https://arxiv.org/abs/2403.03077
  * Two-stage approach, proposal-then-selection, spatial relation
* **Towards CLIP-driven Language-free 3D Visual Grounding via 2D-3D Relational Enhancement and Consistency** | [Github](https://github.com/xibi777/3DLFVG)
  * Yuqi Zhang, Han Luo, Yinjie Lei
  * Sichuan University
  * [CVPR2024] https://openaccess.thecvf.com/content/CVPR2024/papers/Zhang_Towards_CLIP-driven_Language-free_3D_Visual_Grounding_via_2D-3D_Relational_Enhancement_CVPR_2024_paper.pdf
  * Two-stage approach, proposal-then-selection, additional multi-modal input
* **Multi-Attribute Interactions Matter for 3D Visual Grounding** | [Github](https://github.com/volcanoXC/MA2TransVG)
  * Can Xu, Yuehui Han, Rui Xu, Le Hui, Jin Xie, Jian Yang
  * Nanjing University of Science and Technology, Northwestern Polytechnical University, Nanjing University
  * [CVPR2024] https://openaccess.thecvf.com/content/CVPR2024/papers/Xu_Multi-Attribute_Interactions_Matter_for_3D_Visual_Grounding_CVPR_2024_paper.pdf
  * Two-stage approach, proposal-then-selection, additional multi-modal input
* **Viewpoint-Aware Visual Grounding in 3D Scenes** | 
  * Xiangxi Shi, Zhonghua Wu, Stefan Lee
  * Oregon State University, SenseTime Research
  * [CVPR2024] https://openaccess.thecvf.com/content/CVPR2024/papers/Shi_Viewpoint-Aware_Visual_Grounding_in_3D_Scenes_CVPR_2024_paper.pdf
  * Two-stage approach, proposal-then-selection, additional multi-modal input
* **SCENEVERSE: Scaling 3D Vision-Language Learning for Grounded Scene Understanding** | [Github](https://github.com/scene-verse/SceneVerse)
  * Baoxiong Jia , Yixin Chen , Huanyue Yu, Yan Wang, Xuesong Niu, Tengyu Liu, Qing Li, Siyuan Huang
  * Beijing Institute for General Artificial Intelligence
  * [Arxiv2024] https://arxiv.org/abs/2401.09340
  * A dataset, Two-stage approach, proposal-then-selection
* **SeCG: Semantic-Enhanced 3D Visual Grounding via Cross-modal Graph Attention** | [Github](https://github.com/onmyoji-xiao/3dvg_SeCG)
  * Feng Xiao, Hongbin Xu, Qiuxia Wu, Wenxiong Kang
  * South China University of Technology
  * [Arxiv2024] https://arxiv.org/abs/2403.08182
  * Two-stage approach, proposal-then-selection, additional multi-modal input
* **DOrA: 3D Visual Grounding with Order-Aware Referring** | 
  * Tung-Yu Wu, Sheng-Yu Huang, Yu-Chiang Frank Wang
  * National Taiwan University, NVIDIA
  * [Arxiv2024] https://arxiv.org/abs/2403.16539
  * Two-stage approach, proposal-then-selection, Chain-of-Thoughts
* **Dual Attribute-Spatial Relation Alignment for 3D Visual Grounding** | 
  * Yue Xu, Kaizhi Yang, Jiebo Luo, Xuejin Chen
  * University of Science and Technology of China, University of Rochester
  * [Arxiv2024] https://arxiv.org/abs/2406.08907
  * Two-stage approach, proposal-then-selection, spatial embedding

## Fully-Supervised-One-Stage
* **3DVG-Transformer: Relation Modeling for Visual Grounding on Point Clouds** | [Github](https://github.com/zlccccc/3DVG-Transformer)
  * Lichen Zhao, Daigang Cai, Lu Sheng, Dong Xu
  * Beihang University, The University of Sydney
  * [ICCV2021] https://openaccess.thecvf.com/content/ICCV2021/papers/Zhao_3DVG-Transformer_Relation_Modeling_for_Visual_Grounding_on_Point_Clouds_ICCV_2021_paper.pdf
  * One-stage approach, unified detection-interaction
* **3D-SPS: Single-Stage 3D Visual Grounding via Referred Point Progressive Selection** | [Github](https://github.com/fjhzhixi/3D-SPS)
  * Junyu Luo, Jiahui Fu, Xianghao Kong, Chen Gao, Haibing Ren, Hao Shen, Huaxia Xia, Si Liu
  * Beihang University, Meituan Inc.
  * [CVPR2022] https://openaccess.thecvf.com/content/CVPR2022/papers/Luo_3D-SPS_Single-Stage_3D_Visual_Grounding_via_Referred_Point_Progressive_Selection_CVPR_2022_paper.pdf
  * One-stage approach, regression-based
* **Bottom Up Top Down Detection Transformers for Language Grounding in Images and Point Clouds** | [Github](https://github.com/nickgkan/butd_detr)
  * Ayush Jain, Nikolaos Gkanatsios, Ishita Mediratta, Katerina Fragkiadaki
  * Carnegie Mellon University, Meta AI
  * [ECCV2022] https://arxiv.org/abs/2112.08879
  * One-stage approach, unified detection-interaction
* **EDA: Explicit Text-Decoupling and Dense Alignment for 3D Visual Grounding** | [Github](https://github.com/yanmin-wu/EDA)
  * Yanmin Wu, Xinhua Cheng, Renrui Zhang, Zesen Cheng, Jian Zhang
  * Peking University, The Chinese University of Hong Kong, Peng Cheng Laboratory, Shanghai AI Laboratory
  * [CVPR2023] https://arxiv.org/abs/2209.14941
  * One-stage approach, unified detection-interaction, text-decoupling, dense
* **Dense Object Grounding in 3D Scenes** | 
  * Wencan Huang, Daizong Liu, Wei Hu
  * Peking University
  * [ACMMM2023] https://arxiv.org/abs/2309.02224
  * One-stage approach, unified detection-interaction, transformer
* **3DRP-Net: 3D Relative Position-aware Network for 3D Visual Grounding** |
  * Zehan Wang, Haifeng Huang, Yang Zhao, Linjun Li, Xize Cheng, Yichen Zhu, Aoxiong Yin, Zhou Zhao
  * Zhejiang University, ByteDance
  * [EMNLP2023] https://aclanthology.org/2023.emnlp-main.656/
  * One-stage approach, unified detection-interaction, relative position
* **LAMM: Language-Assisted Multi-Modal Instruction-Tuning Dataset, Framework, and Benchmark** | [Github](https://github.com/OpenLAMM/LAMM)
  * Zhenfei Yin, Jiong Wang, Jianjian Cao, Zhelun Shi, Dingning Liu, Mukai Li, Lu Sheng, Lei Bai, Xiaoshui Huang, Zhiyong Wang, Jing Shao, Wanli Ouyang
  * Shanghai AI Lab, Beihang University, The Chinese University of Hong Kong (Shenzhen), Fudan University, Dalian University of Technology, The University of Sydney
  * [NeurIPs2023] https://arxiv.org/abs/2306.06687
  * A dataset, One-stage approach, regression-based, multi-task
* **PATRON: Perspective-Aware Multitask Model for Referring Expression Grounding Using Embodied Multimodal Cues** | 
  * Md Mofijul Islam, Alexi Gladstone, Tariq Iqbal
  * University of Virginia
  * [AAAI2023] https://ojs.aaai.org/index.php/AAAI/article/view/25177
  * A dataset, One-stage approach, multi-task, multi-modal
* **Toward Fine-Grained 3D Visual Grounding through Referring Textual Phrases** | [Github](https://github.com/CurryYuan/PhraseRefer)
  * Zhihao Yuan, Xu Yan, Zhuo Li, Xuhao Li, Yao Guo, Shuguang Cui, Zhen Li
  * CUHK-Shenzhen, Shanghai Jiao Tong University
  * [Arxiv2023] https://arxiv.org/abs/2207.01821
  * A dataset, One-stage approach, unified detection-interaction
* **A Unified Framework for 3D Point Cloud Visual Grounding** | [Github](https://github.com/Leon1207/3DRefTR)
  * Haojia Lin, Yongdong Luo, Xiawu Zheng, Lijiang Li, Fei Chao, Taisong Jin, Donghao Luo, Yan Wang, Liujuan Cao, Rongrong Ji
  * Xiamen University, Peng Cheng Laboratory
  * [Arxiv2023] https://arxiv.org/abs/2308.11887
  * One-stage approach, unified detection-interaction, superpoint
* **Uni3DL: Unified Model for 3D and Language Understanding** |
  * Xiang Li, Jian Ding, Zhaoyang Chen, Mohamed Elhoseiny
  * King Abdullah University of Science and Technology, Ecole Polytechnique
  * [Arxiv2023] https://arxiv.org/abs/2312.03026
  * One-stage approach, regression-based, multi-task
* **3D-STMN: Dependency-Driven Superpoint-Text Matching Network for End-to-End 3D Referring Expression Segmentation** | [Github](https://github.com/sosppxo/3D-STMN)
  * Changli Wu, Yiwei Ma, Qi Chen, Haowei Wang, Gen Luo, Jiayi Ji, Xiaoshuai Sun
  * Xiamen University
  * [AAAI2024] https://arxiv.org/abs/2308.16632
  * One-stage approach, unified detection-interaction, superpoint
* **Vision-Language Pre-training with Object Contrastive Learning for 3D Scene Understanding** | 
  * Taolin Zhang, Sunan He, Tao Dai, Zhi Wang, Bin Chen, Shu-Tao Xia
  * Tsinghua University, Hong Kong University of Science and Technology, Shenzhen University, Harbin Institute of Technology(Shenzhen), Peng Cheng Laboratory
  * [AAAI2024] https://arxiv.org/abs/2305.10714
  * One-stage approach, regression-based, pre-training
* **Visual Programming for Zero-shot Open-Vocabulary 3D Visual Grounding** | [Github](https://github.com/CurryYuan/ZSVG3D)
  * Zhihao Yuan, Jinke Ren, Chun-Mei Feng, Hengshuang Zhao, Shuguang Cui, Zhen Li
  * The Chinese University of Hong Kong (Shenzhen), A*STAR, The University of Hong Kong
  * [CVPR2024] https://arxiv.org/abs/2311.15383
  * One-stage approach, zero-shot, data construction
* **G3-LQ: Marrying Hyperbolic Alignment with Explicit Semantic-Geometric Modeling for 3D Visual Grounding** | 
  * Yuan Wang, Yali Li, Shengjin Wang
  * Tsinghua University, Beijing National Research Center for Information Science and Technology 
  * [CVPR2024] https://openaccess.thecvf.com/content/CVPR2024/papers/Wang_G3-LQ_Marrying_Hyperbolic_Alignment_with_Explicit_Semantic-Geometric_Modeling_for_3D_CVPR_2024_paper.pdf
  * One-stage approach, regression-based
* **PointCloud-Text Matching: Benchmark Datasets and a Baseline** | 
  * Yanglin Feng, Yang Qin, Dezhong Peng, Hongyuan Zhu, Xi Peng, Peng Hu
  * Sichuan University, A*STAR
  * [Arxiv2024] https://arxiv.org/abs/2403.19386
  * A dataset, One-stage approach, regression-based, pre-training

## Weakly-supervised
* **Distilling Coarse-to-Fine Semantic Matching Knowledge for Weakly Supervised 3D Visual Grounding** | [Github](https://github.com/ZzZZCHS/WS-3DVG)
  * Zehan Wang, Haifeng Huang, Yang Zhao, Linjun Li, Xize Cheng, Yichen Zhu, Aoxiong Yin, Zhou Zhao
  * Zhejiang University
  * [ICCV2023] https://openaccess.thecvf.com/content/ICCV2023/papers/Wang_Distilling_Coarse-to-Fine_Semantic_Matching_Knowledge_for_Weakly_Supervised_3D_Visual_ICCV_2023_paper.pdf
  * weakly-supervised, two-stage matching, pseudo label
* **Weakly-Supervised 3D Visual Grounding based on Visual Linguistic Alignment** | 
  * Xiaoxu Xu, Yitian Yuan, Qiudan Zhang, Wenhui Wu, Zequn Jie, Lin Ma, Xu Wang
  * Meituan
  * [Arxiv2023] https://arxiv.org/abs/2312.09625
  * weakly-supervised, two-stage matching, multi-modal

## Other-Modality
* **Refer-it-in-RGBD: A Bottom-up Approach for 3D Visual Grounding in RGBD Images** | [Github](https://github.com/HaolinLiu97/Refer-it-in-RGBD)
  * Haolin Liu, Anran Lin, Xiaoguang Han, Lei Yang, Yizhou Yu, Shuguang Cui
  * CUHK-Shenzhen, Deepwise AI Lab, The University of Hong Kong
  * [CVPR2021] https://arxiv.org/pdf/2103.07894
  * No point cloud input, RGB-D image
* **PATRON: Perspective-Aware Multitask Model for Referring Expression Grounding Using Embodied Multimodal Cues** | 
  * Md Mofijul Islam, Alexi Gladstone, Tariq Iqbal
  * University of Virginia
  * [AAAI2023] https://ojs.aaai.org/index.php/AAAI/article/view/25177
  * No point cloud input, multi-view
* **Mono3DVG: 3D Visual Grounding in Monocular Images** | [Github](https://github.com/ZhanYang-nwpu/Mono3DVG)
  * Yang Zhan, Yuan Yuan, Zhitong Xiong
  * Northwestern Polytechnical University, Technical University of Munich
  * [AAAI2024] https://arxiv.org/pdf/2312.08022
  * No point cloud input, monocular image
* **EmbodiedScan: A Holistic Multi-Modal 3D Perception Suite Towards Embodied AI** | [Github](https://github.com/OpenRobotLab/EmbodiedScan)
  * Tai Wang, Xiaohan Mao, Chenming Zhu, Runsen Xu, Ruiyuan Lyu, Peisen Li, Xiao Chen, Wenwei Zhang, Kai Chen, Tianfan Xue, Xihui Liu, Cewu Lu, Dahua Lin, Jiangmiao Pang
  * Shanghai AI Laboratory, Shanghai Jiao Tong University, The University of Hong Kong, The Chinese University of Hong Kong, Tsinghua University
  * [CVPR2024] https://arxiv.org/abs/2312.16170
  * A dataset, No point cloud input, RGB-D image
* **WildRefer: 3D Object Localization in Large-scale Dynamic Scenes with Multi-modal Visual Data and Natural Language** | 
  * Zhenxiang Lin, Xidong Peng, Peishan Cong, Yuenan Hou, Xinge Zhu, Sibei Yang, Yuexin Ma
  * ShanghaiTech University, Shanghai AI Laboratory, The Chinese University of Hong Kong
  * [Arxiv2023] https://arxiv.org/abs/2304.05645
  * No point cloud input, wild point cloud, additional multi-modal input

## LLMs-based
* **ViewRefer: Grasp the Multi-view Knowledge for 3D Visual Grounding with GPT and Prototype Guidance** | [Github](https://github.com/Ivan-Tang-3D/ViewRefer3D)
  * Zoey Guo, Yiwen Tang, Ray Zhang, Dong Wang, Zhigang Wang, Bin Zhao, Xuelong Li
  * Shanghai Artificial Intelligence Laboratory, The Chinese University of Hong Kong, Northwestern Polytechnical University
  * [ICCV2023] https://arxiv.org/pdf/2303.16894
  * LLMs-based, enriching text description
* **LAMM: Language-Assisted Multi-Modal Instruction-Tuning Dataset, Framework, and Benchmark** | [Github](https://github.com/OpenGVLab/LAMM)
  * Zhenfei Yin, Jiong Wang, Jianjian Cao, Zhelun Shi, Dingning Liu, Mukai Li, Lu Sheng, Lei Bai, Xiaoshui Huang, Zhiyong Wang, Jing Shao, Wanli Ouyang
  * Shanghai AI Lab, Beihang University, The Chinese University of Hong Kong (Shenzhen), Fudan University, Dalian University of Technology, The University of Sydney
  * [NeurIPs2023] https://arxiv.org/abs/2306.06687
  * LLMs-based, LLM architecture
* **Transcribe3D: Grounding LLMs Using Transcribed Information for 3D Referential Reasoning with Self-Corrected Finetuning** | 
  * Jiading Fang, Xiangshan Tan, Shengjie Lin, Hongyuan Mei, Matthew R. Walter
  * Toyota Technological Institute at Chicago
  * [CoRL2023] https://openreview.net/forum?id=7j3sdUZMTF
  * LLMs-based, enriching text description
* **LLM-Grounder: Open-Vocabulary 3D Visual Grounding with Large Language Model as an Agent** | 
  * Jianing Yang, Xuweiyi Chen, Shengyi Qian, Nikhil Madaan, Madhavan Iyengar, David F. Fouhey, Joyce Chai1
  *  University of Michigan, New York University
  * [Arxiv2023] https://arxiv.org/abs/2309.12311
  * LLMs-based, enriching text description
* **Mono3DVG: 3D Visual Grounding in Monocular Images** | [Github](https://github.com/ZhanYang-nwpu/Mono3DVG)
  * Yang Zhan, Yuan Yuan, Zhitong Xiong
  * Northwestern Polytechnical University, Technical University of Munich
  * [AAAI2024] https://arxiv.org/pdf/2312.08022
  * LLMs-based, enriching text description
* **COT3DREF: Chain-of-Thoughts Data-Efficient 3D Visual Grounding** | [Github](https://github.com/CoT3DRef/COT3DRef)
  * Eslam Mohamed Bakr, Mohamed Ayman, Mahmoud Ahmed, Habib Slim, Mohamed Elhoseiny
  * King Abdullah University of Science and Technology
  * [ICLR2024] https://arxiv.org/abs/2310.06214
  * LLMs-based, Chain-of-Thoughts, reasoning
* **Visual Programming for Zero-shot Open-Vocabulary 3D Visual Grounding** | [Github](https://github.com/CurryYuan/ZSVG3D)
  * Zhihao Yuan, Jinke Ren, Chun-Mei Feng, Hengshuang Zhao, Shuguang Cui, Zhen Li
  * The Chinese University of Hong Kong (Shenzhen), A*STAR, The University of Hong Kong
  * [CVPR2024] https://arxiv.org/abs/2311.15383
  * LLMs-based, construct text description
* **Naturally Supervised 3D Visual Grounding with Language-Regularized Concept Learners** | [Github](https://github.com/chunfeng3364/LARC)
  * Chun Feng, Joy Hsu, Weiyu Liu, Jiajun Wu
  * Stanford University
  * [CVPR2024] https://arxiv.org/abs/2404.19696
  * LLMs-based, language constraint
* **3DMIT: 3D MULTI-MODAL INSTRUCTION TUNING FOR SCENE UNDERSTANDING** | [Github](https://github.com/staymylove/3DMIT)
  * Zeju Li, Chao Zhang, Xiaoyan Wang, Ruilong Ren, Yifan Xu, Ruifei Ma, Xiangde Liu
  * Beijing University of Posts and Telecommunications, Beijing Digital Native Digital City Research Center, Peking University, Beihang University, Beijing University of Science and Technology
  * [Arxiv2024] https://arxiv.org/abs/2401.03201
  * LLMs-based, LLM architecture
* **DOrA: 3D Visual Grounding with Order-Aware Referring** | 
  * Tung-Yu Wu, Sheng-Yu Huang, Yu-Chiang Frank Wang
  * National Taiwan University, NVIDIA
  * [Arxiv2024] https://arxiv.org/abs/2403.16539
  * LLMs-based, Chain-of-Thoughts
* **SCENEVERSE:
Scaling 3D Vision-Language Learning for Grounded Scene Understanding** | [Github](https://github.com/scene-verse/SceneVerse)
  * Baoxiong Jia , Yixin Chen , Huanyue Yu, Yan Wang, Xuesong Niu, Tengyu Liu, Qing Li, Siyuan Huang
  * Beijing Institute for General Artificial Intelligence
  * [Arxiv2024] https://arxiv.org/abs/2401.09340
  * A dataset, LLMs-based, LLM architecture

## Outdoor-Scenes
* **Talk2Radar: Bridging Natural Language with 4D mmWave Radar for 3D Referring Expression Comprehension** | [Github](https://github.com/GuanRunwei/Talk2Radar)
  * Runwei Guan, Ruixiao Zhang, Ningwei Ouyang, Jianan Liu, Ka Lok Man, Xiaohao Cai, Ming Xu, Jeremy Smith, Eng Gee Lim, Yutao Yue, Hui Xiong
  * JITRI, University of Liverpool, University of Southampton, Vitalent Consulting, Xi’an Jiaotong-Liverpool University, HKUST (GZ)
  * [Arxiv2024] https://arxiv.org/abs/2405.12821
  * Ourdoor scene, autonomous driving
* **Talk to Parallel LiDARs: A Human-LiDAR Interaction Method Based on 3D Visual Grounding** | 
  * Yuhang Liu, Boyi Sun, Guixu Zheng, Yishuo Wang, Jing Wang, Fei-Yue Wang
  * Chinese Academy of Sciences, South China Agricultural University, Beijing Institute of Technology
  * [Arxiv2024] https://arxiv.org/abs/2405.15274
  * Ourdoor scene, autonomous driving
