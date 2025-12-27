# Advanced machine learning project github. Diffusion models and GANS
All the code to reproduce the results is located in the folder reproducibility. Make sure to run the code on a gpu if you want to sample new images as the forward passes are quite costly and can take quite some time on a CPU. generation can take anywhere between 10 seconds to a minute and 40s depending on the model generating.

# Simple out of the box method to reproduce the results directly if you have access to the Onyxia platform :

- Go to [datalab](https://datalab.sspcloud.fr/)
- Go to 'My services'
- Create a new notebook 'Vscode-pytorch-gpu'
- Clone this library inside the notebook
- Everything in the reproducibility folder should run directly (this should already be the case but do confirm that CUDA is available with torch.cuda.is_available()).

Most of the code was created with the assistance of LLMs, we adapted the construction blocks for the models used from the pytorch documentation then automated the writing of the code of the training loops, visualization helpers and auxiliary functions with the assistance of those LLMs. Most of our work was centered around building and adapting the mathematical theory, designing the architectures and analyze and interpret the results to know what to fix when needed (e.g. high frequency speckles, training instability etc...). No code was copy pasted from any other source. 
