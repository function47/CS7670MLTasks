# CS7670 MLTasks

Train a NN on pytorch on CIFAR-10.

## Selection of NNs
A common selection is ResNet18 which is a built-in model of pytorch. However, an 18-layer model may be too large for this task. We could use ResNet-9 or even LeNet-5. However, since the dataloader is handling the data loads. I belive the different models will not affect the results. 

---

## Hyperparameters

The image loading in pytorch is handled by `torch.dataloader`. A few hyperparameters will affect the images loading processes. 

### Batch size 

Batch size is the number of samples used for updating the internal model parameters. 

### Sample approach
    1. Sequential vs shuffled sampler
    2. memory pinning
### Data parallelism
The dataloader allow user to define number of sub-processes as number of workers for handling dataset.

### Prefech factors

----


## References
Ofeidis, Iason, Diego Kiedanski, and Leandros Tassiulas. "An Overview of the Data-Loader Landscape: Comparative Performance Analysis." arXiv preprint arXiv:2209.13705 (2022).


