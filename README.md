# semi-supervised-learning-for-vessel-segmentation
The code of paper "A Self-training Framework for Semi-supervised Pulmonary Vessel Segmentation Using Interactive Annotation and Application in COPD Patients"

<div align="center">

<samp>

<h2> A Self-training Framework for Semi-supervised Pulmonary Vessel Segmentation Using Interactive Annotation and Application in COPD Patients </h1>

<h4> Yanan Wu, Meihuan Wang, Xin Du, Haowen Pang, Jiaxuan Xu, and Shouliang Qi# </h3>

</samp>   

</div>     
    
---

If you find our code or paper useful, please cite as (This paper will be updated later)

```bibtex
@article{wu2023two,
  title={Two-stage contextual transformer-based convolutional neural network for airway extraction from CT images},
  author={Wu, Yanan and Zhao, Shuiqing and Qi, Shouliang and Feng, Jie and Pang, Haowen and Chang, Runsheng and Bai, Long and Li, Mengqi and Xia, Shuyue and Qian, Wei and others},
  journal={Artificial Intelligence in Medicine},
  pages={102637},
  year={2023},
  publisher={Elsevier}
}
@article{wu2023transformer,
  title={Transformer-based 3D U-Net for pulmonary vessel segmentation and artery-vein separation from CT images},
  author={Wu, Yanan and Qi, Shouliang and Wang, Meihuan and Zhao, Shuiqing and Pang, Haowen and Xu, Jiaxuan and Bai, Long and Ren, Hongliang},
  journal={Medical \& Biological Engineering \& Computing},
  pages={1--15},
  year={2023},
  publisher={Springer}
}
```

---
## Abstract
 CT images.  

<p align="center">
<img src="graph abstract.png" alt="TransformerVessel" width="1000"/>
</p>


---
## Environment

- SimpleITK
- PyTorch
- numpy
- pandas
- scipy
- scikit-learn
- timm
- tqdm
- pickle

## Directory Setup
<!---------------------------------------------------------------------------------------------------------------->
In this project, we implement our method using the Pytorch library, the structure is as follows: 
 
- model_ds.py : 3D CoT module and double attention module.
- main.py : training the model in the provided dataset
- loss.py : the focal loss and dice loss are combined
- utils.py

---
## Dataset
1. The in-house dataset was provided by the hospital. 
2. The ISICDM dataset released in the ISICDM 2021 challenge and labeled by the challenge organizer.

---



## References
Code adopted and modified from:
1. CoTNet model
    - Paper [Contextual Transformer Networks for Visual Recognition](https://arxiv.org/pdf/2107.12292.pdf).
    - official pytorch implementation [Code](https://github.com/JDAI-CV/CoTNet.git).
2. double attention model
    - Paper [A^2-Nets: Double Attention Networks](https://proceedings.neurips.cc/paper_files/paper/2018/file/e165421110ba03099a1c0393373c5b43-Paper.pdf).
    - official pytorch implementation [Code](https://github.com/nguyenvo09/Double-Attention-Network.git).

---

## Contact
For any queries, please raise an issue or contact [Yanan Wu](mailto:yananwu513@gmail.com).

---
