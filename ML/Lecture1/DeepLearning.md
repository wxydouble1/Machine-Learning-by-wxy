# DeepLearning

*DeepLearning attracts lots of attention*

---

Ups and downs of DeepLearning

- 1958: Perceptron(linear model)

- 1969: Perceptron has limitation

- 1980s Multi-layer perceptron

  Do not have significant difference from DNN today

- 1986: Back propagation

  Usually more than 3 hidden layers is not helpful

- 1989: 1 hidden layer is "good enough”, why deep?

- 2006: RBM initialization (breakthrough)

- 2009: GPU

- 2011: Start to be popular in speech recognition

- 2012: win ILSVRC image competition

#### DeepLearning 三部曲

- Step 1: define a set of function (Neural Network)
- Step 2: goodness of function 
- Step 3: pick the best function

#### Step 1: Neural Network

![image-20230723183043308](DeepLearning.assets/image-20230723183043308.png)

怎么将神经连接起来呢?

Fully Connect Feedforward Network(全连接前向传播神经网络)![image-20230723183533439](DeepLearning.assets/image-20230723183533439.png)

将function集合起来就是function set

![image-20230723183633173](DeepLearning.assets/image-20230723183633173.png)

![image-20230723183901710](DeepLearning.assets/image-20230723183901710.png)

<u>*Deep = Many hidden layers*</u>

![image-20230723184120571](DeepLearning.assets/image-20230723184120571.png)

用Matrix Operation 来表示Network:

![image-20230723184608677](DeepLearning.assets/image-20230723184608677.png)

![image-20230723184629909](DeepLearning.assets/image-20230723184629909.png)

Hidden Layers: Feature extractor replacing 

Output Layer: Multi-class Classifier

![image-20230723184937183](DeepLearning.assets/image-20230723184937183.png)

EXAMPLE:

![image-20230723185230753](DeepLearning.assets/image-20230723185230753.png)

![image-20230723185246810](DeepLearning.assets/image-20230723185246810.png)

![image-20230723185255336](DeepLearning.assets/image-20230723185255336.png)

![image-20230723185354289](DeepLearning.assets/image-20230723185354289.png)

FAQ:![image-20230723185916847](DeepLearning.assets/image-20230723185916847.png)

#### Step 2: goodness of function

*Loss for an Example*

![image-20230723190351649](DeepLearning.assets/image-20230723190351649.png)

#### Step 3 

 用Gradient Descent来找minimize total loss

![image-20230723194044221](DeepLearning.assets/image-20230723194044221.png)

Backpropagation: 

![image-20230723194318076](DeepLearning.assets/image-20230723194318076.png)

#### **What are the benefits of deep architecture?**

#### **Why “Deep” neural network not “Fat” neural network?**

![image-20230723194616072](DeepLearning.assets/image-20230723194616072.png)

