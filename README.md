# Awesome-ML4tooth

If you have any problems, suggestions or improvements, please submit the issue or PR.

## Contents
* [Datasets](#datasets)
* [Papers](#papers)
  * [Survey](#survey)
  * [LVLM](#lvlm)
  * [Agentic AI](#agentic-ai)
  * [Segmentation](#segmentation)
  * [Registration](#registration)
  * [Construction](#construction)
  * [Landmark](#landmark)
  * [Arrangement/Alignment](#arrangementalignment)
  * [Digital Smile Design](#digital-smile-design)
* [Projects](#projects)

## Datasets

### Imaging and 3D Datasets

| Dataset | Year | Size | Modality / Format | Access | Tasks |
| --- | --- | --- | --- | --- | --- |
| [MetaDent](https://huggingface.co/datasets/dengwenhui/MetaDent) | 2026 | 60,669 images; approximately 15K VQA pairs | Intraoral photographs + semi-structured text | Open, CC BY-NC 4.0 | VQA, captioning, multi-label classification |
| [COde: Multimodal Oro-Dental Dataset](https://doi.org/10.57967/hf/6421) | 2026 | 4,800 patients; 8,775 checkups; 50,000 photos; 8,056 radiographs | Intraoral photographs, radiographs, bilingual clinical records | Open on Hugging Face | Classification, report generation, LVLM training |
| [Adults' Dental CBCT Missing-Teeth Dataset](https://doi.org/10.57760/sciencedb.26465) | 2026 | 158 cases | CBCT DICOM + 3D JSON annotations | Open on ScienceDB | Missing-tooth detection and classification |
| [BRAR](https://figshare.com/s/cc2db8648788c7aa175c) | 2025 | 1,104 patients | Panoramic radiographs + demographics + tooth-level annotations | Open, CC BY 4.0 | Periodontal bone-resorption grading |
| [MMDental](https://doi.org/10.6084/m9.figshare.28505276) | 2025 | 660 patients; 161,200 CBCT slices; 2,125 records | 3D CBCT + expert clinical records | Open on Figshare | Multimodal diagnosis, report understanding, treatment planning |
| [FDTooth](https://www.physionet.org/content/fdtooth/1.0.0/) | 2025 | 241 patients | Intraoral photographs + paired CBCT | Controlled PhysioNet access | Fenestration and dehiscence detection |
| [STS-3D / STS-3D-Tooth](https://tianchi.aliyun.com/competition/entrance/532087/introduction) | 2023–2025 | 1,084 CBCT volumes in challenge release | 3D CBCT | Open challenge data | Tooth instance segmentation |
| [STS-2D / STS-2D-Tooth](https://tianchi.aliyun.com/competition/entrance/532086/introduction) | 2023–2025 | 9,500 panoramic X-rays in challenge release | 2D panoramic X-ray | Open challenge data | Tooth segmentation |
| [Multimodal Dental Dataset](https://www.nature.com/articles/s41597-024-04130-1) | 2024 | 169 patients; 329 CBCT scans | CBCT, panoramic and generated periapical radiographs | Controlled PhysioNet access | Segmentation, reconstruction, image translation |
| [toothfairy3](https://toothfairy3.grand-challenge.org) | 2025 | 532 | 3D CBCT | Open challenge data | Segmentation |
| [toothfairy2](https://toothfairy2.grand-challenge.org) | 2024 | 480 | 3D CBCT | Open challenge data | Segmentation |
| [toothfairy](https://toothfairy.grand-challenge.org) | 2023 | 290 | 3D CBCT | Open challenge data | Segmentation |
| [DENTEX](https://dentex.grand-challenge.org/data/) | 2023 | 2,332 labeled + 1,571 unlabeled X-rays | Panoramic X-ray + hierarchical annotations | Open on Zenodo | Quadrant, tooth enumeration and abnormality detection |
| [DC1000](https://github.com/Zzz512/MLUA) | 2023 | 1,000 | 2D panoramic X-ray | Open | Caries segmentation |
| [3DTeethSeg22 / Teeth3DS](https://github.com/abenhamadou/3DTeethSeg22_challenge) | 2022 | 1,800 | 3D intraoral scans | Open challenge data | Tooth segmentation and labeling |
| [Aariz](https://github.com/manwaarkhd/aariz-cephalometric-dataset) | 2022 | 1,000 | Lateral cephalometric radiographs | Open | Landmark localization |
| [Shining3D](https://drive.google.com/drive/folders/1fx9_KVEugZxbO3aTdwdfVTGf87_9FoLx) | 2020 | 210 | 3D intraoral scans | Open | Segmentation |
| [FALA](https://figshare.com/s/37ec464af8e81ae6ebbf) | 2016 | 400 | Lateral cephalometric radiographs | Open | Landmark localization |

### LVLM, LLM and Agent Benchmarks

| Dataset / Benchmark | Year | Size | Modality / Format | Access | Tasks |
| --- | --- | --- | --- | --- | --- |
| [GlobalDentBench](https://github.com/FreedomIntelligence/GlobalDentBench) | 2026 | 8,978 questions; 14 specialties; 88 countries/regions | MCQ, short-answer and case-based questions | OA subset open; full set by request | Clinical reasoning, robustness and safety-risk evaluation |
| [MM-OPG / ToothXpert Annotations](https://huggingface.co/datasets/jeffrey423/ToothXpert.MM-OPG-Annotations) | 2026 | 131,065 QA pairs; 11 conditions | Panoramic X-rays + visual QA + segmentation | Open, Apache 2.0 | OPG VQA, tooth segmentation and report generation |
| [MMOral-OPG-Bench](https://huggingface.co/datasets/OralGPT/MMOral-OPG-Bench) | 2025 | 100 images; 491 closed-ended + 578 open-ended questions | Panoramic X-rays + VQA | Open, MIT | Dental perception, history, pathology, jaw analysis and reporting |
| [MMOral-OPG-Training](https://huggingface.co/datasets/OralGPT/MMOral-OPG-Training) | 2025 | 18.7 GB; sample count not stated | Panoramic X-rays + instruction data | Gated on Hugging Face | Dental LVLM instruction tuning |
| [MetaDent-Bench](https://github.com/WenhDeng/metadent-bench) | 2026 | Approximately 15K VQA pairs; 18-class labels | Intraoral photographs + hierarchical annotations | Open benchmark and pipeline | VQA, captioning and multi-label classification |
| [OralCorpus](https://huggingface.co/datasets/OralGPT/OralCorpus) | 2026 | Approximately 134.8M tokens | Chinese and English dental text + vector databases | Gated on Hugging Face | RAG, domain adaptation and knowledge retrieval |
| [DentalBench](https://arxiv.org/abs/2508.20416) | 2025 | DentalQA: 36,597 questions; DentalCorpus: 337.35M tokens | Chinese-English text | Paper available; official public release not verified | Bilingual QA, SFT and RAG |
| [MMOral-Uni](https://openaccess.thecvf.com/content/CVPR2026/html/Hao_OralGPT-Omni_A_Versatile_Dental_Multimodal_Large_Language_Model_CVPR_2026_paper.html) | 2026 | 2,809 open-ended QA pairs | Five dental imaging modalities; five tasks | Announced by authors; release link not verified | Unified multimodal dental reasoning |
| [OralMLLM-Bench](https://arxiv.org/abs/2605.01333) | 2026 | 27 tasks; 3,820 clinician assessments | Periapical, panoramic and lateral cephalometric radiographs | Paper available; dataset release not verified | Perception, comprehension, prediction and decision-making |
| [DentalGemma-VQA](https://huggingface.co/datasets/naazimsnh02/dentalgemma-vqa) | 2026 | 2,529 image-text pairs | Clinical photographs + panoramic X-rays | Open community dataset, Apache 2.0 | VQA, pathology classification and localization |

Access labels: **Open** = directly downloadable; **Controlled/Gated** = registration, agreement or approval required; **OA subset** = only an open test subset is public; **release not verified** = described in a paper but no confirmed official dataset download was found.




## Papers

### Survey
- A review of deep learning in dentistry
  [[pdf]](https://www.sciencedirect.com/science/article/pii/S092523122300752X)
  - Chenxi Huang, Jiaji Wang, Shuihua Wang, Yudong Zhang. *Neurocomputing 2023*

- Artificial intelligence in stomatology: Innovations in clinical practice, research, education, and healthcare management
  [[paper]](https://pmc.ncbi.nlm.nih.gov/articles/PMC12549346/)
  - Reviews AI applications in clinical care, research, education, hospital management, and multi-agent collaboration. *Beijing Da Xue Xue Bao 2025*

- Leveraging large language models for patient instructions in dentistry: A systematic review and meta-analysis
  [[paper]](https://pubmed.ncbi.nlm.nih.gov/41368722/)
  - Rui Zhang, Yu Pan, Yushu Liu, Yinlong Deng, Edmond Ho Nang Pow. *Journal of Prosthodontics 2025*

- The role of large language models in dental diagnosis, decision-making, and communication: A systematic review
  [[paper]](https://pmc.ncbi.nlm.nih.gov/articles/PMC12865642/)
  - Taibe Tokgoz Kaplan, Gulbahar Erdinc Akyol. *Japanese Dental Science Review 2026*

- Multimodal large language models for oral lesion diagnosis: A systematic review of diagnostic performance and clinical utility
  [[paper]](https://pubmed.ncbi.nlm.nih.gov/41816099/)
  - Fatma E. A. Hassanein, Malik Alkabazi, Melek Tassoker, Yousra Ahmed, Suliman Alsaeed, Asmaa Abou-Bakr. *Frontiers in Oral Health 2026*

- A six-level clinical autonomy framework for artificial intelligence in dentistry
  [[paper]](https://www.frontiersin.org/journals/oral-health/articles/10.3389/froh.2026.1836492/full)
  - Sohaib Shujaat. *Frontiers in Oral Health 2026*

### LVLM

**2026**

- A multimodal vision-language model for comprehensive dental diagnosis and enhanced clinical practice (DentVLM)
  [[paper]](https://www.nature.com/articles/s41467-026-75718-x)
  [[preprint]](https://arxiv.org/abs/2509.23344)
  - Zijie Meng, Jin Hao, Xiwei Dai, et al. *Nature Communications 2026*

- Towards clinical-level interpretation of dental panoramic radiography using an instance-guided vision-language model (DentFound)
  [[paper]](https://www.nature.com/articles/s41551-026-01713-8)
  - Qikui Zhu, Yeyu Lin, Weitao Fu, et al. *Nature Biomedical Engineering 2026*

- Developing and evaluating multimodal large language model for orthopantomography analysis to support clinical dentistry (ToothXpert)
  [[paper]](https://pmc.ncbi.nlm.nih.gov/articles/PMC13006406/)
  [[model]](https://huggingface.co/jeffrey423/ToothXpert)
  - Xinyu Liu, Kuo Feng Hung, Weihao Yu, Ray Anthony W. T. Ng, Wuyang Li, Tianye Niu, Hui Chen, Yixuan Yuan. *Cell Reports Medicine 2026*

- DentalGPT: Incentivizing Multimodal Reasoning in Dentistry
  [[paper]](https://aclanthology.org/2026.findings-acl.135/)
  [[code]](https://github.com/FreedomIntelligence/DentalGPT)
  - Zhenyang Cai, Jiaming Zhang, Junjie Zhao, et al. *Findings of ACL 2026*

- A benchmark multimodal oro-dental dataset for large vision-language models
  [[paper]](https://www.nature.com/articles/s41597-026-07342-9)
  - Haoxin Lv, Ijazul Haq, Jin Du, et al. *Scientific Data 2026*

**2025**

- Towards Better Dental AI: A Multimodal Benchmark and Instruction Dataset for Panoramic X-ray Analysis
  [[pdf]](https://arxiv.org/abs/2509.09254)
  [[code]](https://github.com/isbrycee/OralGPT)
  - Jing Hao, Yuxuan Fan, Yanpeng Sun, Kaixin Guo, Lizhuo Lin, Jinrong Yang, Qi Yong H. Ai, Lun M. Wong, Hao Tang, Kuo Feng Hung. *NIPS2025*

- OralGPT-Omni: A Versatile Dental Multimodal Large Language Model
  [[pdf]](https://arxiv.org/abs/2511.22055)
  [[code]](https://github.com/isbrycee/OralGPT)
  - Jing Hao, Yuci Liang, Lizhuo Lin, Yuxuan Fan, Wenkai Zhou, Kaixin Guo, Zanting Ye, Yanpeng Sun, Xinyu Zhang, Yanqi Yang, Qiankun Li, Hao Tang, James Kit-Hon Tsoi, Linlin Shen, Kuo Feng Hung. *Arxiv*
    
- ArchMap: Arch-Flattening and Knowledge-Guided Vision Language Model for Tooth Counting and Structured Dental Understanding
  [[pdf]](https://arxiv.org/abs/2511.14336)
  - Bohan Zhang, Yiyi Miao, Taoyu Wu, Tong Chen, Ji Jiang, Zhuoxiao Li, Zhe Tang, Limin Yu, Jionglong Su. *Arxiv*

### Agentic AI

**2026**

- OralAgent: Integrating Reasoning, Tools, and Knowledge for Interactive Dental Image Analysis
  [[paper]](https://arxiv.org/abs/2605.27378)
  [[code]](https://github.com/isjinghao/OralAgent)
  - Jing Hao, Siyuan Dai, Yongxin Zhang, et al. *arXiv 2026*

- DentAgent: Evidence-Centric Multi-Agent Coordination for Multimodal Dental Reasoning
  [[paper]](https://arxiv.org/abs/2608.18878)
  - Zijie Meng, Xiwei Dai, Yixuan Tang, et al. *arXiv 2026*

- OPGAgent: An Agent for Auditable Dental Panoramic X-ray Interpretation
  [[paper]](https://arxiv.org/abs/2603.00462)
  [[code]](https://github.com/Zhaolin-Yu/OPGAgent)
  - Zhaolin Yu, Litao Yang, Ben Babicka, et al. *arXiv 2026*

- OralGPT-Plus: Learning to Use Visual Tools via Reinforcement Learning for Panoramic X-ray Analysis
  [[paper]](https://openaccess.thecvf.com/content/CVPR2026/html/Fan_OralGPT-Plus_Learning_to_Use_Visual_Tools_via_Reinforcement_Learning_for_CVPR_2026_paper.html)
  [[code]](https://github.com/isjinghao/OralGPT)
  - Yuxuan Fan, Jing Hao, Hong Chen, Jiahao Bao, Yihua Shao, Yuci Liang, Kuo Feng Hung, Hao Tang. *CVPR 2026*

### Segmentation

**2024**

- Sparse Anatomical Prompt Semi-Supervised Learning with Masked Image Modeling for CBCT Tooth Segmentation
  [[pdf]](https://arxiv.org/abs/2402.04587)
  - Pengyu Dai, Yafei Ou, Yang Liu, Yue Zhao. *ISBI 2024*
    
- Fully automatic integration of dental CBCT images and full-arch intraoral impressions with stitching error correction via individual tooth segmentation and identification
  [[pdf]](https://www.sciencedirect.com/science/article/pii/S1361841524000215)
  - Tae Jun Jang, Hye Sun Yun, Chang Min Hyun, Jong-Eun Kim, Sang-Hwy Lee, Jin Keun Seo. *MIA*

 - USCT: Uncertainty-regularized symmetric consistency learning for semi-supervised teeth segmentation in CBCT
   [[pdf]](https://www.sciencedirect.com/science/article/pii/S1746809424000909)
   - Yixin Jing, Jie Liu, Weifan Liu, Zhicheng Yang, ZhongWei Zhou, Zekuan Yu. *Biomedical Signal Processing and Control*

**2023**
 
- Robust Hybrid Learning for Automatic Teeth Segmentation and Labeling on 3D Dental Models
  [[pdf]](https://ieeexplore.ieee.org/abstract/document/10169899)
  - Shangxuan Li, Chichi Li, Yu Du, Li Ye, Yanshu Fang, Cheng Wang, Wu Zhou. *MICCAI 2023*
    
- 3D Tooth Mesh Segmentation with Simplified Mesh Cell Representation
  [[pdf]](https://ieeexplore.ieee.org/abstract/document/10230650/citations#citations)
  [[code]](https://github.com/ananyajana/tooth_mesh_seg)
  - Ananya Jana, Hrebesh Molly Subhash, Dimitris Metaxas. *ISBI 2023 oral*
    
- Toothsegnet: Image Degradation Meets Tooth Segmentation in CBCT Images
  [[pdf]](https://ieeexplore.ieee.org/abstract/document/10230557)
  - Jiaxiang Liu, Tianxiang Hu, Yang Feng, Wanghui Ding, Zuozhu Liu. *ISBI 2023*
    
- Dental Anatomy Segmentation from Cone Beam CT Images
  [[pdf]](https://ieeexplore.ieee.org/abstract/document/10230393)
  - Minhui Tan, Yu Fang, Lei Ma, Yu Zhang, Zhiming Cui, Dinggang Shen. *ISBI 2023*

- GRAB-Net: Graph-Based Boundary-Aware Network for Medical Point Cloud Segmentation
  [[pdf]](https://ieeexplore.ieee.org/abstract/document/10093984)
  - Yifan Liu, Wuyang Li, Jie Liu, Hui Chen, Yixuan Yuan. *TMI*
    
- Transformer-Based Tooth Segmentation, Identification and Pulp Calcification Recognition in CBCT
  [[pdf]](https://link.springer.com/chapter/10.1007/978-3-031-43904-9_68)
  - Yiwei Wang, Wenjun Xia, Zhennan Yan, Liang Zhao, Xiaohe Bian, Chang Liu, Zhengnan Qi, Shaoting Zhang, Zisheng Tang. *MIA*
   
- Root canal treatment planning by automatic tooth and root canal segmentation in dental CBCT with deep multi-task feature learning
  [[pdf]](https://www.sciencedirect.com/science/article/pii/S1361841523000117)
  - Yiwei Wang, Wenjun Xia, Zhennan Yan, Liang Zhao, Xiaohe Bian, Chang Liu, Zhengnan Qi, Shaoting Zhang, Zisheng Tang. *MIA*
  
- WITS: Weakly-supervised individual tooth segmentation model trained on box-level labels
  [[pdf]](https://www.sciencedirect.com/science/article/pii/S003132032200454X)
  [[code]](https://github.com/ruicx/Individual-Tooth-Segmentation-with-Rectangle-Labels)
  - Ruicheng Xie, Yunyun Yang, Zhaoyang Chen. *PR*

- Teeth U-Net: A segmentation model of dental panoramic X-ray images for context semantics and contrast enhancement
  [[pdf]](https://www.sciencedirect.com/science/article/pii/S0010482522010046)
  - Senbao Hou, Tao Zhou, Yuncan Liu, Pei Dang, Huiling Lu, Hongbin Shi. *Computers in Biology and Medicine*

- A fine-grained orthodontics segmentation model for 3D intraoral scan data
  [[pdf]](https://www.sciencedirect.com/science/article/pii/S0010482523012866)
  [[code]](https://github.com/MIVRC/Fast-TGCN)
  - Juncheng Li, Bodong Cheng, Najun Niu, Guangwei Gao, Shihui Ying, Jun Shi, Tieyong Zeng. *Computers in Biology and Medicine*
  
- 3D tooth segmentation in cone-beam computed tomography images using distance transform
  [[pdf]](https://www.sciencedirect.com/science/article/pii/S174680942200578X)
  - Somayeh Kakehbaraei, Roghayyeh Arvanaghi, Hadi Seyedarabi, Farzad Esmaeili, Ali Taghavi Zenouz. *Biomedical Signal Processing and Control*
 
- Deep-Learning-Based Segmentation of Individual Tooth and Bone With Periodontal Ligament Interface Details for Simulation Purposes
  [[pdf]](https://ieeexplore.ieee.org/abstract/document/10256039)
  [[code]](https://github.com/diku-dk/AutoJawSegment)
  - Peidi Xu, Torkan Gholamalizadeh, Faezeh Moshfeghifar, Sune Darkner, Kenny Erleben. *IEEE Access*

- Semantic Segmentation on Panoramic Dental X-Ray Images Using U-Net Architectures
  [[pdf]](https://ieeexplore.ieee.org/abstract/document/10477346)
  - Rafiatul Zannah, Mubtasim Bashar, Rahil Bin Mushfiq, Amitabha Chakrabarty, Shahriar Hossain, Yong Ju Jung. *IEEE Access*

- Multi-level uncertainty aware learning for semi-supervised dental panoramic caries segmentation
  [[pdf]](https://www.sciencedirect.com/science/article/pii/S0925231223003193)
  [[code]](https://github.com/Zzz512/MLUA)
  - Xianyun Wang, Sizhe Gao, Kaisheng Jiang, Huicong Zhang, Linhong Wang, Feng Chen, Jun Yu, Fan Yang. *Neurocomputing*

**2022**
- 3D Tooth Instance Segmentation Learning Objectness and Affinity in Point Cloud
  [[pdf]](https://dl.acm.org/doi/full/10.1145/3504033)
  - Yan Tian, Yujie Zhang, Wei-Gang Chen, Dongsheng Liu, Huiyan Wang, Huayi Xu, Jianfeng Han, Yiwen Ge. *TOMM*

- A fully automatic AI system for tooth and alveolar bone segmentation from cone-beam CT images
  [[pdf]](https://www.nature.com/articles/s41467-022-29637-2)
  [[code]](https://github.com/ErdanC/Tooth-and-alveolar-bone-segmentation-from-CBCT)
  - Zhiming Cui, Yu Fang, Lanzhuju Mei, Bojun Zhang, Bo Yu, Jiameng Liu, Caiwen Jiang, Yuhang Sun, Lei Ma, Jiawei Huang, Yang Liu, Yue Zhao, Chunfeng Lian, Zhongxiang Ding, Min Zhu, Dinggang Shen. *Nature Communications*

### Registration
**2024**
- Automatic 3D Registration of Dental CBCT and Face Scan Data using 2D Projection Images
  [[pdf]](https://arxiv.org/abs/2305.10132)
  - Hyoung Suk Park, Chang Min Hyun, Sang-Hwy Lee, Jin Keun Seo, Kiwan Jeon. *IEEE Access*
    
**2023**
- A Revised Approach to Orthodontic Treatment Monitoring From Oralscan Video
  [[pdf]](https://ieeexplore.ieee.org/abstract/document/10264061)
  - Yan Tian, Guotang Jian, Jialei Wang, Hong Chen, Lei Pan, Zhaocheng Xu, Jianyuan Li, Ruili Wang. *JBHI*

- Automatic registration of dental CT and 3D scanned model using deep split jaw and surface curvature
  [[pdf]](https://www.sciencedirect.com/science/article/pii/S0169260723001335)
  - Minchang Kim, Minyoung Chung, Yeong-Gil Shin, Bohyoung Kim. *Computer Methods and Programs in Biomedicine*

**2020**
- Automatic Registration Between Dental Cone-Beam CT and Scanned Surface via Deep Pose Regression Neural Networks and Clustered Similarities
  [[pdf]](https://ieeexplore.ieee.org/abstract/document/9133542)
  - Minyoung Chung, Jingyu Lee, Wisoo Song, Youngchan Song, Il-Hyung Yang, Jeongjin Lee , and Yeong-Gil Shin. *TMI*

### Construction 
**2024**

- NeBLa: Neural Beer-Lambert for 3D Reconstruction of Oral Structures from Panoramic Radiographs
  [[pdf]](https://ojs.aaai.org/index.php/AAAI/article/view/28241)
  [[code]](https://github.com/sihwa-park/nebla)
  [[video]](https://ojs.aaai.org/index.php/AAAI/article/view/28241/28478)
  - Sihwa Park, Seongjun Kim, Doeyoung Kwon, Yohan Jang, In-Seok Song, Seung Jun Baek. *AAAI 2024*
    
- DTR-Net: Dual-Space 3D Tooth Model Reconstruction From Panoramic X-Ray Images
  [[pdf]](https://ieeexplore.ieee.org/abstract/document/10264685)
  - Lanzhuju Mei, Yu Fang, Yue Zhao, Xiang Sean Zhou, Min Zhu, Zhiming Cui, Dinggang Shen. *TMI*

- Construction of unbiased dental template and parametric dental model for precision digital dentistry
  [[pdf]](https://arxiv.org/abs/2304.03556)
  [[code]](https://github.com/Marvin0724/Teeth_template)
  - Lei Ma, Jingyang Zhang, Ke Deng, Peng Xue, Zhiming Cui, Yu Fang, Minhui Tang, Yue Zhao, Min Zhu, Zhongxiang Ding, Dinggang Shen. *Biomedical Signal Processing and Control*
  
**2023**
- 3D Teeth Reconstruction from Panoramic Radiographs Using Neural Implicit Functions
  [[pdf]](https://link.springer.com/chapter/10.1007/978-3-031-43999-5_36)
  - Sihwa Park, Seongjun Kim, In-Seok Song, Seung Jun Baek. *MICCAI 2023*

- Deep learning-enabled 3D multimodal fusion of cone-beam CT and intraoral mesh scans for clinically applicable tooth-bone reconstruction
  [[pdf]](https://www.sciencedirect.com/science/article/pii/S2666389923001940)
  - Jiaxiang Liu, Jin Hao, Hangzheng Lin, Wei Pan, Jianfei Yang, Yang Feng, Gaoang Wang, Jin Li, Zuolin Jin, Zhihe Zhao, Zuozhu Liu. *Patterns*

- Geometry-Aware Attenuation Field Learning for Sparse-View CBCT Reconstruction
  [[pdf]](https://arxiv.org/abs/2303.14739)
  - Zhentao Liu, Yu Fang, Changjian Li, Han Wu, Yuan Liu, Zhiming Cui, Dinggang Shen. *Arxiv*

**2022**
- SNAF: Sparse-view CBCT Reconstruction with Neural Attenuation Fields
  [[pdf]](https://arxiv.org/abs/2211.17048)
  - Yu Fang, Lanzhuju Mei, Changjian Li, Yuan Liu, Wenping Wang, Zhiming Cui, Dinggang Shen. *Arxiv*
 
### Landmark
**2024**
- Anchor Ball Regression Model for large-scale 3D skull landmark detection
  [[pdf]](https://www.sciencedirect.com/science/article/abs/pii/S0925231223011748)
  [[code]](https://github.com/ithet1007/mmld_code)
  - Tao He, Guikun Xu, Li Cui, Wei Tang, Jie Long, Jixiang Guo. *Neurocomputing*

**2023**
- Unsupervised Domain Adaptation for Anatomical Landmark Detection
  [[pdf]](https://link.springer.com/chapter/10.1007/978-3-031-43907-0_66)
  [[code]](https://github.com/jhb86253817/UDA_Med_Landmark)
  - Haibo Jin, Haoxuan Che, Hao Chen. *MICCAI 2023*

### Arrangement/Alignment
**2026**
- MDTAN: An Automatic Tooth Arrangement Network Based on Multi-feature Fusion and Diffusion Model
  [[paper]](https://doi.org/10.1016/j.bspc.2026.109747)
  - Hong-an Li, Jiaxing Fu, Man Liu. *Biomedical Signal Processing and Control 2026*

- Tooth Alignment by Diffusion Model with Hierarchical Spatial Relationship Learning
  [[paper]](https://doi.org/10.1016/j.bspc.2026.109624)
  - Changkai Ji, Yusheng Liu, Sheng Wang, et al. *Biomedical Signal Processing and Control 2026*

- Automatic Orthodontic Treatment Planning Using Deep Learning
  [[paper]](https://doi.org/10.1007/s11633-025-1556-2)
  - Uroosa Sehar, Jing Xiong, Jiemei Zhai, Zeyang Xia. *Machine Intelligence Research 2026*

**2025**
- CLIK-Diffusion: Clinical Knowledge-informed Diffusion Model for Tooth Alignment
  [[paper]](https://doi.org/10.1016/j.media.2025.103746)
  [[code]](https://github.com/ShanghaiTech-IMPACT/CLIK-Diffusion)
  - Yulong Dou, Han Wu, Changjian Li, Chen Wang, Tong Yang, Min Zhu, Dinggang Shen, Zhiming Cui. *Medical Image Analysis 2025*

- Transformer-based Tooth Alignment Prediction with Occlusion and Collision Constraints
  [[paper]](https://openaccess.thecvf.com/content/ICCV2025/html/Dong_Transformer-based_Tooth_Alignment_Prediction_with_Occlusion_and_Collision_Constraints_ICCV_2025_paper.html)
  - Zhenxing Dong, Jiazhou Chen. *ICCV 2025*

- TEANet: Automated Tooth Extraction and Arrangement with Tooth-level Graph Spatial Transformation Network
  [[paper]](https://doi.org/10.1016/j.cmpb.2025.108985)
  - Xiaoshuang Li, et al. *Computer Methods and Programs in Biomedicine 2025*

- Differentiable Collision-Supervised Tooth Arrangement Network with a Decoupling Perspective
  [[paper]](https://doi.org/10.1109/TVCG.2025.3589215)
  [[preprint]](https://arxiv.org/abs/2409.11937)
  - Zhihui He, Chengyuan Wang, Shidong Yang, Li Chen, Yanheng Zhou, Shuo Wang. *IEEE Transactions on Visualization and Computer Graphics 2025*

- An automatic teeth arrangement method based on an intelligent optimization algorithm and the Frenet–Serret formula
  [[pdf]](https://www.sciencedirect.com/science/article/abs/pii/S174680942500117X)
  - Hong-an Li, Man Liu. *Biomedical Signal Processing and Control*

- A Dynamic Arrangement Framework for Automatic Tooth Alignment based on Orthodontic Rules
  [[paper]](https://doi.org/10.1016/j.cagd.2025.102436)
  - Yeying Fan, Guangshun Wei, Weijie Liu, Chuanxiang Yang, Chuanyun Fu, Wenping Wang, Yuanfeng Zhou. *Computer Aided Geometric Design 2025*

**2024**
- Collaborative Tooth Motion Diffusion Model in Digital Orthodontics
  [[pdf]](https://ojs.aaai.org/index.php/AAAI/article/view/27935)
  - Yeying Fan, Guangshun Wei, Chen Wang, Shaojie Zhuang, Wenping Wang, Yuanfeng Zhou. *AAAI 2024*

- TAPoseNet: Teeth Alignment based on Pose estimation via multi-scale Graph Convolutional Network
  [[pdf]](https://link.springer.com/chapter/10.1007/978-3-031-72390-2_30)
  [[code]](https://github.com/StardustandRain/TAPoseNet)
  - Qingxin Deng, Xunyu Yang, Minghan Huang, Landu Jiang, Dian Zhang. *MICCAI 2024*

- Improving Dental Alignment Accuracy with 3D Scanning and Deep Learning Model Optimization
  [[pdf]](https://ieeexplore.ieee.org/abstract/document/10822132)
  - Geunye Kim, Sena Lee, Juryeong Jeong, Yongkyu Jin, Sejung Yang. *BIBM 2024*
    
- A 3D dental model dataset with pre/post-orthodontic treatment for automatic tooth alignment
  [[pdf]](https://www.nature.com/articles/s41597-024-04138-7)
  [[code]](https://github.com/lcshhh/TADPM)
  - Shaofeng Wang, Changsong Lei, Yaqian Liang, Jun Sun, Xianju Xie, Yajie Wang, Feifei Zuo, Yuxin Bai, Song Li, Yong-Jin Liu. *scientific data*
 
- Automatic tooth arrangement with joint features of point and mesh representations via diffusion probabilistic models
  [[pdf]](https://www.sciencedirect.com/science/article/abs/pii/S016783962400027X)
  - Changsong Lei, Mengfei Xia, Shaofeng Wang, Yaqian Liang, Ran Yi,Yu-Hui Wen, Yong-Jin Liu. *Computer Aided Geometric Design*
   
- Neural Orthodontic Staging: Predicting Teeth Movements with a Transformer
  [[pdf]](https://ieeexplore.ieee.org/abstract/document/10764725)
  - Jiayue Ma, Jianwen Lou†, Borong Jiang, Hengyi Ye, Wenke Yu, Xiang Chen, Kun Zhou, Youyi Zheng. *TVCG*

- LETA: Tooth Alignment Prediction Based on Dual-branch Latent Encoding
  [[pdf]](https://ieeexplore.ieee.org/abstract/document/10566714)
  - Zefeng Shi, Zijie Meng, Ruizhe Chen, Yang Feng, Zeyu Zhao, Jin Hao, Bing Fang, Zuozhu Liu, Youyi Zheng. *TVCG*

**2023**
- A Semantic-Guided and Knowledge-Based Generative Framework for Orthodontic Visual Outcome Preview
  [[pdf]](https://link.springer.com/chapter/10.1007/978-3-031-43987-2_14)
  - Yizhou Chen, Xiaojun Chen. *MICCAI 2023*

**2022**
- Tooth Alignment Network Based on Landmark Constraints and Hierarchical Graph Structure
  [[pdf]](https://ieeexplore.ieee.org/abstract/document/9933028)
  - Chen Wang, Guangshun Wei, Guodong Wei, Wenping Wang, Yuanfeng Zhou. *TVCG*

**2020**
- TANet: Towards Fully Automatic Tooth Arrangement
  [[pdf]](https://link.springer.com/chapter/10.1007/978-3-030-58555-6_29)
  [[code]](https://github.com/ziyangyeh/TANet-Pytorch)
  - Guodong Wei, Zhiming Cui, Yumeng Liu, Nenglun Chen, Runnan Chen, Guiqing Li, Wenping Wang. *ECCV 2020*

- iOrthoPredictor: model-guided deep prediction of teeth alignment
  [[PDF]](https://dl.acm.org/doi/10.1145/3414685.3417771)
  [[code]](https://github.com/Lingchen-chen/iOrthopredictor)
  - Lingchen Yang, Zefeng Shi, Yiqian Wu, Xiang Li, Kun Zhou, Hongbo Fu, Youyi Zheng. *SIGGRAPH ASIA 2020*

- Malocclusion Treatment Planning via PointNet Based Spatial Transformation Network
  [[pdf]](https://link.springer.com/chapter/10.1007/978-3-030-59716-0_11)
  - Xiaoshuang Li, Lei Bi, Jinman Kim, Tingyao Li, Peng Li, Ye Tian, Bin Sheng, and Dagan Feng. *MICCAI 2020*

#### Complete Denture Tooth Arrangement

- AI-assisted Digital Tooth Arrangement System for Esthetic Optimization in Virtual Dentures
  [[paper]](https://pubmed.ncbi.nlm.nih.gov/42109357/)
  - Karthikeyan Vasudevan, Vijay Parmar, Gouri R. Reddy, et al. *Bioinformation 2026*
  - CNN trained on 2,500 clinically validated denture cases and evaluated on 40 edentulous patients; the software and code are not publicly identified.

- Complete Denture Tooth Arrangement Technology Driven by a Reconfigurable Rule
  [[paper]](https://doi.org/10.1371/journal.pone.0198252)
  - Rule-driven automatic arrangement using position, scaling, posture and contact constraints. *PLOS ONE 2018*

- Study on Digital Teeth Selection and Virtual Teeth Arrangement for Complete Denture
  [[paper]](https://doi.org/10.1016/j.cmpb.2017.11.022)
  - Personalized tooth selection, arrangement-line calculation and virtual tooth placement. *Computer Methods and Programs in Biomedicine 2018*

### Digital Smile Design
**2024**
- Dynasmile: Video-based smile analysis software in orthodontics
  [[pdf]](https://www.sciencedirect.com/science/article/pii/S2352711024003741)
  [[code]](https://github.com/dentistfrankchen/dynasmile)
  - Ke Chen, Lingling Qiu, Xianju Xie, Yuxing Bai. *SoftwareX*



## Projects
- [SlicerAutomatedDentalTools](https://github.com/DCBIA-OrthoLab/SlicerAutomatedDentalTools)
- [OralAgent](https://github.com/isjinghao/OralAgent)
- [OralGPT](https://github.com/isjinghao/OralGPT)
- [OPGAgent](https://github.com/Zhaolin-Yu/OPGAgent)
- [DentalGPT](https://github.com/FreedomIntelligence/DentalGPT)
- [ToothXpert](https://huggingface.co/jeffrey423/ToothXpert)
- [Dental Tool Agent](https://github.com/Paul-dumont/dental-tool-agent)
- [bone-finder](https://bone-finder.com/)
- [auto_tooth_arragement](https://github.com/yeyuxmf/auto_tooth_arrangement)
