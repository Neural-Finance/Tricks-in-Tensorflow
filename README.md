# Tricks-in-Tensorflow 
### Hard to search the answers, because these are less frequently answered questions

**1.  【Prune the fully connected layers】 Pruning deep neural networks - tensorflow.ipynb**

This part is only about the tricks in pruning and stop gradient. (But they are hard to be searched online, few people have questioned about it) For the other tricks, at present, I didn't have time to summarize them and upload. You can keep an eye on this document and frequently check my updates if you are interested in AI and Quant.

### Such as：
![Image text](https://github.com/ThuAlexFang/Tricks-in-Tensorflow/blob/master/fig/1.PNG)
![Image text](https://github.com/ThuAlexFang/Tricks-in-Tensorflow/blob/master/fig/2.PNG)

**2.  【Fix some layers, only updates the other layers.】**

Why we need to only update some layers? In transfer learning, pre-training, or Decopuling (a SOTA method for long-tailed data), we need use this technic. 

And I think this technic may be a very common method to use in other experiment, frequently test this idea, you may find you things.

**Method1:**
![Image text](https://github.com/ThuAlexFang/Tricks-in-Tensorflow/blob/master/fig/3.PNG)

**Method2:**
![Image text](https://github.com/ThuAlexFang/Tricks-in-Tensorflow/blob/master/fig/4.PNG)
