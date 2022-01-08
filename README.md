# glmhmm
This package provides flexible and easy-to-use code for fitting Generalized Linear Models (GLMs), Hidden Markov Models (HMMs), and combination GLM-HMMs (also known as Input-Output HMMs or IO-HMMs). The GLM code include options for fitting observational data of either Bernoulli or Multinomial distributions. HMM inference is done using the Expectation Maximization (EM) algorithm, with an optional mode for performing deterministic-annealing EM (DAEM), which is useful for hard to fit datasets.   

### Package Contents

#### glmhmm
* glm.py: GLM class fitting code
* hmm.py: HMM class fitting code
* glm-hmm.py: GLM-HMM class fitting code
* init_params.py: a script for defining initialization options for different model parameters
* observations.py: a script for defining distribution options for GLM observations
* utils.py: a script containing miscellaneous helper functions (more still to come)
* visualize.py: a script containing plotting and post-fitting analysis functions (more still to come)


#### examples
* fit-glm.ipynb: a simple example of fitting a GLM to simulated data
* fit-hmm.ipynb: a simple example of fitting an HMM to simulated data
* fit-hmm-DAEM.ipynb: an example illustrating the benefits of deterministic annealing EM (DAEM), with a comparison to traditional EM
* fit-glm-hmm.ipynb: an example of fitting GLM-HMMs to simulated data 

#### figures
##### folders
* data: a folder includeing pre-formatted design matrices and choice behavior for fitting the three mouse data sets described in [Bolkan, Stone et al 2021](https://www.biorxiv.org/content/10.1101/2021.07.23.453573v1)
* matlab: a folder containing MATLAB scripts used for fitting the psychometric curve plots shown in [Bolkan, Stone et al 2021](https://www.biorxiv.org/content/10.1101/2021.07.23.453573v1)
* fit models: a folder containing the model objects from several models fit during the figure generation process. 

##### notebooks 
Each jupyter notebook recreates the plots from a specified figure in [Bolkan, Stone et al 2021](https://www.biorxiv.org/content/10.1101/2021.07.23.453573v1)
* fig4.ipynb: a notebook describing how to fit a GLM to real data and recreating the plots from Figure 4
* fig5.ipynb: a notebook comparing model performance between a standard Bernoulli GLM and a 3-state GLM-HMM, as seen in Figure 5
* fig6.ipynb: a notebook describing how to fit a 3-state GLM-HMM to real data and recreating the plots from Figure 6
* fig7.ipynb: a notebook demonstrating statistical analyses to describe how the three states identified by the GLM-HMM manifest in the data and recreating the plots from Figure 7
* extdatafig7: a notebook detailing model selection and control analyses and recreating the plots from Extended Data Figure 7
* extdatafig8: a notebook demonstrating how model simulations recapitulate characteristics of the real data and recreating the plots from Extended Data Figure 8
* extdatafig9: a notebook showing how individual mice occupy different states for each session that they participate in the task and recreating the plots from Extended Data Figure 9

### Installation
For easy installation, download the code using the link above or type the following into a terminal window:
```
git clone https://github.com/irisstone/glmhmm.git
```
For convenience, we recommend setting up a virtual environment before running the code, to avoid any unpleasant version control issues or interactions with other projects you're working on. See the env.yml file for configuration details. Note the package requires python 3.7 to run.  
