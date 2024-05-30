# Awesome-LVLM-Attack [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)
A **continual** collection of papers related to safety of Multimodal Large Language Models (MLLMs).

LMM hallucination😵 refers to occasional instances where LMMs generate content that appears plausible but deviates from or conflicts with the provided image. 
LMMs tend to rely more on their own parametric knowledge than on provided visual features, causing them to respond with guesses and generate multimodal hallucinations.

In the MLLM community, we've developed methods for detecting, evaluating, and mitigating hallucinations👍.



> If you find some important work missed, it would be super helpful to let me know (`isXinLiu@gmail.com`). Thanks!

> If you find our survey useful for your research, please consider citing:

```
@article{liu:arxiv2024,
  title={Safety of Multimodal Large Language Models on Images and Text},
  author={Liu, Xin and Zhu, Yichen and Lan, Yunshi and Yang, Chao and Qiao, Yu},
  journal={arXiv preprint arXiv:2402.00357},
  year={2024}
}
```

**Table of Contents**
- [Evaluation](#Evaluation)
- [Attack](#Attack)
- [Defense](#Defense)
- [Other](#Other)
---

## Evaluation
* **Privacy-Aware Visual Language Models**
  * Laurens Samson, Nimrod Barazani, Sennay Ghebreab, Yuki M. Asano
  * University of Amsterdam
  * [2024.05.27] https://arxiv.org/abs/2405.17423
  * Defense, Benchmark
* **Learning To See But Forgetting To Follow: Visual Instruction Tuning Makes LLMs More Prone To Jailbreak Attacks** | [Github](https://github.com/gpantaz/vl_jailbreak) ![Star](https://img.shields.io/github/stars/gpantaz/vl_jailbreak.svg?style=social&label=Star)
  * Georgios Pantazopoulos, Amit Parekh, Malvina Nikandrou, Alessandro Suglia
  * Heriot-Watt University
  * [2024.05.07] https://arxiv.org/abs/2405.04403
  * A finding
* **Private Attribute Inference from Images with Vision-Language Models**
  * Batuhan Tömekçe, Mark Vero, Robin Staab, Martin Vechev
  * ETH Zurich
  * [2024.04.16] https://arxiv.org/abs/2404.10618
  * Benchmark
* **Red Teaming GPT-4V: Are GPT-4V Safe Against Uni/Multi-Modal Jailbreak Attacks?**
  * Shuo Chen, Zhen Han, Bailan He, Zifeng Ding, Wenqian Yu, Philip Torr, Volker Tresp, Jindong Gu
  * LMU Munich | University of Oxford | Siemens AG | MCML | Wuhan University
  * [2024.04.04] https://arxiv.org/abs/2404.03411
  * Benchmark
* **JailBreakV-28K: A Benchmark for Assessing the Robustness of MultiModal Large Language Models against Jailbreak Attacks** | [Github](https://github.com/EddyLuo1232/JailBreakV_28K) ![Star](https://img.shields.io/github/stars/EddyLuo1232/JailBreakV_28K.svg?style=social&label=Star)
  * Weidi Luo, Siyuan Ma, Xiaogeng Liu, Xiaoyu Guo, Chaowei Xiao
  * The Ohio State University | University of Wisconsin-Madison
  * [2024.04.03] https://arxiv.org/abs/2404.03027
  * Benchmark
* **Uncovering Bias in Large Vision-Language Models with Counterfactuals**
  * Phillip Howard, Anahita Bhiwandiwalla, Kathleen C. Fraser, Svetlana Kiritchenko
  * Intel Labs | National Research Council Canada
  * [2024.03.29] https://arxiv.org/abs/2404.00166
  * Analysis
* **Assessment of Multimodal Large Language Models in Alignment with Human Values** | [Github](https://github.com/OpenGVLab/LAMM) ![Star](https://img.shields.io/github/stars/OpenGVLab/LAMM.svg?style=social&label=Star)
  * Zhelun Shi, Zhipin Wang, Hongxing Fan, Zaibin Zhang, Lijun Li, Yongting Zhang, Zhenfei Yin, Lu Sheng, Yu Qiao, Jing Shao
  * Shanghai Artificial Intelligence Laboratory | School of Software, Beihang University | Dalian University of Technology | University of Science and Technology of China | The University of Sydney
  * [2024.03.26] https://arxiv.org/abs/2403.17830
  * Benchmark
* **Evaluating the Efficacy of Prompt-Engineered Large Multimodal Models Versus Fine-Tuned Vision Transformers in Image-Based Security Applications**
  * Fouad Trad, Ali Chehab
  * American University of Beirut
  * [2024.03.26] https://arxiv.org/abs/2403.17787
  * Analysis
* **AVIBench: Towards Evaluating the Robustness of Large Vision-Language Model on Adversarial Visual-Instructions**
  * Hao Zhang, Wenqi Shao, Hong Liu, Yongqiang Ma, Ping Luo, Yu Qiao, Kaipeng Zhang
  * Xi'an Jiaotong University | Shanghai Artificial Intelligence Laboratory | Osaka University
  * [2024.03.14] https://arxiv.org/abs/2403.09346
  * Benchmark
* **Prismatic VLMs: Investigating the Design Space of Visually-Conditioned Language Models** | [Github](https://github.com/TRI-ML/prismatic-vlms) ![Star](https://img.shields.io/github/stars/TRI-ML/prismatic-vlms.svg?style=social&label=Star)
  * Siddharth Karamcheti, Suraj Nair, Ashwin Balakrishna, Percy Liang, Thomas Kollar, Dorsa Sadigh
  * Stanford | Toyota Research Institute
  * [2024.02.12] https://arxiv.org/abs/2402.07865
  * Insights
* **HarmBench: A Standardized Evaluation Framework for Automated Red Teaming and Robust Refusal** | [Github](https://github.com/centerforaisafety/HarmBench) ![Star](https://img.shields.io/github/stars/centerforaisafety/HarmBench.svg?style=social&label=Star)
  * Mantas Mazeika, Long Phan, Xuwang Yin, Andy Zou, Zifan Wang, Norman Mu, Elham Sakhaee, Nathaniel Li, Steven Basart, Bo Li, David Forsyth, Dan Hendrycks
  * University of Illinois Urbana-Champaign | Center for AI Safety | Carnegie Mellon University | UC Berkeley | Microsoft
  * [2024.02.06] https://arxiv.org/abs/2402.04249
  * Benchmark
* **Safety Fine-Tuning at (Almost) No Cost: A Baseline for Vision Large Language Models** | [Github](https://github.com/ys-zong/VLGuard) ![Star](https://img.shields.io/github/stars/ys-zong/VLGuard.svg?style=social&label=Star)
  * Yongshuo Zong, Ondrej Bohdal, Tingyang Yu, Yongxin Yang, Timothy Hospedales
  * University of Edinburgh | EPFL
  * [2024.02.03] https://arxiv.org/abs/2402.02207
  * Defense, Benchmark
* **Red Teaming Visual Language Models**
  * Mukai Li, Lei Li, Yuwei Yin, Masood Ahmed, Zhenguang Liu, Qi Liu
  * The University of Hong Kong | Zhejiang University
  * [2024.01.23] https://arxiv.org/abs/2401.12915
  * Benchmark
* **InferAligner: Inference-Time Alignment for Harmlessness through Cross-Model Guidance** | [Github](https://github.com/Jihuai-wpy/InferAligner) ![Star](https://img.shields.io/github/stars/Jihuai-wpy/InferAligner.svg?style=social&label=Star)
  * Pengyu Wang, Dong Zhang, Linyang Li, Chenkun Tan, Xinghao Wang, Ke Ren, Botian Jiang, Xipeng Qiu
  * Fudan University
  * [2024.01.20] https://arxiv.org/abs/2401.11206
  * Defense, Benchmark
* **GOAT-Bench: Safety Insights to Large Multimodal Models through Meme-Based Social Abuse**
  * Hongzhan Lin, Ziyang Luo, Bo Wang, Ruichao Yang, Jing Ma
  * Hong Kong Baptist University
  * [2024.01.03] https://arxiv.org/abs/2401.01523
  * Benchmark
* **ToViLaG: Your Visual-Language Generative Model is Also An Evildoer**
  * Xinpeng Wang, Xiaoyuan Yi, Han Jiang, Shanlin Zhou, Zhihua Wei, Xing Xie
  * Tongji University | Microsoft Research Asia
  * [2023.12.13] https://arxiv.org/abs/2312.11523v1
  * Benchmark
* **MM-SafetyBench: A Benchmark for Safety Evaluation of Multimodal Large Language Models** | [Github](https://github.com/isXinLiu/MM-SafetyBench) ![Star](https://img.shields.io/github/stars/isXinLiu/MM-SafetyBench.svg?style=social&label=Star)
  * Xin Liu, Yichen Zhu, Jindong Gu, Yunshi Lan, Chao Yang, Yu Qiao
  * East China Normal University | Midea Group | Shanghai AI Laboratory
  * [2023.11.29] https://arxiv.org/abs/2311.17600
  * Attack, Benchmark
* **Large Language Models as Automated Aligners for benchmarking Vision-Language Models**
  * Yuanfeng Ji, Chongjian Ge, Weikai Kong, Enze Xie, Zhengying Liu, Zhengguo Li, Ping Luo
  * The University of Hong Kong | Huawei Noah's Ark Lab
  * [2023.11.24] https://arxiv.org/abs/2311.14580
  * Benchmark
* **DRESS: Instructing Large Vision-Language Models to Align and Interact with Humans via Natural Language Feedback**
  * Yangyi Chen, Karan Sikka, Michael Cogswell, Heng Ji, Ajay Divakaran
  * SRI International | University of Illinois Urbana-Champaign
  * [2023.11.16] https://arxiv.org/abs/2311.10081
  * Defense, Benchmark
* **FigStep: Jailbreaking Large Vision-language Models via Typographic Visual Prompts** | [Github](https://github.com/ThuCCSLab/FigStep) ![Star](https://img.shields.io/github/stars/ThuCCSLab/FigStep.svg?style=social&label=Star)
  * Yichen Gong, Delong Ran, Jinyuan Liu, Conglei Wang, Tianshuo Cong, Anyu Wang, Sisi Duan, Xiaoyun Wang
  * Tsinghua University | Shandong University | Carnegie Mellon University
  * [2023.11.09] https://arxiv.org/abs/2311.05608
  * Attack, Benchmark
* **Fine-tuning Aligned Language Models Compromises Safety, Even When Users Do Not Intend To!** | [Github](https://github.com/LLM-Tuning-Safety/LLMs-Finetuning-Safety) ![Star](https://img.shields.io/github/stars/LLM-Tuning-Safety/LLMs-Finetuning-Safety.svg?style=social&label=Star)
  * Xiangyu Qi, Yi Zeng, Tinghao Xie, Pin-Yu Chen, Ruoxi Jia, Prateek Mittal, Peter Henderson
  * Princeton University | Virginia Tech | IBM Research | Stanford University
  * [2023.10.05] https://arxiv.org/abs/2310.03693
  * A finding
* **Can Language Models be Instructed to Protect Personal Information?** | [Github](https://github.com/ethanm88/llm-access-control) ![Star](https://img.shields.io/github/stars/ethanm88/llm-access-control.svg?style=social&label=Star)
  * Yang Chen, Ethan Mendes, Sauvik Das, Wei Xu, Alan Ritter
  * Georgia Institute of Technology | Carnegie Mellon University
  * [2023.10.03] https://arxiv.org/abs/2310.02224
  * Attack, Defense, Benchmark
## Attack
* **White-box Multimodal Jailbreaks Against Large Vision-Language Models**
  * Ruofan Wang, Xingjun Ma, Hanxu Zhou, Chuanjun Ji, Guangnan Ye, Yu-Gang Jiang
  * Fudan University |  Shanghai Jiao Tong University | DataGrand Tech
  * [2024.05.28] https://arxiv.org/abs/2405.17894
  * Attack
* **Composite Backdoor Attacks Against Large Language Models** | [Github](https://github.com/MiracleHH/CBA) ![Star](https://img.shields.io/github/stars/MiracleHH/CBA.svg?style=social&label=Star)
  * Hai Huang, Zhengyu Zhao, Michael Backes, Yun Shen, Yang Zhang
  * CISPA Helmholtz Center for Information Security | Xi'an Jiaotong University | NetApp
  * [2024.03.30] https://arxiv.org/abs/2310.07676
  * Attack
* **Images are Achilles' Heel of Alignment: Exploiting Visual Vulnerabilities for Jailbreaking Multimodal Large Language Models**
  * Yifan Li, Hangyu Guo, Kun Zhou, Wayne Xin Zhao, Ji-Rong Wen
  * Renmin University | Beijing Key Laboratory of Big Data Management and Analysis Methods
  * [2024.03.14] https://arxiv.org/abs/2403.09792
  * Attack
* **ImgTrojan: Jailbreaking Vision-Language Models with ONE Image** | [Github](https://github.com/xijia-tao/ImgTrojan) ![Star](https://img.shields.io/github/stars/xijia-tao/ImgTrojan.svg?style=social&label=Star)
  * Xijia Tao, Shuai Zhong, Lei Li, Qi Liu, Lingpeng Kong
  * The University of Hong Kong
  * [2024.03.05] https://arxiv.org/abs/2403.02910
  * Attack
* **The Wolf Within: Covert Injection of Malice into MLLM Societies via an MLLM Operative** | [Github](https://github.com/ChengshuaiZhao0/The-Wolf-Within) ![Star](https://img.shields.io/github/stars/ChengshuaiZhao0/The-Wolf-Within.svg?style=social&label=Star)
  * Zhen Tan, Chengshuai Zhao, Raha Moraffah, Yifan Li, Yu Kong, Tianlong Chen, Huan Liu
  * Arizona State University | Michigan State University | MIT
  * [2024.02.20] https://arxiv.org/abs/2402.14859
  * Attack(Agent)
* **Exploiting Alpha Transparency In Language And Vision-Based AI Systems**
  * David Noever, Forrest McKee
  * PeopleTec
  * [2024.02.15] https://arxiv.org/abs/2402.09671
  * Attack
* **Test-Time Backdoor Attacks on Multimodal Large Language Models** | [Github](https://github.com/sail-sg/AnyDoor) ![Star](https://img.shields.io/github/stars/sail-sg/AnyDoor.svg?style=social&label=Star)
  * Dong Lu, Tianyu Pang, Chao Du, Qian Liu, Xianjun Yang, Min Lin
  * Southern University of Science and Technology | Sea AI Lab | University of California
  * [2024.02.13] https://arxiv.org/abs/2402.08577
  * Attack
* **Agent Smith: A Single Image Can Jailbreak One Million Multimodal LLM Agents Exponentially Fast** | [Github](https://github.com/sail-sg/Agent-Smith) ![Star](https://img.shields.io/github/stars/sail-sg/Agent-Smith.svg?style=social&label=Star)
  * Xiangming Gu, Xiaosen Zheng, Tianyu Pang, Chao Du, Qian Liu, Ye Wang, Jing Jiang, Min Lin
  * Sea AI Lab | National University of Singapore | Singapore Management University
  * [2024.02.13] https://arxiv.org/abs/2402.08567
  * Attack(Agent)
* **Shadowcast: Stealthy Data Poisoning Attacks Against Vision-Language Models** | [Github](https://github.com/umd-huang-lab/VLM-Poisoning) ![Star](https://img.shields.io/github/stars/umd-huang-lab/VLM-Poisoning.svg?style=social&label=Star)
  * Yuancheng Xu, Jiarui Yao, Manli Shu, Yanchao Sun, Zichu Wu, Ning Yu, Tom Goldstein, Furong Huang
  * University of Maryland, College Park | JPMorgan AI Research | University of Waterloo | Salesforce Research
  * [2024.02.05] https://arxiv.org/abs/2402.06659
  * Attack
* **GUARD: Role-playing to Generate Natural-language Jailbreakings to Test Guideline Adherence of Large Language Models**
  * Haibo Jin, Ruoxi Chen, Andy Zhou, Jinyin Chen, Yang Zhang, Haohan Wang
  * University of Illinois at Urbana-Champaign | Zhejiang University of Technology | Lapis Labs
  * [2024.02.05] https://arxiv.org/abs/2402.03299
  * Attack
* **Jailbreaking Attack against Multimodal Large Language Model**
  * Zhenxing Niu, Haodong Ren, Xinbo Gao, Gang Hua, Rong Jin
  * Xidian University | Wormpex AI Research | Meta
  * [2024.02.04] https://arxiv.org/abs/2402.02309
  * Attack
* **An Image Is Worth 1000 Lies: Transferability of Adversarial Images across Prompts on Vision-Language Models** | [Github](https://github.com/Haochen-Luo/CroPA) ![Star](https://img.shields.io/github/stars/Haochen-Luo/CroPA.svg?style=social&label=Star)
  * Haochen Luo, Jindong Gu, Fengyuan Liu, Philip Torr
  * University of Oxford
  * [2024.01.16] https://openreview.net/forum?id=nc5GgFAvtk
  * Attack
* **MM-SafetyBench: A Benchmark for Safety Evaluation of Multimodal Large Language Models** | [Github](https://github.com/isXinLiu/MM-SafetyBench) ![Star](https://img.shields.io/github/stars/isXinLiu/MM-SafetyBench.svg?style=social&label=Star)
  * Xin Liu, Yichen Zhu, Jindong Gu, Yunshi Lan, Chao Yang, Yu Qiao
  * East China Normal University | Midea Group | Shanghai AI Laboratory
  * [2023.11.29] https://arxiv.org/abs/2311.17600
  * Attack, Benchmark
* **How Many Unicorns Are in This Image? A Safety Evaluation Benchmark for Vision LLMs** | [Github](https://github.com/UCSC-VLAA/vllm-safety-benchmark) ![Star](https://img.shields.io/github/stars/UCSC-VLAA/vllm-safety-benchmark.svg?style=social&label=Star)
  * Haoqin Tu, Chenhang Cui, Zijun Wang, Yiyang Zhou, Bingchen Zhao, Junlin Han, Wangchunshu Zhou, Huaxiu Yao, Cihang Xie
  * UC Santa Cruz | UNC-Chapel Hill | University of Edinburgh | University of Oxford | AIWaves Inc
  * [2023.11.27] https://arxiv.org/abs/2311.16101
  * Attack
* **Jailbreaking GPT-4V via Self-Adversarial Attacks with System Prompts**
  * Yuanwei Wu, Xiang Li, Yixin Liu, Pan Zhou, Lichao Sun
  * Huazhong University of Science and Technology | Lehigh University
  * [2023.11.15] https://arxiv.org/abs/2311.09127
  * Attack, Defense
* **FigStep: Jailbreaking Large Vision-language Models via Typographic Visual Prompts** | [Github](https://github.com/ThuCCSLab/FigStep) ![Star](https://img.shields.io/github/stars/ThuCCSLab/FigStep.svg?style=social&label=Star)
  * Yichen Gong, Delong Ran, Jinyuan Liu, Conglei Wang, Tianshuo Cong, Anyu Wang, Sisi Duan, Xiaoyun Wang
  * Tsinghua University | Shandong University | Carnegie Mellon University
  * [2023.11.09] https://arxiv.org/abs/2311.05608
  * Attack, Benchmark
* **Misusing Tools in Large Language Models With Visual Adversarial Examples**
  * Xiaohan Fu, Zihan Wang, Shuheng Li, Rajesh K. Gupta, Niloofar Mireshghallah, Taylor Berg-Kirkpatrick, Earlence Fernandes
  * University of California San Diego | University of Washington
  * [2023.10.04] https://arxiv.org/abs/2310.03185
  * Attack
* **Can Language Models be Instructed to Protect Personal Information?** | [Github](https://github.com/ethanm88/llm-access-control) ![Star](https://img.shields.io/github/stars/ethanm88/llm-access-control.svg?style=social&label=Star)
  * Yang Chen, Ethan Mendes, Sauvik Das, Wei Xu, Alan Ritter
  * Georgia Institute of Technology | Carnegie Mellon University
  * [2023.10.03] https://arxiv.org/abs/2310.02224
  * Attack, Defense, Benchmark
* **How Robust is Google's Bard to Adversarial Image Attacks?** | [Github](https://github.com/thu-ml/Attack-Bard) ![Star](https://img.shields.io/github/stars/thu-ml/Attack-Bard.svg?style=social&label=Star)
  * Yinpeng Dong, Huanran Chen, Jiawei Chen, Zhengwei Fang, Xiao Yang, Yichi Zhang, Yu Tian, Hang Su, Jun Zhu
  * Tsinghua University | RealAI
  * [2023.09.21] https://arxiv.org/abs/2309.11751
  * Attack
* **Image Hijacks: Adversarial Images can Control Generative Models at Runtime** | [Github](https://github.com/euanong/image-hijacks) ![Star](https://img.shields.io/github/stars/euanong/image-hijacks.svg?style=social&label=Star)
  * Luke Bailey, Euan Ong, Stuart Russell, Scott Emmons
  * UC Berkeley | Harvard University | University of Cambridge
  * [2023.09.01] https://arxiv.org/abs/2309.00236
  * Attack
* **On the Adversarial Robustness of Multi-Modal Foundation Models**
  * Christian Schlarmann, Matthias Hein
  * University of Tubingen
  * [2023.08.21] https://arxiv.org/abs/2308.10741
  * Attack
* **Jailbreak in pieces: Compositional Adversarial Attacks on Multi-Modal Language Models**
  * Erfan Shayegani, Yue Dong, Nael Abu-Ghazaleh
  * University of California
  * [2023.07.26] https://arxiv.org/abs/2307.14539
  * Attack
* **Abusing Images and Sounds for Indirect Instruction Injection in Multi-Modal LLMs**
  * Eugene Bagdasaryan, Tsung-Yin Hsieh, Ben Nassi, Vitaly Shmatikov
  * Cornell Tech
  * [2023.07.19] https://arxiv.org/abs/2307.10490
  * Attack
* **Are aligned neural networks adversarially aligned?**
  * Nicholas Carlini, Milad Nasr, Christopher A. Choquette-Choo, Matthew Jagielski, Irena Gao, Anas Awadalla, Pang Wei Koh, Daphne Ippolito, Katherine Lee, Florian Tramer, Ludwig Schmidt
  * Google DeepMind | Stanford | University of Washington | ETH Zurich
  * [2023.06.26] https://arxiv.org/abs/2306.15447
  * Attack
* **Visual Adversarial Examples Jailbreak Aligned Large Language Models** | [Github](https://github.com/Unispac/Visual-Adversarial-Examples-Jailbreak-Large-Language-Models) ![Star](https://img.shields.io/github/stars/Unispac/Visual-Adversarial-Examples-Jailbreak-Large-Language-Models.svg?style=social&label=Star)
  * Xiangyu Qi, Kaixuan Huang, Ashwinee Panda, Peter Henderson, Mengdi Wang, Prateek Mittal
  * Princeton University | Stanford University
  * [2023.06.22] https://arxiv.org/abs/2306.13213
  * Attack
## Defense
* **Privacy-Aware Visual Language Models**
  * Laurens Samson, Nimrod Barazani, Sennay Ghebreab, Yuki M. Asano
  * University of Amsterdam
  * [2024.05.27] https://arxiv.org/abs/2405.17423
  * Defense, Benchmark
* **Safety Alignment for Vision Language Models**
  * Zhendong Liu, Yuanbi Nie, Yingshui Tan, Xiangyu Yue, Qiushi Cui, Chongjun Wang, Xiaoyong Zhu, Bo Zheng
  * Nanjing University | Chongqing University | Alibaba Group | Chinese University of Hong Kong
  * [2024.05.22] https://arxiv.org/abs/2405.13581
  * Defense
* **AdaShield: Safeguarding Multimodal Large Language Models from Structure-based Attack via Adaptive Shield Prompting** | [Github](https://github.com/rain305f/AdaShield) ![Star](https://img.shields.io/github/stars/rain305f/AdaShield.svg?style=social&label=Star)
  * Yu Wang, Xiaogeng Liu, Yu Li, Muhao Chen, Chaowei Xiao
  * Peking University | University of Wisconsin-Madison | International Digital Economy Academy | University of California, Davis
  * [2024.03.14] https://arxiv.org/abs/2403.09513
  * Defense
* **Eyes Closed, Safety On: Protecting Multimodal LLMs via Image-to-Text Transformation** | [Github](https://github.com/gyhdog99/ECSO) ![Star](https://img.shields.io/github/stars/gyhdog99/ECSO.svg?style=social&label=Star)
  * Yunhao Gou, Kai Chen, Zhili Liu, Lanqing Hong, Hang Xu, Zhenguo Li, Dit-Yan Yeung, James T. Kwok, Yu Zhang
  * Southern University of Science and Technology | Hong Kong University of Science and Technology | Huawei Noah's Ark Lab | Peng Cheng Laboratory
  * [2024.03.14] https://arxiv.org/abs/2403.09572
  * Defense
* **The First to Know: How Token Distributions Reveal Hidden Knowledge in Large Vision-Language Models?** | [Github](https://github.com/Qinyu-Allen-Zhao/LVLM-LP) ![Star](https://img.shields.io/github/stars/Qinyu-Allen-Zhao/LVLM-LP.svg?style=social&label=Star)
  * Qinyu Zhao, Ming Xu, Kartik Gupta, Akshay Asthana, Liang Zheng, Stephen Gould
  * The Australian National University | Seeing Machines Ltd
  * [2024.03.14] https://arxiv.org/abs/2403.09037
  * Defense
* **Safety Fine-Tuning at (Almost) No Cost: A Baseline for Vision Large Language Models** | [Github](https://github.com/ys-zong/VLGuard) ![Star](https://img.shields.io/github/stars/ys-zong/VLGuard.svg?style=social&label=Star)
  * Yongshuo Zong, Ondrej Bohdal, Tingyang Yu, Yongxin Yang, Timothy Hospedales
  * University of Edinburgh | EPFL
  * [2024.02.03] https://arxiv.org/abs/2402.02207
  * Defense, Benchmark
* **InferAligner: Inference-Time Alignment for Harmlessness through Cross-Model Guidance** | [Github](https://github.com/Jihuai-wpy/InferAligner) ![Star](https://img.shields.io/github/stars/Jihuai-wpy/InferAligner.svg?style=social&label=Star)
  * Pengyu Wang, Dong Zhang, Linyang Li, Chenkun Tan, Xinghao Wang, Ke Ren, Botian Jiang, Xipeng Qiu
  * Fudan University
  * [2024.01.20] https://arxiv.org/abs/2401.11206
  * Defense, Benchmark
* **MLLM-Protector: Ensuring MLLM's Safety without Hurting Performance** | [Github](https://github.com/pipilurj/MLLM-protector) ![Star](https://img.shields.io/github/stars/pipilurj/MLLM-protector.svg?style=social&label=Star)
  * Renjie Pi, Tianyang Han, Yueqi Xie, Rui Pan, Qing Lian, Hanze Dong, Jipeng Zhang, Tong Zhang
  * The Hong Kong University of Science and Technology | University of Illinois at Urbana-Champaign | The Hong Kong Polytechnic University
  * [2024.01.05] https://arxiv.org/abs/2401.02906
  * Defense
* **DRESS: Instructing Large Vision-Language Models to Align and Interact with Humans via Natural Language Feedback**
  * Yangyi Chen, Karan Sikka, Michael Cogswell, Heng Ji, Ajay Divakaran
  * SRI International | University of Illinois Urbana-Champaign
  * [2023.11.16] https://arxiv.org/abs/2311.10081
  * Defense, Benchmark
* **Jailbreaking GPT-4V via Self-Adversarial Attacks with System Prompts**
  * Yuanwei Wu, Xiang Li, Yixin Liu, Pan Zhou, Lichao Sun
  * Huazhong University of Science and Technology | Lehigh University
  * [2023.11.15] https://arxiv.org/abs/2311.09127
  * Attack, Defense
* **Can Language Models be Instructed to Protect Personal Information?** | [Github](https://github.com/ethanm88/llm-access-control) ![Star](https://img.shields.io/github/stars/ethanm88/llm-access-control.svg?style=social&label=Star)
  * Yang Chen, Ethan Mendes, Sauvik Das, Wei Xu, Alan Ritter
  * Georgia Institute of Technology | Carnegie Mellon University
  * [2023.10.03] https://arxiv.org/abs/2310.02224
  * Attack, Defense, Benchmark
## Other
* **Unbridled Icarus: A Survey of the Potential Perils of Image Inputs in Multimodal Large Language Model Security**
  * Yihe Fan, Yuxin Cao, Ziyu Zhao, Ziyao Liu, Shaofeng Li
  * TongJi University | Tsinghua University | Beijing University of Technology | Nanyang Technological University | Peng Cheng Laboratory
  * [2024.04.08] https://arxiv.org/abs/2404.05264
  * Survey
* **Safety of Multimodal Large Language Models on Images and Text**
  * Xin Liu, Yichen Zhu, Yunshi Lan, Chao Yang, Yu Qiao
  * East China Normal University | Midea Group | Shanghai AI Laboratory
  * [2024.02.01] https://arxiv.org/abs/2402.00357
  * Survey
