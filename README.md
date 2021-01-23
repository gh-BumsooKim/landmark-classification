# landmark-classification

*CUAI - Deep Learning, Deep2Deep2Deep*

### [Paper]() | [Site]() 

#### Environment

- conda create python=3.6.12
- conda install tensorflow==2.1.0
- conda install matplotlib 
- pip install opencv-python==4.0.0.21
- conda install pandas

#### Fraemworks

- keras

#### DataSet

 - Landmark Image : [https://dacon.io/competitions/official/235585/data/](https://dacon.io/competitions/official/235585/data/)
 
#### Comparison Test Table (Using [Mnist DataSet](https://en.wikipedia.org/wiki/MNIST_database))

| index | 1 (Default) | 2 | 3 | 4 |
| :---: | :---: | :---: | :---: | :---: |
| 1  | Conv2D       | Conv2D         | Conv2D               | Conv2D                   |
| 2  | ReLU         | **Leaky_ReLU** | ReLU                 | ReLU                     |
| 3  | MaxPooling2D | MaxPooling2D   | **AveragePooling2D** | MaxPooling2D             |
| 4  | Conv2D       | Conv2D         | Conv2D               | Conv2D                   |
| 5  | ReLU         | **Leaky_ReLU** | ReLU                 | ReLU                     |
| 6  | Maxpooling2D | Maxpooling2D   | **Averagepooling2D** | Maxpooling2D             |
| 7  | Conv2D       | Conv2D         | Conv2D               | Conv2D                   |
| 8  | ReLU         | **Leaky_ReLU** | ReLU                 | ReLU                     |
| 9  | MaxPooling2D | MaxPooling2D   | **AveragePooling2D** | MaxPooling2D             |
| 10 | Flatten      | Flatten        | Flatten              | Flatten                  |
| 11 | Dense        | Dense          | Dense                | Dense                    |
| 12 | Dropout(0.4) | Dropout(0.4)   | Dropout(0.4)         | **GaussianDropout(0.4)** |
| 13 | Dense        | Dense          | Dense                | Dense                    |
| Epoch_15_Accuracy<br>- Loss<br>- Train / Test | 0.00246471<br>0.9994 / 0.9936 | 0.00208529<br>0.9994 / 0.9934 | 0.00679290<br>0.9986 / 0.9929 | 0.00541235<br>0.9994 / 0.9917 |

## Application

- Origin Image
<p align="center">
  <img src="imgs/org1.png">
</p>

- MaxPooling
<p align="center">
  <img src="imgs/ref1.png">
</p>

- AveragePooling
<p align="center">
  <img src="imgs/ref2.png">
</p>

- **MaxPooling : AveragePooling = 3 : 2**
<p align="center">
  <img src="imgs/ref3.png">
</p>

## Basic

- Origin Image
<p align="center">
  <img src="imgs/org2.png">
</p>

- MaxPooling / AveragePooling / **MaxPooling : AveragePooling = 1 : 1**
<p align="center">
  <img src="imgs/ref4.png">
</p>
