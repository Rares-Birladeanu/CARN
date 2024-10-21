# Experiment Results

| Experiments                          | Test Acc. |
|--------------------------------------|-----------|
|  Version 1                           | 40.57%    |
|  Version 2                           | 55.27%    |
|  Version 3                           | 58.96%    |
|  Version 4                           | 62.82%    |
|  Version 5                           | 63.85%    |
|  Version 6                           | 62.40%    |

## Notes:
1. [Version 1](https://github.com/Rares-Birladeanu/CARN/blob/main/Tema_2/Version%201/Version_1.ipynb)
   - Added the mean = (0.5071, 0.4867, 0.4408) and standard deviation = (0.2675, 0.2565, 0.2761) specific for the CIFAR-100 dataset
2. [Version 2](https://github.com/Rares-Birladeanu/CARN/blob/main/Tema_2/Version%202/Version_2.ipynb)
   - Changed batch size to 32 and changed the optimizer to Adam with learning rate = 0.0001
4. [Version 3](https://github.com/Rares-Birladeanu/CARN/blob/main/Tema_2/Version%203/Version_3.ipynb)
   - Added a the ReduceLROnPlateau learning rate scheduler with reducing factor = 0.5 and patience = 3
5. [Version 4](https://github.com/Rares-Birladeanu/CARN/blob/main/Tema_2/Version%204/Version_4.ipynb)
   - Changed the optimizer to SGD, learning rate = 0.015, momentum = 0.9, weight decay = 5e-4, fused = True and increased epochs to 60
7. [Version 5](https://github.com/Rares-Birladeanu/CARN/blob/main/Tema_2/Version%205/version_5.ipynb)
   - Changed batch size to 64, added label smoothing = 0.25 to CrossEntropyLoss function, changed learning rate to 0.03 added nesterov=True  and changed the parameters for the scheduler: factor = 0.12, patience = 4
8. [Version 6](https://github.com/Rares-Birladeanu/CARN/blob/main/Tema_2/Version%206/Version%206.ipynb)
   - Added some image transforamtion : Random Rotation +- 15 and Random Horizontal Flip.

All the Configurations have been made starting from the baselin in a sequential order ( Version 2 is The same as Version 1 the only difference being the changes mentioned). 
