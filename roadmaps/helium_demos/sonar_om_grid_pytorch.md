# Helium - "OpenMined Grid" Prototype - PyTorch

<b>Background:</b> One of Sonar's main value propositions to the OpenMined ecosystem is the ability to create a marketplace for the training of ML models. This is a hybrid market for compute and data, as both the available computing power AND the available training data is distributed throughout the marketplace.

In this work, we wish to make independent progress on building the "compute marketplace" functionality of Sonar, such that spare GPU time can be bought and sold in the marketplace for the purpose of training deep neural networks.

### Part 1: User Stories

* <b>User Story A:</b> As an <b>AI Researcher</b> I want the ability to submit un-trained Neural Models to be trained by members of the OpenMined Grid. Furthermore, instead of renting access to a specific machine, I instead want to push my model to a queue which automatically allocates my model to a machine of the appropriate size and cost given my constraints. I should be able to BOTH submit a model to this queue AND receive the trained mode from the queue in a Jupyter Notebook. Finally, in this setup, I am also submitting all training data for the model to be trained on alongside the model to be trained. I provide the model, the training data, and I am willing to pay only for the compute power to train the model.
* <b>User Story B:</b> As a <b>GPU Owner</b>, I want the ability to rent out spare time on my GPU to the OpenMined grid, such that I can earn a passive income in a secure way facilitating the training of Machine Learning models. I'm interested in doing this because while I love using my GPU, most of the time I don't use it, and when I do I (frankly) wish that I had 10 GPUs. I'm interested in participating in the OpenMined platform because I want to rent out the use of my 1 GPU so that I can occasionally have access to 10 or 100 at a time when I'm doing my research. It is my hope that I will still break even on the cost/revenue of this tradeoff while giving me the flexibility to scale up compute as needed to support my projects.

### Part 2: Mockup

The following notebook shows an example of how OpenMined Grid could work. However, while the code is plausible, please consider it only for inspiration. Furthermore, the model in the notebook uses PySyft for Machine Learning, whereas this ticket uses an external framework.

* [Mockup Notebook](https://github.com/OpenMined/PySonar/blob/master/notebooks/OpenMined%20Grid%20Mockup.ipynb)

### Part 3: Acceptance Criteria

[PySonar: Epic - OpenMind Grid Prototype](https://github.com/OpenMined/PySonar/issues/43)
* [Issue 30](https://github.com/OpenMined/Sonar/issues/30) - OpenMind Grid Smart Contract
* [Issue 44](https://github.com/OpenMined/PySonar/issues/44) - OpenMined Grid - PyTorch Demo
