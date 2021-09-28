# SOP-U2Net

The code available in the Github https://github.com/xuebinqin/U-2-Net and the corresponding paper https://arxiv.org/pdf/2005.09007.pdf were used to implement Salient Object Detection using a nested U-Structure.   
Saliency Object Detection accurately identifies the most visually noticeable features in an image.   
The paper proposes 2 models for the U2-Net architecture (176.3 MB and 4.7 MB) to enable usage in different environments.  

The following libraries (as mentioned in the Github) are required to be downloaded before running the codes:-  

- Python 3.6
- numpy 1.15.2
- scikit-image 0.14.0
- python-opencv PIL 5.2.0
- PyTorch 0.4.0
- torchvision 0.2.1
- glob  

DUTS-TR (or any other relevant) dataset can be downloaded for training and testing purpose.

1. model/u2net.py- The U2-net architecture is specified here with a ReSidual U-block (RSU) on the bottom level and a U-Net like structure in the top level.   
2. u2net_train.py- This file can be run to train the model. The model name and directory of training dataset folder can be specified from lines 49-53. (The pre-trained model and weights can also be directly downloaded from https://drive.google.com/file/d/1ao1ovG1Qtx4b7EoskHXmi2E9rp5CHLcZ/view . The predicted saliency maps for datasets SOD, ECSSD, DUT-OMRON, PASCAL-S, HKU-IS and DUTS-TE can be found in https://drive.google.com/file/d/1mZFWlS4WygWh1eVI8vK2Ad9LrPq4Hp5v/view )
3. u2net_test.py- This file can be used for trianing. The model name and image paths can be set from lines 57-63.  
  

  
The resulting images can be found in test_data/u2net_results.
