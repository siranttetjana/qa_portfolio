# 🔗 API Testing – Swagger Petstore (Postman)

## 📌 Overview

This document demonstrates API testing using the **Swagger Petstore API** in Postman.

The collection includes basic CRUD operations and examples of working with API requests and responses.

---

## 🛠️ Tools

* Postman
* Swagger Petstore API

---

## 📂 Scope of Testing

The following API operations were tested:

* **GET** – Find pets by status
* **POST** – Add a new pet
* **PUT** – Update an existing pet
* **DELETE** – Delete a pet

Each request includes:

* Parameters
* Headers
* Request body (where applicable)
* Example responses

---

## 🧪 Test Approach

During testing, the following aspects were validated:

* Correct status codes (e.g., 200 OK)
* API response structure
* Data returned in response body
* Basic request execution in Postman

Example test validation:

```javascript id="z8ydfr"
pm.test("Status code is 200", function () {
    pm.response.to.have.status(200);
});
```

---

## 🔗 File with Requests

You can view the Postman collection here:
👉 (add your PDF or Postman link here)

---

## 📝 Notes

* This project demonstrates basic API testing skills
* Focus is on understanding request/response flow
* Additional test scenarios (negative and edge cases) can be added in future iterations

---



