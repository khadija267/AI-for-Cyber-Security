# AI for Cyber Security
 Intelligent solutions for cyber security probelms.
 
 
## 1. Kafka Dynamic Intrusion Detector
A comparison between static learning and adaptive learning using kafka server.

1. Cicids Network Intrusion Detection:

> Binary class classification to predict whether there is an attack or not.

-- Static solution:<br>
Random Forest with hyper parameters tuning:<br>
The model performance has slightly improved , as in the first class the f1 score
increased up till 100%.
![alt text](https://github.com/khadija267/AI-for-Cyber-Security/blob/main/images/1_static.png?raw=true)
-- Dynamic slution:<br>
Adaptive Learning using HoeffdingTreeClassifier on the data streamed using
skmultiflow library.<br>
The accuracy is decreased as the mean accuracy
within streams was only 0.88.
![alt text](https://github.com/khadija267/AI-for-Cyber-Security/blob/main/images/1.dynamic.png?raw=true)<br>
Comparing between mean and
current metrics results:<br>
![alt text](https://github.com/khadija267/AI-for-Cyber-Security/blob/main/images/2_dynamic.png?raw=true)

2. IOT Botnet Attack Detection:

> Multiclass classification to predict is the case is normal or a specific type of attack.

-- Static solution:<br>
Random Forest with hyper parameters tuning:<br>

![alt text](https://github.com/khadija267/AI-for-Cyber-Security/blob/main/images/2_static.png?raw=true)

-- Dynamic slution:<br>
Adaptive Learning using HoeffdingTreeClassifier on the data streamed using
skmultiflow library.<br>

The accuracy is decreased as the mean accuracy
within streams was only 0.92.<br>
![alt text](https://github.com/khadija267/AI-for-Cyber-Security/blob/main/images/2_dynamic_2.png?raw=true)
<br>
Comparing between mean and
current metrics results:
The mean accuracy is 92.8%
which is not far away from the
static solution.<br>
![alt text](https://github.com/khadija267/AI-for-Cyber-Security/blob/main/images/2_dynamic_3.png?raw=true)

3. Summary:<br>
<p>
We except that the static solution is better than the dynamic one, as the model is
being confused from dynamic solutions drawbacks such as the drifting concept.
Streaming data is tricky to deal with and needs more intelligent solutions than the
traditional machine learning solutions.</p>
## 2. Network Attack Detection:

Applying clustering and binary classification by classic and ensemble supervised algorithms on network data.
We got AUC of approximately 1 and +98% accuracy.

![alt text](https://github.com/khadija267/AI-for-Cyber-Security/blob/main/images/1.png?raw=true)
