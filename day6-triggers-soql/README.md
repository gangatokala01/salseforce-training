# Day 6 - Triggers & SOQL

# 1. What is SOQL?
SOQL  stands for Salesforce Object Query Language is a query language used in Salesforce to retrieve data from objects and databases.
It is similar to SQL but specially designed for Salesforce objects.

Using SOQL, we can:
- Read records from objects
- Filter data using conditions
- Retrieve related records
- Display required information

### Example:
Get all students whose attendance is below 75%.

SOQL helps enterprise systems access data intelligently.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------

# 2. What is an Apex Trigger?

An Apex Trigger is a piece of Apex code that runs automatically when specific events happen on Salesforce objects.

Triggers run when records are:
- Inserted
- Updated
- Deleted

Triggers help systems react automatically to data changes.

### Example:
When a new student record is created:
- Automatically generate Student ID
- Send welcome notification
- Create attendance record

------------------------------------------------------------------------------------------------------------------------------------------------------------------
# 3. Difference

# A) Flow vs Trigger

 Flow                                                           Trigger 

 No-code automation                                        Code-based automation 
 Easy to build                                             Requires programming 
 Best for simple logic                                     Best for complex logic 
 Drag-and-drop interface                                    Written in Apex 
 Used by admins                                             Used by developers 

### Example:
- Flow → Send reminder email
- Trigger → Complex scholarship calculation

# B) Before Trigger vs After Trigger

 Before Trigger                                                         After Trigger 
 Runs before saving record                                              Runs after saving record 
 Used for validation and updating fields                                Used for related actions 
 Faster processing                                                     Used when record ID is needed 

### Example:
- Before Trigger → Validate fee amount
- After Trigger → Send confirmation email after record creation

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# 4. Your Trigger Use Cases (5 Examples)

## 1. Student ID Generation
When a student record is created:
- Automatically generate unique student ID

## 2. Attendance Warning System
When attendance drops below 75%:
- Automatically send warning email

## 3. Fee Payment Update
When fee is paid:
- Automatically update payment status

## 4. Exam Result Processing
When marks are entered:
- Automatically calculate grade and percentage

## 5. Library Fine Automation
When book return date exceeds due date:
- Automatically calculate fine amount
-----------------------------------------------------------------------------------------------------------------------------------------------------------------
# 5. Query Examples (English Query Ideas)

## Example 1
Get all students from CSE department.

---

## Example 2
Find students whose attendance is below 75%.

---

## Example 3
Get all unpaid fee records.

---

## Example 4
Find students who scored above 90%.

---

## Example 5
Get all faculty members from Computer Science department.

----------------------------------------------------------------------------------------------------------------------------------------------------------------------

# 6. Reflection - Why Enterprise Systems React Automatically to Data Changes

Enterprise systems handle thousands of records and business events daily. Manual monitoring becomes difficult and inefficient.

Triggers and automation help systems:
- React instantly to changes
- Maintain data consistency
- Reduce human effort
- Improve business efficiency
- Ensure faster processing

Modern enterprise software is event-driven, meaning actions happen automatically whenever important data changes occur.

This makes systems smarter, faster, and more reliable.

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
