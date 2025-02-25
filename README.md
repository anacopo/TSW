## Summary

This work presents different visualisation techniques that help in the explainability of visual transformers(ViTs). Visualization techniques play a crucial role in enhancing the interpretability of ViTs by providing insights into the model’s decision making process. Following methods have been analyzed: Attention Rollout, Transition Attention Maps, Class Activation Maps(CAM), Layerwise Relevance Propagation(LRP) and Causal Explanations. They all try to give insightful details on the decisions of the model, but the ways in which they do this differ. We offer implementation of two such visualization methods, LRP and CAM and do a comparison of them by looking at different types of results that they produce. By alligning the results with human interpretability but also by comparing some quantitative results we conclude that LRP performs better than CAM. The report concludes with an overview of ongoing research directions aimed at improving the interpretability and explainability of ViTs

## Requirements

No requirements are other then a internet connection, a browser and a Google account are needed. The implementation is done in a Jupyter Notebook, which can be run in google colaboratory or kaggle. You need to set the runtime type to GPU.
The dependencies are already in the notebook and they can be installed directly within the notebook.
Execute the notebook cells in order.

## Dataset

The Pascal Visual Object Classes 2012 (VOC) validation dataset has been used.
You can download it directly from torchvision.

```
from torchvision.datasets import VOCSegmentation
import torchvision.transforms as T

dataset = VOCSegmentation(root='data', year='2012', image_set='val', download=True, transform=T.ToTensor())
```
## Results
### Visual Results
![image](https://github.com/user-attachments/assets/b7742a23-b3ec-4114-92fa-2de53fab45ab)

### Evaluation Metrics
![image](https://github.com/user-attachments/assets/89bf8413-b561-4659-83eb-251975ccfb3b)
![image](https://github.com/user-attachments/assets/0a159ee9-f07a-4a00-a31c-b991f6fdfc22)


