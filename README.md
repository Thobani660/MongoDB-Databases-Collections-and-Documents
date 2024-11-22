# MongoDB-Databases-Collections-and-Documents

# MongoDB Task: Databases, Collections, and Documents

## **Overview**

This task demonstrates the use of MongoDB databases, collections, and documents. It also covers the differences between JSON and BSON and provides step-by-step instructions for creating a database, inserting documents, exporting data, and pushing the files to GitHub.

---

## **Getting Started**

### **Prerequisites**

1. Install MongoDB and MongoDB Shell (`mongosh`).
   - Download MongoDB Community Edition: [MongoDB Download](https://www.mongodb.com/try/download/community).
2. Install Git for version control.
3. Ensure your system's PATH is configured to include the MongoDB binaries (`mongodump`, `mongosh`, etc.).

---

## **Key Concepts**

### **MongoDB Hierarchy**

1. **Database:** A container for collections.
2. **Collection:** A group of MongoDB documents, similar to a table in relational databases.
3. **Document:** A record in a collection, stored in JSON-like format.

### **JSON vs BSON**

- **JSON (JavaScript Object Notation):**
  - Text-based and human-readable.
  - Limited data types.
- **BSON (Binary JSON):**
  - Binary representation of JSON.
  - Supports additional data types like Date, Binary, and Decimal.
  - Optimized for storage and efficiency in MongoDB.

---

## **Step-by-Step Instructions**

### **1. Starting the MongoDB Shell**

1. Open a terminal.
2. Start the MongoDB server:
   ```bash
   mongod
   ```

### ** 2. On the VsCode **

1. Open a new terminal in VsCode

   - Click on the Terminal icon in the Activity Bar.

   2. Navigate to the MongoDB installation directory:

      ````bash
      cd /usr/local/mongodb/bin
          ```
          3. Start the MongoDB shell:
              ```bash
              mongosh
                  ```
  ### **3. Creating a Database and Collection**
 1. In the MongoDB shell, create a new database
      ```bash
       use CodeTribe
        ```
   2. Create a new collection:
    ```bash
     db.createCollection("students")
     ```
     ### **4. Inserting Documents**
     1. Insert a new document into the "students" collection:
     ```bash
     e.g db.students.insertOne({name: "John Doe", age: 20})
       ```
       ### **5. Querying Documents**
       1. Find all documents in the "students" collection:
        ```bash
        db.students.find()
        ```
        2. Find a specific document by its ID:
         ```bash
        db.students.findOne({ _id: ObjectId("...") })

      ````
