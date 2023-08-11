# Classification

#### *Classification as Regression*

- Regression

  ![image-20230806105139949](Classification.assets/image-20230806105139949.png)

- Classification as regression

  ![image-20230806105204075](Classification.assets/image-20230806105204075.png)



##### 将Class用one-hot vector(独热编码)来表示

![image-20230806105624921](Classification.assets/image-20230806105624921.png)

 输出三个数值的神经网络

![image-20230806105740946](Classification.assets/image-20230806105740946.png)

Regression和Classification

![image-20230806110237880](Classification.assets/image-20230806110237880.png)

y------->y' 要经过一个softmax的过程,目的是为了将任意的y的值分标准化到0~1之间.

##### softmax的过程是:

$$
y'_i = \frac{exp(y_i)}{Σ_jexp(y_i)}
$$

![image-20230806111651553](Classification.assets/image-20230806111651553.png)

> 当只有两个class的时候取sigmoid

---

#### Loss of Classification

当然可以用MSE(均方差)来计算Loss,但是有一个更常用的办法就是Cross-entropy(交叉熵)

![image-20230806111842988](Classification.assets/image-20230806111842988.png)

**`Minimizing cross-entropy is equivalent to maximizing likelihood.`**

Cross-entropy比MSE更加适合用在Classification上.

> softmax内嵌在Cross-entropy里面,不需要再加一次softmax



##### 为什么交叉熵更好呢?

MSE可能会在大Loss的地方卡住,而cross-entropy在大Loss的地方有斜率的,不会卡住.

![image-20230806113633995](Classification.assets/image-20230806113633995.png)

