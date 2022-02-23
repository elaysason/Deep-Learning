# Deep-Learning
Implementation of different fully connected classifiers which solves MINSIT and comparison between them.Furthurmore there is an demonstration of overfitting to random labels in Exerice 2.

1. [General](#General)
    - [Background](#background)
    - [Program Structure](https://github.com/elaysason/Deep-Learning-Comparining-Overfitting/blob/main/README.md#program-structure)
    - [Running Instructions](https://github.com/elaysason/Deep-Learning-Comparining-Overfitting/blob/main/README.md#running-instructions)
2. [Installation](#installation)
3. [Footnote](#footnote)

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


## Installation
I will use google as an example but similar procces can be prefomred on other nootbook editors
1. Open google colab
2. Clone the project by:
	```
	!git clone https://github.com/elaysason/Deep-Learning-Comparining-Overfitting.git
	```	
<img src="https://i.imgur.com/GpMGS2t.png" data-canonical-src="https://gyazo.com/eb5c5741b6a9a16c692170a41a49c858.png" width=50% height=50% />

3. Now the folder is in your files on colab. simpily download the nootbook as showed
<img src="https://i.imgur.com/yl4jdKr.png" data-canonical-src="https://gyazo.com/eb5c5741b6a9a16c692170a41a49c858.png" width=30% height=30% />
	

	 
## Footnote:
The paramters which wasn't comppared in Exerice 1 was determinted from the baseline case which was given.
