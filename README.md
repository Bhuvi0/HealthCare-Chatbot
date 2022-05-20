# HealthCare-Chatbot
******About Doctor Chatbot******
Health Care chatbot is a conversational system which can be used in predicting heart diseases. The system behaves like a Cardiologist which asks consulting questions related to heart problems and tries to provide relavent solutions. This helps in saving a lot of time of the doctor as it gets the consultation before hand. The system also helps the patient to book appointment with Cardiologists depending on the situation. Prediction of Heart Diseases is achieved using ML based Support Vector Machine Algorithm with heart dataset implemented in python. To create a localhost on your PC, ngrok is used which uses port 5000 of your PC & generates a public link for your PC which is required to communicate with Dialogflow Chatbot. Note: The Appointment Scheduler is just a dummy module for this project.

For Research Paper , Project Report and other Materials ,Refer to the drive:
https://drive.google.com/drive/folders/1eRFia1TE7AL7aSjfuM_85qlKWgXyoTUw?usp=sharing
******Technology Stack used:******
1.Dialogflow (Api.ai)
2.python
3.ngrok
4.SVM Algorithm
5.Heart Disease Dataset
6.HTML, CSS, JS
****Python Libraries used:****
1.flask
2.pandas
3.sklearn
4.smtplib
5.json

from Project folder, run this command to install the libraries:

$ pip install -r requirements.txt
_**
**How to use the Project:****_
1.Before we start, go to Project folder and edit pygmail.py file, filling gmailaddress and gmailpassword variables with a email and password, which are admin credentials for this project. We recommend creating & using a dummy Gmail for test purpose. Login, and go to Less Secure App Access and turn it ON to allow mail permissions.
2.Now, Go to Dialogflow Console & create a new project named Doctor_Chatbot. Click on the gear icon (next to project name), and import the Doctor_Chatbot.rar file (from repository) from the IMPORT FROM ZIP option available.
3.Download ngrok. Open command prompt from that folder in which it's present, and execute ngrok http 5000 command. Copy the https link. Go back to Dialogflow project, click on Fulfillment tab and paste the link in the URL section followed by /webhook. Click SAVE button below.
4.Go to Integration tab, click Web Demo and copy the url link. Replace this link in the Chatbot.html file, down below inside the <iframe> where the src url is present.
5.Next, run connection.py file from the Project folder (repository). Open a browser, and enter localhost:5000 or 127.0.0.1:5000 to execute the interface.
