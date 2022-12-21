# Triple-MNIST-classifier-
This is the second assignment in the introduction to machine learning course at Innopolis University. The main tasks in the assignment were:
- To build an ANN model that predicts the grades of the students in 3 different subjects. (regression problem)
- To build a CNN model that predicts the 3 numbers in an image.
- Decision Trees and Ensemble Learning to predict if the bank should give a loan or not.

## Task 1:

I build a flexible ANN architecture that allows changing the number of hidden layers and their channels in order to make the hyperparameter tuning process easier.
![image](https://user-images.githubusercontent.com/71794972/208926243-5aa02c3b-8a92-4e24-9b50-ee01ec580927.png)

For hyperparameter tuning, I used a library called Ray, which does some experiments and returns the best hyperparameters.

## Task 2:

The main issue in task 2 was how to make the neural network predict the value of 3 numbers at once.
To solve this problem, I made it output a 3x10 matrix where every 10 numbers denote the probability distribution for each digit in the image
![image](https://user-images.githubusercontent.com/71794972/208927128-1c026c3e-eef1-4c0f-b6fe-e2b6f51ecb85.png)
![image](https://user-images.githubusercontent.com/71794972/208927145-027ca4fe-c246-4314-b924-e8ee39bf08b9.png)

Example of the input

![2_468](https://user-images.githubusercontent.com/71794972/208928339-7f1dacc8-879a-4f21-90d0-01a2b29e8eb5.png)


### Results:
- Accuracy:
  - CNN = 98.03%
- Number of parameters: 
  - CNN = 11515198
- Speed of inference on CPU
  - CNN = 1.6083474159240723 sec
  
## Task 3:

In this task, I built a decision tree and a random forest tree and compared their results
![image](https://user-images.githubusercontent.com/71794972/208927717-ce373639-db30-407d-93e3-a03b176a31cf.png)
