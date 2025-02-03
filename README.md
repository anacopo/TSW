## Summary

This work presents different visualisation techniques that help in the explainability of visual transformers(ViTs). Visualization techniques play a crucial role in enhancing the interpretability of ViTs by providing insights into the model’s decision making process. Following methods have been analyzed: Attention Rollout, Transition Attention Maps, Class Activation Maps(CAM), Layerwise Relevance Propagation(LRP) and Causal Explanations. Two out of these five methods have been implemented: CAM and LRP. By applying different kind of evaluation techniques, LRP is the winner.

## Requirements

No requirements are other then a internet connection and a browser are needed. The implementation is done in a Jupyter Notebook, which can be run in google colaboratory or kaggle. You need to set the runtime type to GPU.

## Dataset

The Pascal Visual Object Classes 2012 (VOC) validation dataset has been used.
You can download it directly from torchvision.

```
from torchvision.datasets import VOCSegmentation
import torchvision.transforms as T

dataset = VOCSegmentation(root='data', year='2012', image_set='val', download=True, transform=T.ToTensor())
```
