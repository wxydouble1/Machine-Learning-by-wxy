*<u>上接P23 Lecture2的浅谈机器学习原理</u>*

---

# Why Deep Learning

![image-20230810174914379](WhyDeepLearning.assets/image-20230810174914379.png)

- 选large|H|,理想的状况Loss压得很低,但是坏处是理想和现实会有比较大的差距.

- 选smaller|H|,好处是理想和现实比较接近,但是Loss比较大.

> 鱼与熊掌可以兼得吗?------deep learning is answer.
>
> 希望能小的H里面找到最好的h使得Loss最小.

Reveiew: why hidden layer?

Piecewise Linear

![image-20230810175231582](WhyDeepLearning.assets/image-20230810175231582.png)

如果切的足够多,就能够逼近曲线.

可以用一个Hidden layer的neural network来制造出绿色线段.

绿色线段可以看作是常数项加上一堆蓝色线段.

![image-20230810175522827](WhyDeepLearning.assets/image-20230810175522827.png)

How to represent this function?

![image-20230810175553796](WhyDeepLearning.assets/image-20230810175553796.png)

hard sigmoid function 就是蓝色线段.

​	假设每一个neural network的每一个neural都可以制造出一个阶梯性的function.选择的activation function是sigmoid的话,可以透过不同的weight和bias制造出不同的sigmoid function.每制造出合适的sigmoid function就把他们统统加起来在加上一个常数项就可以产生任何的piecewise linear function(分段线性函数).然后用这个分段线性函数来逼近任何的function.

![image-20230811172358853](WhyDeepLearning.assets/image-20230811172358853.png)

另外一个来表示Hard Sigmoid function的方法呢就是ReLU function.ReLU叠加起来就能产生Hard Sigmoid

![image-20230811172501561](WhyDeepLearning.assets/image-20230811172501561.png)

![image-20230811172546809](WhyDeepLearning.assets/image-20230811172546809.png)



Deep is Better?

![image-20230811174427003](WhyDeepLearning.assets/image-20230811174427003.png)

Fat+short vs Thin+Tall

![image-20230811174510526](WhyDeepLearning.assets/image-20230811174510526.png)

![image-20230811174549957](WhyDeepLearning.assets/image-20230811174549957.png)

同样参数的条件下deep比fat好!

yes, one hidden layer can represent and function. 

however, using deep structure is more effective.

DEEP LEARNING 需要更少的参数和训练资料,真正的强项是更不容易overfitting.





















