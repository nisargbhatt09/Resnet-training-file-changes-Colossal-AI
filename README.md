# Resnet-training-file-changes-Colossal-AI

In this Repository, there is a code to accelerate the resnet training and performance on the cifar10 dataset.
I am running this assignment on Google Colab. 
In the repository, to boost the training and to optimize the training process, colossal AI tools are being used.

To run this model on single gpu setup, the steps to execute are as followed.

Install the colossalAI library in pip 

```pip install colossalai```

Clone the GitHub repository

```git clone https://github.com/hpcaitech/ColossalAI.git```

**Note**
ColossalAI only works on Linux for now.

Going into the directory where resnet example

```cd examples/images/resnet```

run the given command

```colossalai run --nproc_per_node 1 train.py -c ./ckpt-fp32```

This will start the training, and make a checkpoint called ckpt-fp32.  *make sure you write 1 and not 2 in the given command*. 
There are 80 epochs to train.


After running this sequence of commands, the training will be started and done.
