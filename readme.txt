
dataset: https://www.kaggle.com/ssarkar445/covid-19-xray-and-ct-scan-image-dataset
citation: https://data.mendeley.com/datasets/2fxz4px6d8/4

the file contains the following structure:

MODELS
  |
  |- classifier-(the weights as a pth file to preload and execute if we need to train further)
  |
  |-ML-Algos-(the weights file and ipynb, the ipynb file which contains both PCA on flattened output and first fully connected embedding)

Hyperparameters of the models are mentioned in hyperparams.txt	

once inside classifier folder of any model:
	load the model using net = torch.load("modelname_final.pth") and we can run the jupyter notebook's other cells