## Summary

This work presents different visualisation techniques of attention in visual transformers(ViTs). Visualization techniques play a crucial role in enhancing the interpretability of ViTs by providing insights into the model’s decision making process.

## Requirements

pip install einops

You can run this notebook in google colaboratory or kaggle and set the runtime type to GPU.

## Dataset

The Pascal Visual Object Classes (VOC) dataset has been used.
You can download it directly from torchvision

```
from torchvision.datasets import VOCSegmentation
import torchvision.transforms as T

dataset = VOCSegmentation(root='data', year='2012', image_set='val', download=True, transform=T.ToTensor())
```
