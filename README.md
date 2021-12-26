# Deep-Learning
Implementation of different fully connected classifier which solves MINSIT and comparison between them.Furthurmore there is an demonstration of overfitting to random labels in Exerice 2.

1. [General](#General)
    - [Background](#background)
    - [Program Structure](https://github.com/tomershay100/Multiclass-Classification/blob/main/README.md#program-structure)
    - [About The Output File](https://github.com/tomershay100/Multiclass-Classification/blob/main/README.md#about-the-output-file)
    - [Running Instructions](https://github.com/tomershay100/Multiclass-Classification/blob/main/README.md#running-instructions)
2. [Dependencies](#dependencies) 
3. [Installation](#installation)
4. [Footnote](#footnote)

## General

### Background
The algorithms learn per network a training set of MISIT,the hand written digit database.It makes predictions of new set of digit (test set).

The MINSIT databse got digits from 0 to 9

The various classifiers try to learn the the different characteristics unique to each digit, thus matching the digits in the test set to the digit that best suits it.

#### About The Classifiers
As in the comparssion we compare between the activation function and the number of layer the optimizer function and the loss function are the same between them in order to isolate the effect of the compared attribute. The comparison is made between activation functions:
* ```Relu```: 
![formula](https://render.githubusercontent.com/render/math?math=\color{black}\large{Relu(x)=max(0,x)})	
* ```TanH``` : 
![equation](https://wikimedia.org/api/rest_v1/media/math/render/svg/f8e81902c8d71b06c246769bad0fe17c9cf1efd9)


![alt text](https://i.imgur.com/lTGxBYP.png)
***
The comparison is between 2,3 and 4 layers because the baseline was 3 and I wanted to check the effect of adding and removing one layer. Finnaly as we have 2 choosies for activation function and 3 for n
 
### Program Structure
The code is divided into 4 main functions. In fact, one function per algorithm. Given the training and test files, normalization is performed according to zscore normalization and feature selection is performed too. Then, the four algorithms are called and each in turn returns a list of predictions for each point in the test set. The program exports all the lists to an output file whose contents are briefly explained in the next section.

### About The Output File
All the predictions of each of the algorithms are exported to an output file whose name is received as input to the program. The file contains the data as follows:
```
knn: 0, perceptron: 0, svm: 0, pa: 1
knn: 1, perceptron: 2, svm: 1, pa: 1
knn: 2, perceptron: 2, svm: 2, pa: 1
...
```

### Running Instructions
In order to run the program, it must provide 4 arguments:
* First, a path to the ```txt``` file that contains the training data set.
* Second, a path to the ```txt``` file that contains the labels of each row in the training data set.
* Third, a path to the ```txt``` file that contains the test set.
* Fourth, a path to the output file to which the predictions of each of the algorithms will be written.

The training data set file should contain a number of lines, so that each line consists of 5 floating numbers separated by commas. So is the test set file. The label file consists of the same number of rows of the training set file and contains one numeric value (between 0 and 2) in each row.

## Dependencies
* [Python 3.6+](https://www.python.org/downloads/)
* Git
* [NumPy](https://numpy.org/install/)

## Installation

1. Open the terminal
2. Clone the project by:
	```
	$ git clone https://github.com/tomershay100/Multiclass-Classification.git
	```	
3. Run the ```main.py``` file:
	```
	$ python3 main.py train_x.txt train_y.txt test_x.txt output.txt
	 ```
	 
	 
## Footnote:
As you can see, there are a number of additional files. The files contain different graphs of different experiments in the program (for example, changing the value of the learning rate or changing the feature that is downloaded, etc.). In addition, it contains a report in the Hebrew language that explains the implementation of the algorithms, the experiments performed and the graphs.	 

In addition, there is also the label file of the test file, called test_y.txt. You can run the algorithm and check my accuracy percentages (which stand at ```96.66%``` in KNN, ```94.86%``` in perceptron, ```96.26%``` in SVM and ```94.25%``` in PA).
