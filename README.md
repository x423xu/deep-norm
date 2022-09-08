# easy-deep
A toolkit for deep learning training, evaluation, testing, visualization and other affairs.

```
This is a toolkit to normalize the deep learning workflow. The idea is to create a prototype for my research code in deep learning. 

Each time when I am heading into a new research area, I have to reimplement involved codes and waste a whole bunch of time on repeated code works. For eample, I have to rewrite code to organize data, build models, test models and others. But in fact, the workflow for deep learning coding is pretty a stereotype. If the workflow can be itemized and formed into a prototype, many repeated works can be simplified. 

In my initial design, the deep learning workflow contains following parts:
    1. data organization
    2. model building
    3. model evaluation
    4. model testing
    5. results visualization

Data organization:
    1. The prototype only regulates data input type and output type. It should provide an abstract dataset parent class which lists all legal functions and variables.
    2. It should provide an abstract method for data preprocessing
Model building:
    1. For each user, it should register a task and then build models under the task. So the 'task' should be at the most top layer.
    2. The prototype provides an interface for model building.
Training and evaluation:
    1. For a researcher, the prototype should make the training process visible and understandable. A tool 'wandb' provides a transparent workflow for deep model training. It should be included.

    2. The logs for training should be detailed, so a log output interface should be included. The log format should be predefined and self-customizable.
    log: format, variables
Testing:
    1. To test model, a test interface include: model saved path, data 
```