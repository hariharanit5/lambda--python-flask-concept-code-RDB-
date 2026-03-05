# Python Flask API with AWS Lambda and RDS

## Project Overview

This project demonstrates a **Python Flask-based API that interacts with a MySQL database hosted on AWS RDS**. The application is designed to run in a **serverless architecture using AWS Lambda**, allowing scalable and cost-efficient backend processing.

The Flask application exposes REST API endpoints that retrieve data from the database and return responses in JSON format. The project also includes configuration to enable **Cross-Origin Resource Sharing (CORS)** for frontend integration.

---

## Project Structure

```
project-folder
│
├── app.py
├── lambda--python-flask-concept-code-RDB
└── README.md
```

### Files

**app.py**
Contains the main Flask application that:

* Creates API endpoints
* Connects to the AWS RDS MySQL database
* Returns results in JSON format

**lambda--python-flask-concept-code-RDB**
Contains configuration or deployment logic used to run the Flask application in **AWS Lambda**.

**README.md**
Project documentation and setup instructions.

---

## Technologies Used

* Python
* Flask
* Flask-CORS
* MySQL
* AWS RDS
* AWS Lambda
* REST API

---

## Features

* REST API built using Flask
* Database connection with MySQL (AWS RDS)
* JSON API responses
* CORS enabled for frontend integration
* Serverless deployment using AWS Lambda

---

## Prerequisites

Before running the project, make sure you have:

* Python 3.x installed
* pip package manager
* AWS account
* AWS RDS MySQL database
* Required Python libraries installed

Install dependencies:

```
pip install flask
pip install flask-cors
pip install mysql-connector-python
```

---

## Database Configuration

Update the database configuration in **app.py**:

```
db_config = {
    "host": "your-rds-endpoint",
    "user": "your-username",
    "password": "your-password",
    "database": "your-database-name"
}
```

Replace the values with your **AWS RDS credentials**.

---

## Running the Application Locally

Run the Flask application:

```
python app.py
```

Server will start on:

```
http://localhost:5000
```

---

## API Endpoint Example

Example endpoint:

```
GET /data
```

Example JSON response:

```
{
  "id": 1,
  "name": "example data"
}
```

---

## Deployment (AWS Lambda)

Steps to deploy:

1. Package the application and dependencies.
2. Upload to AWS Lambda.
3. Configure API Gateway.
4. Connect API Gateway to Lambda function.
5. Test the API endpoint.

---

## Use Cases

* Backend API for web applications
* Serverless microservices
* Database-driven applications
* Cloud-based backend services

---


