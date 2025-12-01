
# 📘 Inventory Management API — Postman & Newman Testing

A complete API testing project using **Postman**, **MockAPI**, **Newman**, and **HTML Extra Reporter**.

## 📌 Introduction

This project demonstrates end-to-end API testing for an Inventory Management system.
It covers:

* CRUD operations (Create, Read, Update, Delete)
* Automated test scripts
* Schema validations
* Environment variable usage
* Visualizations in Postman (tables, charts, cards)
* Automation with Newman
* Professional HTML reports

All tests run against a **MockAPI backend**, simulating real-world behavior.

---

## 🌐 Base URL

```
https://692c60fec829d464006f6827.mockapi.io/cardata
```



---

## 📍 Main API Endpoint

**Resource:** `/Products`

| Field  | Type    | Description       |
| ------ | ------- | ----------------- |
| carid  | String  | Unique identifier |
| name   | String  | Product name      |
| Stocks | Boolean | Stock status      |

(From table on page 1) 

---

## 🔄 CRUD Operations Overview

### **1. GET /car** – Retrieve all car details

Used for:

* Validating product lists
* Visualizing stock distribution
* Verifying data structure
  (Page 1–2) 

---

### **2. POST /car** – Add new car

Example Body:

```json
{
  "Name": "benz",
  "price": 1000,
  "Stocks": true
}
```

(Page 2) 

---

### **3. GET /car/{carid}** – Retrieve car by ID

Used for:

* Fetching detailed vehicle information
* Schema validation
* Product card visualization
  (Page 2) 

---

### **4. PUT /car/{carid}** – Update car data

Allows updating:

* Name
* Supplier
* Stock status
  (Page 2) 

---

### **5. DELETE /car/{carid}** – Delete car

Includes follow-up validation to confirm deletion.
(Page 2) 

---

## 🧪 Environment Variables

| Variable    | Purpose                       |
| ----------- | ----------------------------- |
| baseURL     | Base API URL                  |
| endpoint    | Resource name ("Products")    |
| ID          | Dynamic ID for GET/PUT/DELETE |
| ProductName | Dynamic test product          |
| Stocks      | Boolean status                |

(Page 3) 

---

## 🏗 API Architecture

### ✔ RESTful Architecture Includes:

* Client–Server model
* Stateless communication
* Resource-based URIs
* Standard HTTP methods (GET, POST, PUT, DELETE)

(Page 3–4) 

### ✔ JSON Data Model (Example):

```json
{
  "Name": "Audi",
  "Price": 20000,
  "Stocks": true,
  "carid": "20"
}
```

(Page 4) 

### ✔ MockAPI Backend Features

* Auto ID generation
* Hosted cloud DB
* Realistic responses
  (Page 4) 

---

## 🔧 Running with Newman

Commands used (Page 4–5):

```
newman run Inventory_management.postman_collection.json
newman run Inventory_management.postman_collection.json -d data.csv
newman run Inventory_management.postman_collection.json -d data.csv -r htmlextra
```



---

## 🖼 Screenshots (Page 5)

The PDF includes screenshots of:

* Basic Auth test
* Newman run using CSV
* Newman run using JSON

These show all test scripts executed with **0 failures**.


---

## 🏁 Conclusion

This project fully demonstrates how to design, test, automate, and report API testing using:

* Postman
* Environment variables
* MockAPI
* Newman
* HTML Extra Reporter


Just tell me what you want!
