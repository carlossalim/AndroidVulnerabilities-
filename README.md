#  Detecting Android Vulnerabilities using Abnormally Detection

The primary objective of this study is the detection of Android bugs and vulnerabilities. The way to reach our goal of detecting vulnerabilities in Android applications is grounded on our previous works, and we extend the system calls trace research using machine learning techniques to analyze the patterns that could represent a benign and a malign program.
We put together the benign system calls informations using several trustworthy Android Applications and collecting the system call sequences that represents those Apps to build our base dataset.
We also executed programs with known vulnerabilities in a controlled environment and collect system calls triggered by those Apps. We define those sequence of system calls the anomalies in our study.
We selected four vulnerabilities that can be present in Android Apps, and we used the codes from Mitra & Ranganath [17], for the chosen vulnerabilities:  ECB Blockcypher, Dynamic Register Broadcast Rceiver, Fragment Injection Privelege Escalation, and Weak Permissions.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

This research was executed using Anaconda Python, Jupiter Notebook and Tensorflow; you can see bellow the list of libraries used, with their respective version.

```
Python: 3.6.8 |Anaconda, Inc.| (default, Feb 21 2019, 18:30:04) [MSC v.1916 64 bit (AMD64)]
scipy: 1.2.1
numpy: 1.16.2
matplotlib: 3.0.3
pandas: 0.24.2
sklearn: 0.20.3
numba: 0.43.0
pyod: 0.6.8
```
### Installing

```
The log_sample file contains an example of the system call log file that we used in our research. 
FinalProcessing_out.csv - It contains the processed output to be used in the Machine Learning Algorithms

Machine Learning Algorithms used: 
KNN.ipynb - Python code for kNN to detect Android Vulnerabilities.
SVM_MODEL.ipynb - Python code for Support Vector Machine 
LSTM.ipynb -  Python code for Long short-term memory  
GA_LSTM.ipynb - Python code for Genetic Algorithm combined with Long short-term memory
```


A step by step series of examples that tell you how to get a development env running

Say what the step will be

```
Give the example
```

And repeat

```
until finished
```

End with an example of getting some data out of the system or using it for a little demo

## Running the tests

Explain how to run the automated tests for this system

### Break down into end to end tests

Explain what these tests test and why

```
Give an example
```

### And coding style tests

Explain what these tests test and why

```
Give an example
```

## Deployment

Add additional notes about how to deploy this on a live system

## Contributing

Please read [CONTRIBUTING.md](https://gist.github.com/PurpleBooth/b24679402957c63ec426) for details on our code of conduct, and the process for submitting pull requests to us.

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/your/project/tags). 

## Authors

* **Carlos Renato Salim Campos** - *Initial work* - [PurpleBooth](https://github.com/PurpleBooth)
* **Yasir Malik** - *Initial work* - [PurpleBooth](https://github.com/PurpleBooth)

See also the list of [contributors](https://github.com/your/project/contributors) who participated in this project.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* Hat tip to anyone whose code was used
* Inspiration
* etc
