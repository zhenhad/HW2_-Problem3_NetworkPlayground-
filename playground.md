# Zhenous Hadi Jafari _ HW2 _ Problem 3 _NetworkPlayground _ 02/18/2024

## A First Neural Network
Task 1:\
The model as given combines our two input features into a single neuron.
Will this model learn any nonlinearities? Run it to confirm your guess.\
As it is selected, the activation is Linear, the training_loss = 0.49, and Test_Loss = 0.5\ So there is no no nonliniarity learning.
### Screenshots
![1](https://github.com/zhenhad/HW2_-Problem3_NetworkPlayground-/assets/39483728/5132ecba-c11b-4a9c-8c8f-47e285a3be6b)

Task 2:\ 
Increasing the number of neurons in the hidden layer from 1 to 2, and also try changing from a Linear activation to a nonlinear activation like ReLU. Can you create a model that can learn nonlinearities? Can it model the data effectively?\
\
it changed from a linear to a nionlinear but it does not represent the nonlinearity completely and correctly.
## Screenshots
![2](https://github.com/zhenhad/HW2_-Problem3_NetworkPlayground-/assets/39483728/534c927e-347c-4d08-b79c-fa1634be88fd)

Task 3:\ 
Increasing the number of neurons in the hidden layer from 2 to 3, using a nonlinear activation like ReLU. Can it model the data effectively? How does model quality vary from run to run?\
Increasing the number of neurons in hidden layer helped decreasing the Test_loss to 0.17 and Training_los to 0.13, and a complete nonlinear classifying.
## Screenshots
![image](https://github.com/zhenhad/HW2_-Problem3_NetworkPlayground-/assets/39483728/db396d6a-1e41-47ba-89b8-67119c3620ff)\

Task 4:\
Continue experimenting by adding or removing hidden layers and neurons per layer. Also feel free to change learning rates, regularization, and other learning settings. What is the smallest number of neurons and layers you can use that gives test loss of 0.177 or lower?
the smallest number of neurons in hidden layer is 3 that gives test_loss of 0.17\
I tried different architecture of networks. Here is one of them with multi hidden layers (3), learning rate(0.3), changing regularization rate(0.01), changing regularization method(L1), and different activation function(sigmoid):\
## Screenshots
![image](https://github.com/zhenhad/HW2_-Problem3_NetworkPlayground-/assets/39483728/28d5c492-7706-4de3-bfb9-fddc56db67aa)\
Does increasing the model size improve the fit, or how quickly it converges? Does this change how often it converges to a good model? For example, try the following architecture:

First hidden layer with 3 neurons.
Second hidden layer with 3 neurons.
Third hidden layer with 2 neurons.

As you can see in the screenshot below, the loss did not improved more than 0.5.\
so increasing model capacity will not necessarily improve the model, theoritally it increase flexiblity but it has its own draw backs like overfitting because of a lot of parameters, and would make the network more expensive.\
## Screenshot
![image](https://github.com/zhenhad/HW2_-Problem3_NetworkPlayground-/assets/39483728/62b75cda-44ee-4bd8-935a-f8ec157aa696)\
# Neural Net Initialization

This exercise uses the XOR data again, but looks at the repeatability of training Neural Nets and the importance of initialization.\

Task 1:\

This exercise uses the XOR data again, but looks at the repeatability of training Neural Nets and the importance of initialization.\
Run the model as given four or five times. Before each trial, hit the Reset the network button to get a new random initialization. (The Reset the network button is the circular reset arrow just to the left of the Play button.) Let each trial run for at least 500 steps to ensure convergence. What shape does each model output converge to? What does this say about the role of initialization in non-convex optimization?\
## Screenshots 1:
![image](https://github.com/DataScienceAndEngineering/homework-2-problem-2-link-id-and-colab-notebook-zhenhad/assets/39483728/012da786-0e5e-4dbb-9d08-a289894d5304)
test los = 0.350\
## Screenshot 2:
![image](https://github.com/DataScienceAndEngineering/homework-2-problem-2-link-id-and-colab-notebook-zhenhad/assets/39483728/5848d2a4-b976-4e7e-ba7f-40ca17d4fe51)
test los = 0.333\
## Screenshot 3:
![image](https://github.com/DataScienceAndEngineering/homework-2-problem-2-link-id-and-colab-notebook-zhenhad/assets/39483728/fa3ef3f2-fd2d-4313-b01f-8288288fd451)
test los = 0.309\
## Screenshot 4:
![image](https://github.com/DataScienceAndEngineering/homework-2-problem-2-link-id-and-colab-notebook-zhenhad/assets/39483728/e05e29a7-4ff3-49c6-8499-76e5f0cd25ac)
test loss = 0.192\
# Screenshot 5:
![image](https://github.com/DataScienceAndEngineering/homework-2-problem-2-link-id-and-colab-notebook-zhenhad/assets/39483728/0fcfb8e2-5199-480b-b808-7602fad701ec)
test loss = 0.309\
# What shape does each model output converge to? What does this say about the role of initialization in non-convex optimization?
Each time the model had specific shape (star, paralel line) and the test loss was different each time (as I mentioned under each screenshot).\ 
Task 2 :\ 
# Screenshot 1 : 
![image](https://github.com/DataScienceAndEngineering/homework-2-problem-2-link-id-and-colab-notebook-zhenhad/assets/39483728/e0ee2cd3-13ca-4b86-bfa3-902841df7391)
test loss = 0.196\
# Screenshot 2 : 
![image](https://github.com/DataScienceAndEngineering/homework-2-problem-2-link-id-and-colab-notebook-zhenhad/assets/39483728/8d638726-5f31-41dc-88de-b1febee1dfc6)
test loss = 0.181\
# Screenshot 3 : 
![image](https://github.com/DataScienceAndEngineering/homework-2-problem-2-link-id-and-colab-notebook-zhenhad/assets/39483728/020ce345-9635-4c50-8632-978eef3ca472)
test los = 0.190\
# Screenshot 4 :
![image](https://github.com/DataScienceAndEngineering/homework-2-problem-2-link-id-and-colab-notebook-zhenhad/assets/39483728/65e322b3-f7ff-4b5d-9788-fc13d8d7f979)
test loss = 0.191\2
# Screenshot 5 :
![image](https://github.com/DataScienceAndEngineering/homework-2-problem-2-link-id-and-colab-notebook-zhenhad/assets/39483728/8c26238b-4829-4c3e-88c1-caa0ab8d7712)
test loss = 0.173
this time (adding a layer) the shape was more similar to each other, but the test loss still different (not as scatter as in the previous network).

## Neural Net Spiral

# Task 1 & 2 :
At the begining I started with a complex networ and following parameter in the screenshot 1:
![image](https://github.com/DataScienceAndEngineering/homework-2-problem-2-link-id-and-colab-notebook-zhenhad/assets/39483728/aac2427f-919c-4c75-b0f3-cd2915fa53a9)
Then I tried to change the model parameters:
![image](https://github.com/DataScienceAndEngineering/homework-2-problem-2-link-id-and-colab-notebook-zhenhad/assets/39483728/9b5902eb-ef5d-4ccb-aa00-2b9439174110)
Then I added extra feature:
![image](https://github.com/DataScienceAndEngineering/homework-2-problem-2-link-id-and-colab-notebook-zhenhad/assets/39483728/1c8f4068-d93b-416e-9a38-cdf00fca7263)
as you can see adding extra feature helped a lot
## The effect of batch size:
### Small batch size:
More sensitive to individual data points, potentially learning more intricate details.
can increase noise and require more training iterations.
### Large batch size:
Uses more information at once, potentially leading to smoother updates and convergence.
might not fit in memory on smaller devices.
![image](https://github.com/DataScienceAndEngineering/homework-2-problem-2-link-id-and-colab-notebook-zhenhad/assets/39483728/30fa4e62-90f1-4ae8-a86a-bbf07b1ad31c)
## The effect of learning rate:
### High learning rate:
Bigger adjustments to weights, faster learning but risk of instability and getting stuck.
### Low learning rate:
Smaller adjustments, slower learning but more stable and might not reach the best solution.
### Optimal learning rate:
Leads to smooth learning, avoids getting stuck, and helps reach the best possible performance.
The 
