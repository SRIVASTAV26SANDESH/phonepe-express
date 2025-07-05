📱 Node.js Express PhonePe Payment Gateway Integration
This repository demonstrates how to integrate the PhonePe Payment Gateway into a Node.js + Express backend application. It supports initiating payments and validating payment status for User Acceptance Testing (UAT).

🚀 Features
Initiate Payment – Seamlessly initiate a payment and redirect users to the PhonePe payment flow.

Validate Payment – Check transaction status using merchantTransactionId.

🧪 UAT Testing Credentials
Use the following dummy card details for testing in the UAT environment:

Card Number: 4242 4242 4242 4242

Expiry Month: 12

Expiry Year: 44

CVV: 936

OTP: 123456

⚠️ These are test credentials only and will not process real payments.

🛠 How to Run Locally
Clone the repository
// git clone https://github.com/SRIVASTAV26SANDESH/phonepe-express.git

Install dependencies
// npm install

Run the server
// npm start

Open in your browser
// http://localhost:3003/pay?amount=300

📡 API Endpoints
1. GET /pay
Initiates the payment process.

Query Parameter:
amount – Amount to be paid (in INR)

Example:
http://localhost:3003/pay?amount=500

2. GET /payment/validate/:merchantTransactionId
Validates the payment using merchantTransactionId.

Route Parameter:
merchantTransactionId – Unique transaction ID provided at initiation

Example:
http://localhost:3002/payment/validate/txn_123456789
