# store_management_api-testing-with-postman

📌 Project Overview
This project focuses on testing a Product API using Postman. The API operations include:

GET all products

POST new product

GET product by ID

PUT update product

PATCH partial update

DELETE product

Postman test scripts were used to validate response codes, payload, headers, performance, and business logic.

🏗️ Tools & Technologies Used

Postman

Mock API (mockapi.io)

JavaScript Postman Scripting (pm.test)

JSON

Newman CLI

Newman HTML Extra Reporter

🔗 Base API

https://{{baseURL}}/products


Variables:

baseURL = 69258a4282b59600d7241059.mockapi.io
id = Fetch dynamically from POST response


🧪 API Endpoints Tested

1️⃣ GET /products
✔ Status 200
✔ Non-empty JSON response

2️⃣ POST /products
✔ Status 201
✔ Extract & store ID dynamically
Request Body example:

{
  "productName": "chair",
  "price": "1000",
  "stock": "true"
}


3️⃣ GET /products/{{id}}
✔ Single product retrieval
✔ Header validations

4️⃣ PUT /products/{{id}}
✔ Full update
✔ Validation of updated fields

5️⃣ PATCH /products/{{id}}
✔ Partial update
✔ No unwanted field changes

6️⃣ DELETE /products/{{id}}
✔ Status validation
✔ Body existence check

🧠 Automated Validation Checks
✔ Status code
✔ Response time
✔ JSON content-type
✔ Structure validation
✔ Data type checks
✔ Content-length non-zero
✔ Logical conditions
✔ CORS checks

📊 Newman Report Integration
This project includes command-line automation using Newman.
A professional Newman HTML Extra report has been successfully deployed for easy access and review.
It provides a detailed visual view of execution results such as passed/failed API tests, response time charts, and failure logs.

🏁 Results & Conclusion
All CRUD API operations were validated successfully.
Automated testing reduced human error and improved reliability of API behavior.

Final Test Status: ✔ All tests passed

📁 Included Deliverables

README.txt ✔

Postman Collection JSON ✔

Newman CLI Automation ✔

HTML Extra Test Report ✔

PDF API Testing Report (on request) 📌
