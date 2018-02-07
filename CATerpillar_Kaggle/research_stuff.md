Docker might fail to write or remove folders etc. due to issue with Redhat/CentOS file system issues: 


https://www.kaggle.com/c/dogs-vs-cats-redux-kernels-edition/download/train.zip

https://www.kaggle.com/c/dogs-vs-cats-redux-kernels-edition/download/test.zip

the lasagne commit used requires theano==0.7

https://github.com/Lasagne/Lasagne/blob/9f591a5f3a192028df9947ba1e4903b3b46e8fe0/requirements.txt

#. theano 0.7 requires cuda 6.5 and cudnn 2:
#. for the oo solution, we need cudnn2, and cuda 6.5 / to avoid hassle of manual installation we can use 
https://gitlab.com/nvidia/cuda/blob/ubuntu14.04/7.0/devel/cudnn2/Dockerfile

alternatively, we can try with latest cuda and cudnn, but possibly it will fail !!

lasagne version should be around 0.1 from the looks, i need to install and check further, because its not clear from the code.
