# Deep-Learning
Implementation of different fully connected classifiers which solves MINSIT and comparison between them.Furthurmore there is an demonstration of overfitting to random labels in Exerice 2.

1. [General](#General)
    - [Background](#background)
    - [Program Structure](https://github.com/tomershay100/Multiclass-Classification/blob/main/README.md#program-structure)
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
Exerice 1 is divded to servel parts. The first part is creating the the train and test function which will be used by each classifier to train and test its performence.The next part is defining the diffrent classifiers and running train and test on them. At last, there is comprassion between the the layers number selecting the best one and similar process for the activation function. 

In Exerice 2, a similar procces is contsructed.After deffining the needed train and test function we run on a large number of epochs and watch the effect on train and test loss.

### Running Instructions
After donwloading the file on colab. Press on file -> open nootbook -> Upload and then drop to downloaded file.

Now you can run the whole nootbok or specfic cells.

## Dependencies
* [Python 3.6+](https://www.python.org/downloads/)
* Git
* [NumPy](https://numpy.org/install/)

## Installation
I will use google as an example but similar procces can be prefomred on other nootbook editors
1. Open google colab
2. Clone the project by:
	```
	!git clone https://github.com/elaysason/Deep-Learning.git
	```	
<img src="https://i.imgur.com/FOCHnOA.png" data-canonical-src="https://gyazo.com/eb5c5741b6a9a16c692170a41a49c858.png" width=30% height=30% />

3. Now the folder is in your files on colab. simpily download the nootbook as showed
<img src="https://i.imgur.com/I1P2DOv.png" data-canonical-src="https://gyazo.com/eb5c5741b6a9a16c692170a41a49c858.png" width=30% height=30% />
	

	 
## Footnote:
As you can see, there are a number of additional files. The files contain different graphs of different experiments in the program (for example, changing the value of the learning rate or changing the feature that is downloaded, etc.). In addition, it contains a report in the Hebrew language that explains the implementation of the algorithms, the experiments performed and the graphs.	 

In addition, there is also the label file of the test file, called test_y.txt. You can run the algorithm and check my accuracy percentages (which stand at ```96.66%``` in KNN, ```94.86%``` in perceptron, ```96.26%``` in SVM and ```94.25%``` in PA).
