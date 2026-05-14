# Day 5 - Apex Introduction

# 1. What is Apex?

Apex is a programming language developed by Salesforce for building custom business logic on the Salesforce platform.

It is similar to Java and is used when declarative tools like Flows and Process Builder are not enough to solve complex business problems.

Using Apex, developers can:
- Automate complex workflows
- Create custom validations
- Integrate external systems
- Perform calculations
- Handle large-scale data processing
- Build custom APIs and services

Apex runs on Salesforce servers and works securely within the Salesforce platform.

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# 2. Difference

# A) Flow vs Apex

 Flow                                           Apex 

 No-code / low-code tool                      Programming language 
 Drag-and-drop interface                     Written using code 
 Easy for admins                             Used by developers 
 Best for simple automation                  Best for complex logic 
 Faster to build                             More flexible and powerful 
 Limited customization                       Full customization possible 

### Example:
- Flow → Send automatic email after student registration
- Apex → Calculate scholarship eligibility using multiple conditions and academic history

# B) Configuration vs Coding

 Configuration                                   Coding 

 Uses clicks not code                             Uses programming 
 Faster development                              More development time 
 Easy maintenance                                Requires developers 
 Best for standard requirements                  Best for advanced requirements 
 Less flexible                                   Highly flexible 

### Examples:
- Configuration → Validation Rules, Flow Builder, Page Layouts
- Coding → Apex Triggers, Custom APIs, Complex Integrations

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# 3. Real Examples Where Apex Is Needed

## 1. Scholarship Eligibility System

A college wants to:
- Check attendance
- Verify marks
- Validate family income
- Apply special reservation rules

This logic becomes too complex for normal flows, so Apex is used.

## 2. Payment Gateway Integration

College fee system needs to connect with:
- Razorpay
- Paytm
- Bank APIs

External API integrations require Apex programming.

## 3. Automatic Exam Seating Arrangement

System must:
- Allocate rooms
- Avoid duplicate seat numbers
- Separate students by branch
- Manage room capacity

Complex processing and calculations require Apex.

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# 4. Integrated System Design

# College Management System

## A) CRM Usage

CRM helps manage:
- Student admissions
- Faculty details
- Courses
- Fee payments
- Support requests
- Communication

The system improves student management and automation.

# B) Objects

## Standard Objects
- Account → College Departments
- Contact → Students & Faculty

## Custom Objects
- Student__c
- Course__c
- Fee__c
- Attendance__c
- Exam__c
- Result__c

# C) Relationships

 Parent Object                      Child Object                                Relationship 
 Department                           Student                                     Lookup 
 Student                              Fee                                         Master-Detail 
 Student                             Attendance                                    Master-Detail
 Course                              Exam                                            Lookup 

Relationships help connect data properly.

# D) Validation Rules

Examples:
- Student mobile number must contain 10 digits
- Attendance cannot exceed 100%
- Fee amount cannot be negative
- Email must follow valid format

Validation improves data quality.

# E) Flow Usage

## Admission Flow
When student submits form:
1. Create student record
2. Send confirmation email
3. Notify department
4. Generate student ID automatically

## Fee Reminder Flow
- Automatically send reminders before due date


# F) Apex Usage

## Scholarship Logic
Apex calculates:
- Merit score
- Reservation benefits
- Attendance eligibility
- Financial conditions

## External Payment Integration
Apex connects Salesforce with banking/payment systems.

## Exam Processing
Apex generates:
- Hall tickets
- Seating allocation
- Result calculations

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# 5. Pseudocode Examples

# Example 1: Scholarship Eligibility

```text
IF attendance > 75
   AND marks > 80
   AND income < 200000
THEN
   scholarship = approved
ELSE
   scholarship = rejected
```

# Example 2: Fee Reminder System

```text
FOR every student
   IF fee_due_date is near
      SEND reminder email
END FOR
```

---

# Example 3: Attendance Validation

```text
IF attendance > 100
   SHOW error message
ELSE
   SAVE record
```

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# 6. Reflection - Why Enterprise Systems Eventually Need Programming

Enterprise systems start with simple business requirements, but as organizations grow, processes become more complex.
No-code tools are excellent for standard automation, but companies eventually need programming for:
- Complex business logic
- External integrations
- Advanced calculations
- High-performance processing
- Custom user experiences

Programming languages like Apex provide flexibility and scalability that declarative tools alone cannot provide.

The best enterprise systems combine:
- Configuration for simple requirements
- Programming for advanced requirements

This balance reduces development cost while maintaining flexibility.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

# ✍ Reflective Questions

# 1. Why is Apex needed if Salesforce already has Flows?

Flows are powerful for standard automation, but Apex is needed for:
- Complex calculations
- Advanced business logic
- External integrations
- Large-scale processing
- Custom functionality

---

# 2. When should developers prefer no-code solutions?

Developers should prefer no-code solutions when:
- Requirements are simple
- Standard automation is enough
- Faster delivery is needed
- Maintenance should be easier

---

# 3. What problems require custom programming?

Examples:
- Banking integrations
- AI-based processing
- Complex validations
- Dynamic calculations
- Real-time external communication

---

# 4. Why is business logic important in enterprise systems?

Business logic ensures:
- Correct workflows
- Accurate decision-making
- Data consistency
- Policy enforcement
- Process automation

Without business logic, systems cannot handle real organizational rules properly.

---

# 5. Why should developers avoid unnecessary coding?

Unnecessary coding:
- Increases maintenance cost
- Creates complexity
- Causes more bugs
- Reduces system stability

Simple problems should use declarative tools whenever possible.

---

# 6. How does programming increase flexibility?

Programming allows:
- Full customization
- Dynamic processing
- Complex decision-making
- Integration with external systems
- Advanced automation

This flexibility helps organizations adapt to changing business needs.

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------
