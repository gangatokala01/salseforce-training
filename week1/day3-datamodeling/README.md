#### 1. Difference Between: 
 App :A collection of related features, objects, and tools used for a specific purpose.
 Object : A database table that stores similar types of information.
 Record :A single row of data inside an object
 Field : A single piece of information in a record. 
 ## Simple Explanation

### App
An app is a complete system used to manage a specific process or business activity.

### Object
An object stores related data like a table in a database.

### Record
A record is one complete entry stored inside an object.

### Field
A field stores one specific detail about a record.



------------------------------------------------------------------------------------

## 2. Standard vs Custom Objects
### Standard:
      1. Pre-built objects provided by Salesforce.
      2.Already available in the system.
      3.Used for common business data.
      4.Examples: Account, Contact, Opportunity
### Custom Objects:
      1.Objects created by users based on business needs.
      2. Need to be created manually.
      3.used for specific or unique business data.
      4.Examples: Student, Library, Hospital Patient
## Simple Explanation

### Standard Objects
Standard objects are default objects already available in Salesforce for common business operations.

### Custom Objects
Custom objects are user-created objects designed to store special or project-specific data.

--------------------------------------------------------------------------------------------

#### 3. Your College Data Model 
Include: 
 Objects 
 Relationships 
 Diagram/image


###### Objects

1. Student
2. Course
3. Faculty
4. Department


## Relationships
 Object 1      Relationship        Object 2 
 Student      Enrolled In          Course 
 Faculty       Teaches             Course 
 Faculty      Belongs To          Department 
 Student       Belongs To          Department 
 - A student can enroll in many courses.
- A faculty member teaches courses.
- Every faculty member belongs to a department.
- Students are also connected to departments.



##### # Formula Fields
A Formula Field is a special field in Salesforce that automatically calculates values using a formula.
It works like formulas in Excel.
formula fields automatically perform calculations and show results without manual work.
They help reduce errors and save time because values are updated automatically whenever data changes.


---
# Reflective Questions
## 1. Why can’t companies manage everything using Excel sheets?
Excel sheets become difficult to manage when data is very large.
Multiple users editing at the same time can create confusion, duplicate data, and errors. 
Excel also lacks strong security, automation, and relationship management features.

---
## 2. Why are relationships important between objects?
Relationships connect related data between objects. 
They help organize information properly and make data retrieval easier.
For example, connecting Students with Courses helps track which student enrolled in which course.

---
## 3. What problems happen if data is inconsistent?
Inconsistent data can cause wrong reports, duplicate records, confusion, and poor decision-making.
It reduces data accuracy and affects business operations.

---
## 4. Why should repetitive calculations be automated?
Automation saves time, reduces manual effort, and minimizes calculation errors.
It also ensures accurate and consistent results every time.

---
## 5. Why should invalid data be blocked early?
Blocking invalid data early improves data quality and prevents future problems.
It helps maintain correct records and avoids mistakes in reports and processes.

---

## 6. Why is Salesforce called a metadata-driven platform?

Salesforce is called a metadata-driven platform because most customizations are done using configuration instead of coding.
Objects, fields, relationships, and automation are created using metadata, making development faster and easier.

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
