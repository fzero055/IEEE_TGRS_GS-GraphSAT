# IEEE_TGRS_GS-GraphSAT
Abstract— For hyperspectral image classification (HSIC), labeling samples is challenging and expensive due to high dimensionality and massive data, which limits the accuracy and stability of classification. 
To alleviate this problem, a greedy strategy guided graph self-attention network (GS-GraphSAT) is proposed. 
First, a graph self-attention (GSA) mechanism is designed by combining a multihead self-attention (MHSA) mechanism with the graph attention network (GAT), which can simultaneously consider the direct and indirect relationships between nodes and deeply analyze the intrinsic characteristics of nodes. 
Second, a multiattention fusion (MAF) module is developed, which utilizes multiscale convolution kernels and attention mechanisms to significantly enhance the network’s ability to extract local features from images at the pixel level, thereby further enriching the hierarchy and diversity of features.
Finally, a greedy training strategy (GTS) is proposed. 
During the training process, GTS accurately determines the optimal time to supplement samples by analyzing the changes in losses, thereby achieving a significant improvement in network classification performance with limited samples. 
Extensive experiments were conducted on four challenging datasets. 
The results demonstrate that the proposed method significantly outperforms other state-of-the-art methods in terms of classification accuracy and robustness. 
The performance improvement of overall accuracy (OA) can reach up to 1.70% in Houston 2013 (HT). 
[https://ieeexplore.ieee.org/abstract/document/10766621](https://ieeexplore.ieee.org/abstract/document/10766621)

# Environments
```
python = 3.7.0
torch = 1.10.1+cu113
torchaudio = 0.10.1+cu113
torchvision = 0.11.2+cu113
```
# How to use it?
Here an example experiment is given by using **Indian Pines**. Directly run **Main_IP.py** to produce the results. Please note that due to the randomness of the parameter initialization, the experimental results might have slightly different from those reported in the paper.

# Results
All the results presented here are referenced from the original paper.
| Dataset | OA (%) | AA (%) | Kappa (×100) |
| :----: |:------:|:------:|:---------:|
| Indian Pines  | 99.31  | 99.09  |   99.21   |
| Pavia University  | 99.56  | 99.31  |   99.41   |
| Longkou  | 98.92  | 95.90  |   98.57   |
| Houston 2013  | 98.80  | 98.73  |   98.70   |

# Citation
If you find this work interesting in your research, please kindly cite:

```
[1] F. Zhu, C. Shi, L. Wang and K. Shi, "A Greedy Strategy Guided Graph Self-Attention Network for Few-Shot Hyperspectral Image Classification,"
    in IEEE Transactions on Geoscience and Remote Sensing, vol. 62, pp. 1-20, 2024, Art no. 5539620, doi: 10.1109/TGRS.2024.3505539.
```

```
@ARTICLE{10766621,
  author={Zhu, Fei and Shi, Cuiping and Wang, Liguo and Shi, Kaijie},
  journal={IEEE Transactions on Geoscience and Remote Sensing}, 
  title={A Greedy Strategy Guided Graph Self-Attention Network for Few-Shot Hyperspectral Image Classification}, 
  year={2024},
  volume={62},
  number={},
  pages={1-20},
  doi={10.1109/TGRS.2024.3505539}}
```

# Acknowledgements
This code is constructed based on [CEGCN](https://github.com/qichaoliu/CNN_Enhanced_GCN), [WFCG](https://github.com/quanweiliu/WFCG). Many thanks to these scholars！
If you have any questions, please do not hesitate to contact me (Fei Zhu, 2022935750@qqhru.edu.cn or fzhu0826@163.com).
