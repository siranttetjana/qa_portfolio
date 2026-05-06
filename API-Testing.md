# 🔗 API Testing – Swagger Petstore (Postman)

## 📌 Overview

This project demonstrates API testing using the **Swagger Petstore API** in Postman.

The goal was to practice CRUD operations, validate API responses, and test both positive and negative scenarios.

---

## 🛠️ Tools

* Postman
* Swagger Petstore API

---

## 📂 Tested Endpoints

### 🔹 GET – Find pet by status

* **Scenario:** Positive
* Used query parameters
* **Result:** 200 OK

---

### 🔹 POST – Add a new pet (valid data)

* **Scenario:** Positive
* Used variable `{{url}}`
* **Result:** 200 OK

---

### 🔹 POST – Add a new pet (missing required fields)

* **Scenario:** Negative
* Sent invalid data (missing required fields)
* **Result:** 400 Bad Request
* Validation scripts were used

---

### 🔹 PUT – Update a pet

* **Scenario:** Positive
* **Result:** 200 OK

---

### 🔹 DELETE – Delete a pet

* **Scenario:** Positive
* **Result:** 200 OK

---

## 🧪 Validation

During testing, the following checks were performed:

* Status code validation (200, 400)
* Response structure validation
* Basic response validation using Postman test scripts

Example:

```javascript id="k0c6q7"
pm.test("Status code is 200", function () {
    pm.response.to.have.status(200);
});
```

---

## 🧠 Key Learnings

* Practiced working with API endpoints using different HTTP methods
* Implemented both positive and negative testing scenarios
* Used Postman scripts for response validation
* Identified that API may return non-informative error messages (e.g., "bad input")

---

## 🔗 File with Requests

You can view the full Postman collection here:
👉 (add your PDF / Postman link)

---

## 📝 Notes

* This project demonstrates basic API testing skills
* Focus is on understanding API request/response behavior
* Can be extended with additional test scenarios and validations

---

## 🚀 Future Improvements

* Add chained requests (POST → GET validation)
* Use environment variables for dynamic data
* Add more negative and edge test cases
* Improve response validation (schema checks)

---
