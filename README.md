# AI for Cyber Security
 Intelligent solutions for cyber security probelms.

## 1. Time Series Network Anomaly Detection:
NetT is a network data with 9 different anomaly classes.
We got 79 columns after getting rid of the unncessary classes such as the port number and ip addresses.
### Dimensionality Reduction:
We used a Variational Autoencoder (VAE) in PyTorch.
Model Architecture:
fc1 is the first hidden layer, with input_dim input neurons and hidden_dim output neurons.
fc21 is the mean layer, with hidden_dim input neurons and latent_dim output neurons. <br>
This layer outputs the mean values of the Gaussian distribution over the latent space.
fc22 is the log-variance layer, with hidden_dim input neurons and latent_dim output neurons.<br>
 This layer outputs the log-variances of the Gaussian distribution over the latent space.The output of fc21 and fc22 are then combined using the reparameterization trick(

 
## 2. Kafka Dynamic Intrusion Detector
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
We except that the static solution is better than the dynamic one, as the model is
being confused from dynamic solutions drawbacks such as the drifting concept.
Streaming data is tricky to deal with and needs more intelligent solutions than the
traditional machine learning solutions.<br>
## 3. Network Attack Detection:

Applying clustering and binary classification by classic and ensemble supervised algorithms on network data.
We got AUC of approximately 1 and +98% accuracy.

![alt text](https://github.com/khadija267/AI-for-Cyber-Security/blob/main/images/1.png?raw=true)
