# Tricks-in-Tensorflow 
### Hard to search the answers, because these are less frequently answered questions

**1.  【Prune the fully connected layers】 Pruning deep neural networks - tensorflow.ipynb**

This part is only about the tricks in pruning and stop gradient. (But they are hard to be searched online, few people have questioned about it) For the other tricks, at present, I didn't have time to summarize them and upload. You can keep an eye on this document and frequently check my updates if you are interested in AI and Quant.

### Such as：
![Image text](https://github.com/ThuAlexFang/Tricks-in-Tensorflow/blob/master/fig/1.PNG)
![Image text](https://github.com/ThuAlexFang/Tricks-in-Tensorflow/blob/master/fig/2.PNG)

**For more compare and experiment result, you can download the tensorflow.ipynb and have a look.**

**2.  【Fix some layers, only updates the other layers.】**

Why we need to only update some layers? In transfer learning, pre-training, or Decopuling (a SOTA method for long-tailed data), we need use this technic. And I think this technic may be a very common method to use in other experiment, frequently test this idea, you may find you things.

**Method 1 (Define the variable that is trainable)**
![Image text](https://github.com/ThuAlexFang/Tricks-in-Tensorflow/blob/master/fig/3.PNG)

**Attention**

1.If you didn't define it as trainable, the defalut setting is trainable. But you can define it as not trainable, to avoid training on this variable.

2.For the tf.constant variable, all of this variable is a constant, they can't be trained, no matter how you redefine it.


**Method 2 (Define the scope of layer that need to be trainable)**
![Image text](https://github.com/ThuAlexFang/Tricks-in-Tensorflow/blob/master/fig/4.PNG)

I think this part is quite clear, so far so good, no confusing part.

**Method 3 (Save the model and reload it)**

![Image text](https://github.com/ThuAlexFang/Tricks-in-Tensorflow/blob/master/fig/5.PNG)

This method is less frequently used and not conveinet. I not recommend to use it in this situation. 

**I think there are more and more answers can be found on the web. If I have sucked in other special problems & I fixed it & the answers are hard to find & I have time to update this page, I will update it latter...**
