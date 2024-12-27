# AWS Contact Form Project

This project demonstrates deploying a web application using **AWS Lambda**, **API Gateway**, and **DynamoDB**. It provides a contact form where users can submit their details, which are then stored in a DynamoDB table. The application showcases serverless computing and integrates modern web technologies.

---

## Features

- **Contact Form**: A user-friendly web interface for submitting contact details.
- **Serverless Backend**: Powered by AWS Lambda for handling HTTP requests.
- **API Gateway Integration**: Routing requests to the appropriate Lambda function.
- **DynamoDB Storage**: Persisting user-submitted data securely.
- **Responsive Design**: HTML pages styled for a seamless user experience.

---

## Architecture Overview

1. **Frontend**: 
   - `contactus.html`: A form for collecting user data.
   - `success.html`: A thank-you page displayed after form submission.

2. **Backend**: 
   - **AWS Lambda**: Handles form submission, routing, and data processing.
   - **API Gateway**: Acts as the HTTP interface for Lambda functions.
   - **DynamoDB**: Stores the submitted data in a secure and scalable manner.

---

## Files

### 1. `contactus.html`
The contact form's user interface.

### 2. `success.html`
A thank-you page with a simple animation.

### 3. `lambda_function.py`
The backend logic for:
- Serving the HTML pages (`GET` requests).
- Handling form submissions (`POST` requests).
- Storing data in DynamoDB.

---

## How to Deploy

1. **Set Up AWS Services**:
   - Create an API Gateway.
   - Configure a DynamoDB table to store form submissions.
   - Deploy a Lambda function and integrate it with the API Gateway.

2. **Upload Code**:
   - Zip the `lambda_function.py`, `contactus.html`, and `success.html`.
   - Deploy the zip file to AWS Lambda.

3. **Configure API Gateway**:
   - Set up `GET` and `POST` methods.
   - Link them to the Lambda function.

4. **Testing**:
   - Access the API Gateway URL to load the contact form.
   - Submit the form and verify the data in DynamoDB.

---

## Prerequisites

- An AWS account.
- Basic knowledge of AWS Lambda, API Gateway, and DynamoDB.
- Python 3.x installed locally for development.

---

## Future Enhancements

- Add validation for form inputs.
- Integrate a logging mechanism for better debugging.
- Extend DynamoDB to include more attributes (e.g., timestamps).

---

## Acknowledgments

Developed by **Praveen Kumar Patil** as an AWS serverless architecture demonstration.

---

## License

This project is open-source and available under the [MIT License](LICENSE).

