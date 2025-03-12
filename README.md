# Node.js Express PhonePe Payment Gateway Integration

Welcome to the Node.js Express PhonePe Payment Gateway Integration repository! This project demonstrates the seamless integration of the PhonePe payment gateway into a Node.js and Express application. Follow the comprehensive guide below to set up the payment gateway for User Acceptance Testing (UAT).

## Features

/pay API: Initiate payments and redirect users to the PhonePe payment flow.
/payment/validate/:merchantTransactionId API: Validate payment status using merchantTransactionId.

## UAT Testing Credentials

For testing purposes in the UAT environment, use the following credentials:

# Debit Card

“card_number”: “4242424242424242”,
“card_type”: “DEBIT_CARD”,
“card_issuer”: “VISA”,
“expiry_month”: 12,
“expiry_year”: 2027,
“cvv”: “936”

Note: The OTP to be used on the Bank Page: 123456

# Test Net Banking Details

anchor image
Always use “bankId”: “SBIN” for testing purposes in the request payload of PAY API.
Username: test
Password: test
and click “Submit” on the next screen.
Note: For testing transactions, the lower amount limit is defined as Rs.1/- and the upper amount limit is defined as Rs.1000/-. Please make sure your transaction requests are within these limits.

## How to Run

Clone the project:
`git clone https://github.com/VivekNThakkar/phonepe-express.git`

Install dependencies:
`npm install`

Run the app:
`npm run start`

Open in your browser:
`http://localhost:3002/pay?amount=300`

**/payment/validate** API: Validate payment status.
Method: GET
Endpoint: /payment/validate/:merchantTransactionId

`http://localhost:3002/payment/validate/merchantTransactionId`

## API Endpoints
**/pay API**: Initiate payments.
Method: GET
Endpoint: /pay
Parameters: amount (query parameter)

**/payment/validate** API: Validate payment status.
Method: GET
Endpoint: /payment/validate/:merchantTransactionId


## Contact Information
For any inquiries, collaborations, or development work, feel free to reach out:

LinkedIn: `https://www.linkedin.com/in/vivek-thakkar-b94361121/`
Email: `thakkarv29@gmail.com`
GitHub: `https://github.com/VivekNThakkar`

Happy coding!