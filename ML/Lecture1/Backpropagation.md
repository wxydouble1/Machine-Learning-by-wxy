# Gradient Descent-Backpropagation

![image-20230723195924517](Backpropagation.assets/image-20230723195924517.png)

---

#### Chain Rule(链式法则)

Case 1  (链式法则)
$$
y=g(x)
$$

$$
z=h(y)
$$

$$
Δx->Δy->Δz
$$

$$
dz/dx = dz/dy * dy/dx
$$

Case 2 (多元函数微分)

![image-20230723200951331](Backpropagation.assets/image-20230723200951331.png)

现在回到Backpropagation,先考虑某一个neuron:

![image-20230723201342732](Backpropagation.assets/image-20230723201342732.png)

![image-20230723222347633](Backpropagation.assets/image-20230723222347633.png)

sForward pass: 计算出所有的 **∂z/∂w** 

Backward pass: 对所有的激活函数输入的z计算出所有的 **∂c/∂z** 

最后得到 **∂C/∂w = ∂z/∂w * ∂C/∂z**

---

####  Backpropagation -Forward pass

![image-20230723222922793](Backpropagation.assets/image-20230723222922793.png)

![image-20230723222941184](Backpropagation.assets/image-20230723222941184.png)

---

#### Backpropagation - Backward pass

![image-20230723223122885](Backpropagation.assets/image-20230723223122885.png)

##### ∂c/∂z' 和∂c/∂z'' 怎么算呢, 假设他们已经算出来了

![image-20230723223334301](Backpropagation.assets/image-20230723223334301.png)

从另外一个视角看待这个式子:

![image-20230723223404685](Backpropagation.assets/image-20230723223404685.png)

##### 那如何算出∂C/∂z'和∂C/∂z''呢?

![image-20230723223536472](Backpropagation.assets/image-20230723223536472.png)

###### Case 1. Output Layer

![image-20230723223648361](Backpropagation.assets/image-20230723223648361.png)

###### Case 2. Not Output Layer

######  溯源到output layer![image-20230723223825444](Backpropagation.assets/image-20230723223825444.png)

###### actually operation: 

![image-20230723223933088](Backpropagation.assets/image-20230723223933088.png)

###### 从z5, z6 开始算往前传递:

![image-20230723224141642](Backpropagation.assets/image-20230723224141642.png)

###### 建立反向的神经网络:

![image-20230723224258339](Backpropagation.assets/image-20230723224258339.png)

##### Summary:

![image-20230723224609970](Backpropagation.assets/image-20230723224609970.png)

### **∂C/∂w = ∂z/∂w * ∂C/∂z**

