# Collection-in-APEX

A generic implementation of **Oracle APEX Collections** demonstrating temporary data handling with full CRUD operations (Add, Update, Delete), image support, validations, and final persistence to the database.

## Overview

This project showcases how **APEX Collections** can be used in a real-world scenario using an **Employee Management Form**.

It demonstrates:

- Temporary data storage using APEX Collections  
- Add, Update, and Delete operations  
- Image handling within collections  
- Data validation  
- Saving data into a database table  

## What is an APEX Collection?

An **APEX Collection** is a **session-based temporary storage** mechanism in Oracle APEX.

### 🔹 Key Features:
- Works like a **shopping cart**
- Stores data temporarily before committing to the database
- Data persists **only during the session**
- Automatically cleared when the session ends or collection is deleted

## Application Screens

<img src="images/1-collection%20page.png" width="700"/>  
<img src="images/2-collection%20backend.png" width="700"/>

## 🔄 Application Flow

### 1️⃣ Employee Form (Data Entry)

A form is used to capture:

- Employee Name  
- Job  
- Salary  
- Image  

<img src="images/collection%20form.png" width="700"/>

### 2️⃣ Add to Collection

- Form data is added to the collection  
- Uses `APEX_COLLECTION.ADD_MEMBER`  
- SQL query available in the `/code` folder  

<img src="images/add%20collection.png" width="700"/>

### 3️⃣ Collection Report (View Data)

Displays all records stored in the collection:

- Name  
- Job  
- Salary  
- Image  

<img src="images/collection%20report.png" width="700"/>

### 4️⃣ Update Collection Member

- Each row includes an **Update button**  
- Uses `SEQ_ID` to identify the record  
- Updates data using `APEX_COLLECTION.UPDATE_MEMBER`  
- SQL query available in the `/code` folder  

<img src="images/collection%20edit%20form%20and%20report.png" width="700"/>  
<img src="images/collection%20update%20dynamic%20action.png" width="700"/>  
<img src="images/update%20collection.png" width="700"/>

### 5️⃣ Delete Collection Member

- Records can be deleted using a **Delete button**  
- Uses `SEQ_ID` for identification  
- SQL query available in the `/code` folder  

<img src="images/collection%20delete.png" width="700"/>  
<img src="images/collection%20delete%20dynamic%20action.png" width="700"/>  
<img src="images/delete%20collection.png" width="700"/>


### 6️⃣ Save Data to Database Table

- All collection records are inserted into a database table  
- Collection is cleared after successful save  
- SQL query available in the `/code` folder  

<img src="images/save%20collection%20data%20to%20table.png" width="700"/>

### 7️⃣ Final Table Report

Displays persisted data from the database, including images.

<img src="images/Emp%20Table%20Report.png" width="700"/>


### 8️⃣ Validations

Implemented **NOT NULL validations** on:

- Employee Name  
- Job  
- Salary  

<img src="images/collection%20validations%20and%20processes.png" width="700"/>



## Use Cases

- Temporary data staging before database commit  
- Multi-step forms (wizard-style applications)  
- Shopping cart-like implementations  
- Bulk data processing  


## Key Learning

This project helps in understanding:

- How to use APEX Collections effectively  
- Decoupling UI interaction from database transactions  
- Improving user experience using temporary data handling  
- Controlled and validated data persistence  

## Author

**Muhammad Ilyas Awan**  
Oracle Techno-Functional Consultant | Oracle ACE Apprentice ♠️ 

📧 ilyas8284@outlook.com  
📱 +92-336-963-8284  
🔗 https://www.linkedin.com/in/ilyas8284  
