# Efficient-Real-Time-Detection
Experiments with the aim of improving the computational efficiency of SOTA object detection algorithms.

DEIM ([DEIM: DETR with Improved Matching for Fast Convergence, Huang et al. 2024](https://arxiv.org/abs/2412.04234)) is the current SOTA in real-time object detection. When looking through the code base, I noticed that they don't make use of some of the modern improvements to transformer computational efficiency, such as GQA ([GQA: Training Generalized Multi-Query Transformer Models from Multi-Head Checkpoints, Ainslie et al. 2023](http://arxiv.org/abs/2305.13245)). These transformer improvements can significantly reduce memory overhead and speed up inference, making them particularly attractive for real-time systems. This work seeks to investigate whether the addition of these techniques is able to improve the SOTA in real-time object detection.

A large part of the code in this work comes from the repository that is associated with the publication, [DEIM](https://github.com/ShihuaHuang95/DEIM), as this work is a continuation of that work. Please star [DEIM](https://github.com/ShihuaHuang95/DEIM), and cite the original paper, if you use it in your work or find it otherwise useful:

```bibtex
@misc{huang2024deim,
      title={DEIM: DETR with Improved Matching for Fast Convergence},
      author={Shihua Huang, Zhichao Lu, Xiaodong Cun, Yongjun Yu, Xiao Zhou, and Xi Shen},
      year={2024},
      eprint={2412.04234},
      archivePrefix={arXiv},
      primaryClass={cs.CV}
}
```
The changes I made to his code are my own, and are not associated with the authors or publishers of the original work.