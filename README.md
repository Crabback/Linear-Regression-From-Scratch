# Linear-Regression-From-Scratch

# **Linear Regression**

A linear regression model with both L1 and L2 regularization will be implemented. The class LinearRegression will have the following API:

* `__init__(alpha, tol, max_iter, theta_init, penalty, lambd)`
* `compute_cost(theta, X, y)`
* `compute_gradient(theta, X, y)`
* `fit(X, y)`
* `has_converged(theta_old, theta_new)`
* `predict(X)`

### **Cost Function**

The cost function computes the scalar cost for a given $\theta$ vector. 


<img src="https://latex.codecogs.com/svg.image?\mathcal{L}({\theta})&space;=&space;\frac{1}{N}\sum_{i&space;=1}^N&space;(h_{{\theta}}({x}_i)&space;-&space;y_i)^2" title="\mathcal{L}({\theta}) = \frac{1}{N}\sum_{i =1}^N (h_{{\theta}}({x}_i) - y_i)^2" />

where

$h_{{\theta}}({x}_i) = \theta^Tx_i$

L1 Regularization Loss:

<img src="https://latex.codecogs.com/svg.image?\mathcal{L_1}({\theta})&space;=&space;\mathcal{L}({\theta})&space;&plus;&space;\lambda\sum_{j&space;=&space;1}^D&space;&space;|{\theta}_j|" title="\mathcal{L_1}({\theta}) = \mathcal{L}({\theta}) + \lambda\sum_{j = 1}^D |{\theta}_j|" />

L2 Regularization Loss:

<img src="https://latex.codecogs.com/svg.image?\mathcal{L_2}({\theta})&space;=&space;\mathcal{L}({\theta})&space;&plus;&space;\lambda\sum_{j&space;=&space;1}^D&space;&space;{\theta}_j^2&space;" title="\mathcal{L_2}({\theta}) = \mathcal{L}({\theta}) + \lambda\sum_{j = 1}^D {\theta}_j^2 " />
