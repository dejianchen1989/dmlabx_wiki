### 1. SVM流行的原因
* It is a discriminant-based method and uses Vapnik’s principle to never solve a more complex problem as a first step before the actual problem. **[基于判别式，不必估计类密度或后验概率值，只需要估计类边界]**
* After training, the parameter of the linear model, the weight vector, can be written down in terms of a subset of the training set, which are the so-called support vectors. **[支持向量可以提取知识：它们是类边界附近、不确定或有错误的实例；它们的个数提供了泛化误差的估计；模型参数可以核化]**
* The output is written as a sum of the influences of support vectors and these are given by kernel functions that are application-specific measures of similarity between data instances. **[用核函数作为数据实例之间的相似性度量，它能够把数据映射到另一个空间，并在那个空间找到线性解]**
* Typically in most learning algorithms, data points are represented as vectors, and either dot product (as in the multilayer perceptrons) or Euclidean distance (as in radial basis function networks) is used. A kernel function allows us to go beyond that. **[相比于其他学习算法使用点积、欧氏距离，核函数更具有一般性(也就是能自定义核函数)]**
* Kernel-based algorithms are formulated as convex optimization prob- lems, and there is a single optimum that we can solve for analytically. Therefore we are no longer bothered with heuristics for learning rates, initializations, checking for convergence, and such. **[基于核的算法可以表示成凸优化问题，存在单个最优解，并可以解析地求解]**

### 2. 线性可分情况：最大分离超平面

   从两类情况开始，用+1和-1标记。样本为

### 3. 不可分情况：软边缘超平面