# Batch and momentum

---

Review: Optimization with Batch

![image-20230731191233453](BatchandMomentum.assets/image-20230731191233453.png)

---

### Small Batch v.s. Large Batch

![image-20230731191529623](BatchandMomentum.assets/image-20230731191529623.png)

- Larger batch size does **not** require longer time to compute gradient.   GPU有平行运算的能力但是当数据量增加到足够大的时候，一次update 的时间还是会大幅增加。![image-20230731192027539](BatchandMomentum.assets/image-20230731192027539.png)

- Smaller batch requires longer time for one epoch(longer time for seeing all data once)  ![image-20230731192228180](BatchandMomentum.assets/image-20230731192228180.png)

  ![image-20230731192303055](BatchandMomentum.assets/image-20230731192303055.png)

- Smaller batch size has better performance. what's wrong with large batch size?---Optimization Fails

  ![image-20230731192632920](BatchandMomentum.assets/image-20230731192632920.png)

- Noisy update is batter for training![image-20230731192813389](BatchandMomentum.assets/image-20230731192813389.png)

- Small batch is better on testing data

  ![image-20230731193022957](BatchandMomentum.assets/image-20230731193022957.png)

  ![image-20230731193304775](BatchandMomentum.assets/image-20230731193304775.png)

![image-20230731193437111](BatchandMomentum.assets/image-20230731193437111.png)

<u>***思考：有没有方法能够结合两种batch的优点呢？？***</u>

---

### Momentum

![image-20230731193637602](BatchandMomentum.assets/image-20230731193637602.png)

#### (Vanilla) Gradient Descent

![image-20230731193719310](BatchandMomentum.assets/image-20230731193719310.png)

#### Gradient Descent + Momentum

> Movement: movement of **last step** minus gradient at present

![image-20230731194001960](BatchandMomentum.assets/image-20230731194001960.png)

![image-20230731194121321](BatchandMomentum.assets/image-20230731194121321.png)

![image-20230731194233206](BatchandMomentum.assets/image-20230731194233206.png)'

## Concluding Remarks

![image-20230731194306717](BatchandMomentum.assets/image-20230731194306717.png)

