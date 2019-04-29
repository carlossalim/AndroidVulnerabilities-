#  Detecting Android Vulnerabilities using Abnormally Detection

The primary objective of this study is the detection of Android bugs and vulnerabilities. The way to reach our goal of detecting vulnerabilities in Android applications is grounded on our previous works, and we extend the system calls trace research using machine learning techniques to analyze the patterns that could represent a benign and a malign program.
We put together the benign system calls informations using several trustworthy Android Applications and collecting the system call sequences that represents those Apps to build our base dataset.
We also executed programs with known vulnerabilities in a controlled environment and collect system calls triggered by those Apps. We define those sequence of system calls the anomalies in our study.
We selected four vulnerabilities that can be present in Android Apps, and we used the codes from [Mitra & Ranganath](https://bitbucket.org/secure-it-i/android-app-vulnerability-benchmarks/), for the chosen vulnerabilities:  ECB Blockcypher, Dynamic Register Broadcast Rceiver, Fragment Injection Privelege Escalation, and Weak Permissions.

## Getting Started

This research was executed using Anaconda Python, Jupiter Notebook and Tensorflow, so please install these components; we also used several Python libraries that you will also need to install. 

### Libraries

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
### The Project

The log_sample file is not part of the project. It contains an example of the system call log file that we used in our research. The complete log file can be downloaded from [DROPBOX](https://www.dropbox.com/s/vuzw50nijkdfagk/SySCallLog.zip?dl=0)  

```
export_normal1_180sec.txt - Pre-processed file with Normal system calls
export_normal2_180sec.txt - Pre-processed file with Normal system calls
export_vulne_180sec.txt - Pre-processed file with vulnerabilities 

FinalProcessing_out.csv - It contains the processed output to be used in the Machine Learning Algorithms after all features reduction.
FinalProcessing_out97.csv - It contains the processed output to be used in the Machine Learning Algorithms with all fetures.

Machine Learning Algorithms used: 
KNN.ipynb - Python code for kNN to detect Android Vulnerabilities.
SVM_MODEL.ipynb - Python code for Support Vector Machine 
LSTM.ipynb -  Python code for Long short-term memory  
GA_LSTM.ipynb - Python code for Genetic Algorithm combined with Long short-term memory
```

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/your/project/tags). 

## Authors

* **Carlos Renato Salim Campos** - *MSc. Project* - [LinkedIn](https://www.linkedin.com/in/carlossalim/)
* **Yasir Malik** - *Orientation* - [LinkedIn](https://www.linkedin.com/in/ynmalik/)

## Bibliography

[1] 	M. Jaiswal, F. Jaafar and Y. Malik, "Android Gaming Malware Detection Using System Call Behaviour Analysis."

[2] 	M. Ahmed, "Collective Anomaly Detection Techniques for Network Traffic Analysis," Annals of Data Science, p. pp 497–512, December 2018. 

[3] 	G. K. Baah, A. Gray and M. J. Harrold, "On-line Anomaly Detection of Deployed Software," Georgia Institute of Technology, Atlanta.

[4] 	S. Hangal and M. S. Lam, "Tracking Down Software Bugs Using Automatic Anomaly Detection," ICSE, Stanford, 2002.

[5] 	M. Dimitrov and H. Zhou, "Anomaly-Based Bug Prediction, Isolation, and Validation: An Automated Approach for Software Debugging," University of Central Florida, Orlando, 2009.

[6] 	L. Fei and S. P. Midkiff, "Artemis: Practical Runtime Monitoring of Applications for Execution Anomalies," ACM SIGPLAN, Ottawa - Canada, 2006.

[7] 	C. J. Clemente, F. Jaafar and Y. Malik, "Is Predicting Software Security Bugs Using Deep Learning Better Than the Traditional Machine Learning Algorithms?," IEEE International Conference on Software Quality, Reliability and Security, pp. 95-102, 2018. 

[8] 	R. Patel, "Efficiency Analysis of Deep Learning Algorithms In Security Bug Prediction," New York Institute of Technology, Vancouver, 2018.

[9] 	K. Wael, S. S. Murtaza, A. Hamou-Lhadj and C. Talhi, "Combining heterogeneous anomaly detectors for improved software security," Journal of Systems and Software, vol. 137, pp. 415-429, 2018. 

[10] 	S. He, J. Zhu, P. He and M. R. Lyu, "Experience Report: System Log Analysis for Anomaly Detection," in IEEE 27th International Symposium on Software Reliability Engineering (ISSRE), Ottawa, ON, Canada, 2016. 

[11] 	S. Omar, A. Ngadi and H. H. Jebur, "Machine Learning Techniques for Anomaly Detection: An Overview," International Journal of Computer Applications, vol. 79, no. 2, 2013. 

[12] 	S. S. Murtaza, A. Hamou-Lhadj, W. Khreich and M. Couture, "Total ADS: Automated Software Anomaly Detection System," in IEEE 14th International Working Conference on Source Code Analysis and Manipulation, Victoria, BC, Canada, 2014. 

[13] 	M. Du, F. Li, G. Zheng and V. Srikumar, "DeepLog: Anomaly Detection and Diagnosis from System Logs through Deep Learning," ACM SIGSAC Conference on Computer and Communications Security, pp. 1285-1298, 2017. 

[14] 	A. Grover, "Anomaly Detection for Application Log Data," SJSU ScholarWorks, San Jose - CA, 2018.

[15] 	B. Scholkopf and A. J. Smola, Learning with Kernels: Support Vector Machines, Regularization, Optimization, and Beyond, Cambridge, Massachusetts: The MIT Press, 2002. 

[16] 	J. Zhu, S. He, P. H. Jinyang Liu, Q. Xie, Z. Zheng and M. R. Lyu, "LOGPAI," [Online]. Available: https://github.com/logpai/loghub. [Accessed 27 February 2019].

[17] 	J. Mitra and V.-P. Ranganath, "SecureItI Ghera," Kansas State University, 2017. [Online]. Available: https://bitbucket.org/secure-it-i/android-app-vulnerability-benchmarks/.

[18] 	A. Rassem, M. El-Beltagy and M. Saleh, "Cross-Country Skiing Gears Classification using Deep Learning," June 2017. 

[19] 	Mobile App Daily, "Listing The Most Popular Android Versions Of 2018," August 2018. [Online]. Available: https://www.mobileappdaily.com/2018/08/21/popular-android-versions-of-2018. [Accessed 08 April 2019].

[20] 	L. Miakotko, "The impact of smartphones and mobile devices on human health and life," New York University, New York , 2017.

[21]	Android Anatomy and Physiology, http://source.android.com/devices/tech/security (Online; Last Accessed April 01 2018).

[22]	Number of available Android applications, http://www.appbrain.com/stats/number-of-android-apps (Online;Last Accessed 11th April 2019).

[23]	M. Ernst, J. Cockrell, W. Griswold and D. Notkin, “Dynamically discovering likely program invariants to support program evolution”, IEEE TSE, Vol.27, No. 2, Feb 2001.

[24]	R. Hay, "A New Vulnerability in the Android Framework: Fragment Injection," 12 2013. [Online]. Available: https://securityintelligence.com/new-vulnerability-android-framework-fragment-injection/.
	
[25]	A. B. Ayed, "A Literature Review on Android Permission System," International Journal of Advanced Research in Computer Engineering & Technology (IJARCET), vol. Volume 4, no. Issue 4, April 2015.

[26]	L. Sun and et. al., "SigPID: significant permission identification for android malware detection.," 2016 11th International Conference on. IEEE, 2016.

[27]	M. A. Hayes and M. A. Capretz, "Contextual anomaly detection framework for big sensor data," Journal of Big Data, p. 2, 2015.

[28]	H. Zhang, A. Berg, M. Maire and J. Malik, "SVM-KNN: Discriminative Nearest Neighbor Classification for Visual Category Recognition," in 2006 IEEE Computer Society Conference on Computer Vision and Pattern Recognition (CVPR'06), New York, NY, USA,, 2006.

[29]	S. Hochreiter and J. Schmidhuber, "LONG SHORT-TERM MEMORY," Neural Computation, pp. 1735-17780, 1997.

[30]	L. Davis, Handbook of Genetic Algorithms, New York: Artificial Intelligence, 1991.

