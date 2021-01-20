# Adaptive-and-Heuristic-AI-enabled-IoT-Edge-for-high-risk-and-rural-patients
CMPE295B: Master's project Adaptive and Heuristic AI enabled IoT Edge for high-risk and rural patients

The healthcare systems are overburdened, and a countless number of patients are deprived of treatments because of the inaccessibility to healthcare.There are myriad possibilities for AI technologies to be used in healthcare, starting from at-home diagnosis to preventive treatments. The proposed solution consisting of a mobile and web application aims to provide proactive healthcare to rural and high-risk patients. Patients take health tests using the mobile application that serves as an IoT device. It provides fast and reliable diagnosis and treatment recommendations after analyzing the data collected from the patient. The system provides recommendations for respiratory issues and falls.
<br>
Respiratory issues are analyzed by processing lung sounds recorded using a stethoscope and detecting crackles and wheezes in them. Falls are analyzed by checking the data from sensors on the mobile phone.

# Methodology
The system consists of 3 subsystems namely mobile application, web application, and machine learning models.
## Web Application
A single page application (SPA) is built using ReactJS, an open-source javascript library to build user interfaces. In this web application, the users will be able to login and view their profile and dashboard.

## Mobile Application
The mobile app will host a neural network locally to predict users’ conditions and suggest required actions or precautions to be taken by users. The app will be built using the native mobile platform, Android, and the neural network will be hosted within the mobile application using the Tensorflow Lite model, that is generated after compressing an existing Tensorflow model. Chaquopy python sdk for Android is used for preprocessing the data.

## Machine Learning Models
To accomplish the proposed design two different machine learning algorithms are trained. One for predicting respiratory illness (crackles/wheezes detection) and another one for fall detection.

# File Structure

Adaptive-and-Heuristic-AI-enabled-IoT-Edge-for-high-risk-and-rural-patients<br>
|_machinelearning<br>
&nbsp;&nbsp;&nbsp;|__respiratory<br>
&nbsp;&nbsp;&nbsp;|__fall<br>
|_HealthCareAIApp  <br>
|_healthcare-ai-fe<br>
  
