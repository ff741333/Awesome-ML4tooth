# Awesome-ML4tooth

If you have any problems, suggestions or improvements, please submit the issue or PR.

## Contents
* [Datasets](#datasets)
* [Papers](#papers)
  * [Survey](#survey)
  * [Segmentation](#Segmentation)
  * [Registration](#Registration)
  * [Construction](#Construction)
* [Projects](#projects)

## Datasets

| Dataset                   | Time     | Number |  Format   | Institudes | Tasks |
|---------------------------|----------|--------|-----------|------------| ----- |
| [STS-3D](https://tianchi.aliyun.com/competition/entrance/532087/introduction) | 2023 | 1084 | 3D CBCT | / | Segmentation |
| [STS-2D](https://tianchi.aliyun.com/competition/entrance/532086/introduction) | 2023 | 9500  | 2D X-ray | / | Segmentation |
| [DC1000](https://github.com/Zzz512/MLUA) | 2023 | 1000  | 2D X-ray | / | Segmentation |
| [3DTeethSeg22&Teeth3DS](https://github.com/abenhamadou/3DTeethSeg22_challenge) | 2022 | 1800 | 3D intra-oral scans | / | Segmentation |
| [Shining3D](https://drive.google.com/drive/folders/1fx9_KVEugZxbO3aTdwdfVTGf87_9FoLx) | 2020 | 210 | 3D intra-oral scans | / | Segmentation |




## Papers

### Survey
- A review of deep learning in dentistry
  [[pdf]](https://www.sciencedirect.com/science/article/pii/S092523122300752X)
  - Chenxi Huang, Jiaji Wang, Shuihua Wang, Yudong Zhang. *Neurocomputing2023*


### Segmentation

**2024**

- Fully automatic integration of dental CBCT images and full-arch intraoral impressions with stitching error correction via individual tooth segmentation and identification
  [[pdf]](https://www.sciencedirect.com/science/article/pii/S1361841524000215)
  - Tae Jun Jang, Hye Sun Yun, Chang Min Hyun, Jong-Eun Kim, Sang-Hwy Lee, Jin Keun Seo. *MIA*

 - USCT: Uncertainty-regularized symmetric consistency learning for semi-supervised teeth segmentation in CBCT
   [[pdf]](https://www.sciencedirect.com/science/article/pii/S1746809424000909)
   - Yixin Jing, Jie Liu, Weifan Liu, Zhicheng Yang, ZhongWei Zhou, Zekuan Yu. *Biomedical Signal Processing and Control*

- Sparse Anatomical Prompt Semi-Supervised Learning with Masked Image Modeling for CBCT Tooth Segmentation
  [[pdf]](https://arxiv.org/abs/2402.04587)
  - Pengyu Dai, Yafei Ou, Yang Liu, Yue Zhao. *Arxiv*

**2023**
 
- Robust Hybrid Learning for Automatic Teeth Segmentation and Labeling on 3D Dental Models
  [[pdf]](https://ieeexplore.ieee.org/abstract/document/10169899)
  - Shangxuan Li, Chichi Li, Yu Du, Li Ye, Yanshu Fang, Cheng Wang & Wu Zhou. *MICCAI*
    
- 3D Tooth Mesh Segmentation with Simplified Mesh Cell Representation
  [[pdf]](https://ieeexplore.ieee.org/abstract/document/10230650/citations#citations)
  [[code]](https://github.com/ananyajana/tooth_mesh_seg)
  - Ananya Jana, Hrebesh Molly Subhash, Dimitris Metaxas. *ISBI oral*
    
- Toothsegnet: Image Degradation Meets Tooth Segmentation in CBCT Images
  [[pdf]](https://ieeexplore.ieee.org/abstract/document/10230557)
  - Jiaxiang Liu, Tianxiang Hu, Yang Feng, Wanghui Ding, Zuozhu Liu. *ISBI*
    
- Dental Anatomy Segmentation from Cone Beam CT Images
  [[pdf]](https://ieeexplore.ieee.org/abstract/document/10230393)
  - Minhui Tan, Yu Fang, Lei Ma, Yu Zhang, Zhiming Cui, Dinggang Shen. *ISBI*

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
  - Zhiming Cui, Yu Fang, Lanzhuju Mei, Bojun Zhang, Bo Yu, Jiameng Liu, Caiwen Jiang, Yuhang Sun, Lei Ma, Jiawei Huang, Yang Liu, Yue Zhao, Chunfeng Lian, Zhongxiang Ding, Min Zhu & Dinggang Shen. *Nature Communications*

### Registration
**2023**
- A Revised Approach to Orthodontic Treatment Monitoring From Oralscan Video
  [[pdf]](https://ieeexplore.ieee.org/abstract/document/10264061)
  - Yan Tian, Guotang Jian, Jialei Wang, Hong Chen, Lei Pan, Zhaocheng Xu, Jianyuan Li, Ruili Wang. *JBHI*

- Automatic registration of dental CT and 3D scanned model using deep split jaw and surface curvature
  [[pdf]](https://www.sciencedirect.com/science/article/pii/S0169260723001335)
  - Minchang Kim, Minyoung Chung, Yeong-Gil Shin, Bohyoung Kim. *Computer Methods and Programs in Biomedicine*
  
- Automatic 3D Registration of Dental CBCT and Face Scan Data using 2D Projection Images
  [[pdf]](https://arxiv.org/abs/2305.10132)
  - Hyoung Suk Park, Chang Min Hyun, Sang-Hwy Lee, Jin Keun Seo, Kiwan Jeon. *Arxiv*

**2020**
- Automatic Registration Between Dental Cone-Beam CT and Scanned Surface via Deep Pose Regression Neural Networks and Clustered Similarities
  [[pdf]](https://ieeexplore.ieee.org/abstract/document/9133542)
  - Minyoung Chung, Jingyu Lee, Wisoo Song, Youngchan Song, Il-Hyung Yang, Jeongjin Lee , and Yeong-Gil Shin. *TMI*

### Construction 
**2024**
- DTR-Net: Dual-Space 3D Tooth Model Reconstruction From Panoramic X-Ray Images
  [[pdf]](https://ieeexplore.ieee.org/abstract/document/10264685)
  - Lanzhuju Mei, Yu Fang, Yue Zhao, Xiang Sean Zhou, Min Zhu, Zhiming Cui, Dinggang Shen. *TMI*

  
**2023**
- 3D Teeth Reconstruction from Panoramic Radiographs Using Neural Implicit Functions
  [[pdf]](https://link.springer.com/chapter/10.1007/978-3-031-43999-5_36)
  - Sihwa Park, Seongjun Kim, In-Seok Song & Seung Jun Baek. *MICCAI*

- Deep learning-enabled 3D multimodal fusion of cone-beam CT and intraoral mesh scans for clinically applicable tooth-bone reconstruction
  [[pdf]](https://www.sciencedirect.com/science/article/pii/S2666389923001940)
  - Jiaxiang Liu, Jin Hao, Hangzheng Lin, Wei Pan, Jianfei Yang, Yang Feng, Gaoang Wang, Jin Li, Zuolin Jin, Zhihe Zhao, Zuozhu Liu. *Patterns*

- Construction of unbiased dental template and parametric dental model for precision digital dentistry
  [[pdf]](https://arxiv.org/abs/2304.03556)
  [[code]](https://github.com/Marvin0724/Teeth_template)
  - Lei Ma, Jingyang Zhang, Ke Deng, Peng Xue, Zhiming Cui, Yu Fang, Minhui Tang, Yue Zhao, Min Zhu, Zhongxiang Ding, Dinggang Shen. *Arxiv*

- Geometry-Aware Attenuation Field Learning for Sparse-View CBCT Reconstruction
  [[pdf]](https://arxiv.org/abs/2303.14739)
  - Zhentao Liu, Yu Fang, Changjian Li, Han Wu, Yuan Liu, Zhiming Cui, Dinggang Shen. *Arxiv*

**2022**
- SNAF: Sparse-view CBCT Reconstruction with Neural Attenuation Fields
  [[pdf]](https://arxiv.org/abs/2211.17048)
  - Yu Fang, Lanzhuju Mei, Changjian Li, Yuan Liu, Wenping Wang, Zhiming Cui, Dinggang Shen. *Arxiv*
## Projects


