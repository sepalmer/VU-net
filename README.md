# VU-net
code repository for NeurIPS 2022 paper: Learning low-dimensional generalizable natural features from retina using a U-net
Please cite as: 

@inproceedings{wang2022learning,title={Learning low-dimensional generalizable natural features from retina using a U-net},author={Siwei Wang and Benjamin Hoshal and Elizabeth A de Laittre and Olivier Marre and Michael Berry and Stephanie Palmer},booktitle={Advances in Neural Information Processing Systems},editor={Alice H. Oh and Alekh Agarwal and Danielle Belgrave and Kyunghyun Cho},year={2022},url={https://openreview.net/forum?id=bdfJCeWDKUB }}

model definition: vunet_def.py

Demo usage and data processing blocks of 
variational U-net : [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://github.com/sepalmer/VU-net/blob/main/VUnet_demo.ipynb)

We first reverse engineer the retinal encoding process (reconstruct movie clips from their corresponding retinal activity)

![alt text](https://github.com/sepalmer/VU-net/blob/main/fish_truthvspred.gif)

![alt text](https://github.com/sepalmer/VU-net/blob/main/leaf_truthvspred.gif)

![alt text](https://github.com/sepalmer/VU-net/blob/main/water_truthvspred.gif)

We found intermediate emerging background and motion separation learned by the U-net: 
![alt text](https://github.com/sepalmer/VU-net/blob/main/objectmotion.gif)

The above features result in "clean up" of background at penultimate decoding layers: 
![alt text](https://github.com/sepalmer/VU-net/blob/main/topactivatefeatures.gif)

We will release the accompanying data once we submit the experimental paper
