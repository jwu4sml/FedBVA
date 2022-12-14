# FedBVA
This is the official implementation of "Adversarial Robustness through Bias Variance Decomposition: A New Perspective for Federated Learning" (CIKM'22). 


## Requirements
* Python 3.6
* numpy==1.18.1
* torch==1.4.0
* torchvision==0.5.0


## Training and testing
For robust federated learning on MNIST image data set with IID setting, please run
```
python main.py
```

## Details
* utils: hyper-parameter setting (params.py) and decentralized data sampling (sampling.py)
* models: our decentralized learning algorithm, including client update and server update
* data: image data set (e.g., MNIST, Fashion-MNIST, Cifar10 and Cifar100) could be downloaded automatically from torchvision package
* save: we use the same random model initialization for all the experiments, blackbox attack models need to be pretrained


## Acknowledgement
This is the latest source code of **FedBVA**. If you find that it is helpful for your research, please consider to cite our paper:

```
@inproceedings{zhou2020adversarial,
  title={Adversarial Robustness through Bias Variance Decomposition: A New Perspective for Federated Learning},
  author={Zhou, Yao and Wu, Jun and Wang, Haixun and He, Jingrui},
  booktitle={Proceedings of the 31th ACM International Conference on Information and Knowledge Management},
  year={2022}
}
```
