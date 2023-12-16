### *Introduction*:
ML algorithms are based upon:
	input -> model -> output

The model must be trained, to make it give back an output that makes sense.

To train the algorithm we need:
- Data
- Model
- Objective function
- Optimization algorithm

Data: 
	we need a lot of data to train the model (e.g.: historical data, measurements, etc..)

Model: 
	Linear and non Linear models.
	(e.g.: input1 + input2 + input3 -> LINEARM MODEL)

Objective function:
	The function the model relies on to determine if it is doing things correctly (aka, giving or not good results)

Optimization algorithm:
	Mechanics that changes values of the Model in order to change Model behavior and get a "better Objective function".

The ML process is iterative: 
![[Pasted image 20231216120318.png]]
When we will find a good enough solution to our problem, we will stop.

---
### *Training the Model*:
The machine needs to make lots of trials in order to make a good result.
After thousand of thousand of trials it will find the good way to do it.
Anyway this result can be obtained in dull or intelligent ways: 
- Dull way: random tries
- Intelligent way: optimization algorithm driven tries
---
### *Types of Machine Learning*:
- ###### Supervised:
	We provide the algorithm INPUTS and corresponding DESIRED OUTPUTS ("labeled outputs") and based on those it tunes itself to get better results. 
- ###### Unsupervised:
	We provide the algorithm INPUTS but we do not give any DESIRED OUTPUT("unlabeled outputs"), basically we ask the it to find some sort of undelaying bind between the INPUTS.
	This is useful when we want to subdivide the output in groups we aren't sure what they are.
- ###### Reinforcement:
	We train the algorithm by giving him a REWARD, when it gives a good result.

Supervised ML is the simplest and commonly used, it is subdivided in:
- Classification supervised ML model:
	OUTPUTS are CATEGORIES
- Regression supervised ML model:
	OUTPUTS are NUMERICAL TYPES
---
### *The linear model*: 

Formula:
```linear_model
y = xw + b
```

Parameters:
- w = WEIGHT
- b = BIAS

Definition:
	"The goal of the ML algorithm would be to find **WEIGHT** and **BIAS** values, so the output **y** is as close to the observed value as possible."

![[Pasted image 20231216123833.png]]

Multiple Inputs:
	X and W may contain multiple parameters, but keeping the same linear framework as before.
	I need to do matrix operations, in this case down below notice that i have to consider ABSOLUTE values and subtract them (when multiplying two matrixes) 
	```formula
	y = |x1 * w1| - | x2 * w2| + b 	
	```
![[Pasted image 20231216125705.png]]

This can be extended to any type of problem and getting even multiple outputs.
![[Pasted image 20231216125808.png]]

---
