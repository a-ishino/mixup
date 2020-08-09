# Train CIFAR10 with PyTorch

I'm playing with [PyTorch](http://pytorch.org/) on the CIFAR10 dataset.

## Prerequisites
- Python 3.6+
- PyTorch 1.0+

## Accuracy
| Model             | Acc.        | Acc. (mixup)|
| ----------------- | ----------- | ----------- |
| [VGG19](https://arxiv.org/abs/1409.1556)              | 93.82%      | 94.14%      |


## Learning rate adjustment
I manually change the `lr` during training:
- `0.1` for epoch `[0,200)`
- `0.01` for epoch `[200,250)`
- `0.001` for epoch `[250,300)`

Resume the training with `python main.py --resume --lr=0.01 --mixup`
