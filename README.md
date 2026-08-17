\# Login Time-Based Detection of Suspicious Logins Using Behavioral Analysis



\## Project Overview



This project is a machine learning-based web application designed to detect suspicious login activities by analyzing user login behavior.



The system monitors login-related features such as login time, day of the week, login frequency, authentication status, and IP risk. A trained machine learning model analyzes these features and classifies login activity as either \*\*Normal\*\* or \*\*Suspicious\*\*.



The project is implemented using \*\*Python, Django, SQLite, and Machine Learning\*\*.



\## Objectives



\- Monitor user login activities.

\- Analyze login behavior using machine learning.

\- Detect potentially suspicious login attempts.

\- Store login activity and prediction results in a database.

\- Provide a dashboard for viewing login history.

\- Provide a risk analyzer for manually analyzing login behavior.



\## Technologies Used



\- Python

\- Django

\- SQLite

\- HTML

\- CSS

\- JavaScript

\- Scikit-learn

\- Pandas

\- NumPy

\- Joblib



\## Machine Learning



The system uses a trained machine learning model to classify login behavior.



\### Features Used



The prediction is based on the following features:



1\. Login Hour

2\. Day of Week

3\. Login Frequency

4\. Login Status

5\. IP Risk



The trained model is stored in:



```text

login\_monitor/ml\_model/login\_model.pkl



System Features

1\. User Registration



New users can register through the registration page.



2\. User Login



Users can log in using their username and password.



3\. Login Activity Monitoring



The system records login-related information including:



Date and time

Login hour

Day of week

Authentication status

IP address

Login frequency

ML prediction

4\. Suspicious Login Detection



The machine learning model classifies login activity as:



Normal

Suspicious



If suspicious activity is detected, the system displays a security warning.



5\. Security Dashboard



The dashboard displays the user's login activity history along with the corresponding ML predictions.



6\. Risk Analyzer



The Risk Analyzer allows login behavior to be manually analyzed by entering the required feature values.



Project Structure

MCA\_Final\_Project/

│

├── login\_monitor/

│   ├── migrations/

│   ├── ml\_model/

│   │   ├── login\_model.pkl

│   │   ├── train\_model.py

│   │   ├── login\_behavior\_dataset.csv

│   │   └── feature\_importance.png

│   │

│   ├── templates/

│   │   └── login\_monitor/

│   │       ├── base.html

│   │       ├── home.html

│   │       ├── login.html

│   │       ├── register.html

│   │       ├── dashboard.html

│   │       └── analyze\_login.html

│   │

│   ├── models.py

│   ├── views.py

│   ├── forms.py

│   ├── urls.py

│   └── admin.py

│

├── suspicious\_login\_system/

│   ├── settings.py

│   ├── urls.py

│   ├── asgi.py

│   └── wsgi.py

│

├── manage.py

└── README.md



How to Run the Project

Step 1: Clone the Repository

git clone https://github.com/SumayyaShameer/Login-Time-Based-Suspicious-Login-Detection.git



Step 2: Open the Project

cd Login-Time-Based-Suspicious-Login-Detection



Step 3: Create a Virtual Environment

python -m venv venv



Step 4: Activate the Virtual Environment



Windows:



venv\\Scripts\\activate



Step 5: Install Dependencies

pip install -r requirements.txt



Step 6: Apply Database Migrations

python manage.py migrate



Step 7: Run the Django Server

python manage.py runserver



Open the application in your browser:



http://127.0.0.1:8000/



Application Workflow

User Registration

&#x20;      ↓

User Login

&#x20;      ↓

Collect Login Behavior

&#x20;      ↓

Extract Features

&#x20;      ↓

Machine Learning Model

&#x20;      ↓

Normal / Suspicious

&#x20;      ↓

Store Result in Database

&#x20;      ↓

Display in Security Dashboard



Future Enhancements

Real-time email/SMS security alerts.

Advanced anomaly detection.

Device and browser fingerprinting.

Geographic location-based risk analysis.

Multi-factor authentication integration.

Improved machine learning models.



Author



Sumayya A S



MCA Project



License



This project is developed for academic purposes.







