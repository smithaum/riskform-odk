# Criminal Risk Assessment – ODK XLSForm

## 📌 Project Overview

This project focuses on developing an **ODK XLSForm** based on the provided **Criminal Risk Assessment Request** form.

The purpose of this project is to convert the provided paper-based form into a structured digital form that can be used with **ODK (Open Data Kit)**.

The XLSForm represents the information and requirements provided in the original Criminal Risk Assessment Request document, including consent information, personal identification details, identification documents, and criminal risk assessment request details.

---

## 🎯 Objective

The main objective of this assignment is to:

- Convert the provided Criminal Risk Assessment Request form into an ODK XLSForm.
- Structure the form into appropriate ODK question types.
- Define selectable choices where required.
- Mark mandatory fields as required.
- Implement relevant form logic where applicable.
- Prepare the form for validation and testing.
- Maintain the structure and information provided in the original document.

---

## 📄 Source Form

The XLSForm was developed based on the provided:

**Criminal Risk Assessment Request**

The source form contains information related to:

- Consent for Criminal Risk Assessment
- Release of Information
- Personal identification
- Date of birth
- Gender
- Previous names
- Address and contact information
- Identification documents
- Criminal Risk Assessment request information
- Agency information
- Assigned worker information
- Submitting designate information
- Request date

---

## 🗂️ XLSForm Structure

The Excel workbook is divided into three main worksheets:

### 1. `survey`

The `survey` worksheet contains the main structure of the digital form.

It includes fields for:

- Consent information
- Date
- Signature information
- Witness information
- First name
- Second name
- Last name
- Date of birth
- Gender
- Other last names used
- Other first names used
- Current address
- Current phone numbers
- City/Province or Country of Birth
- Identification information
- Driver's licence information
- Name of person being assessed
- Agency submitting the request
- Reason for risk assessment
- Assigned worker
- Previous criminal risk assessment date
- Submitting designate
- Designate phone number
- Designate email
- Designate fax
- Request date

---

### 2. `choices`

The `choices` worksheet contains options used by questions that require predefined selections.

Examples include:

#### Gender

- Male
- Female

#### Identification

- Birth Certificate
- Social Insurance Card
- Manitoba Health Card
- Treaty Card
- Other
- Manitoba Driver's License with Photo

#### Reason for Risk Assessment

- With Consent
- Without Consent
- Child Protection Concerns
- Place of Safety
- Kinship or Customary Care Agreement

---

### 3. `settings`

The `settings` worksheet contains the basic configuration of the ODK form.

It includes:

- Form title
- Form ID
- Form version
- Default language

---

## 🔐 Required Fields

The original Criminal Risk Assessment Request form identifies certain sections with an asterisk (`*`) as required.

These requirements have been reflected in the XLSForm by marking the corresponding fields as mandatory.

Examples include:

- First Name
- Last Name
- Date of Birth
- Gender
- Current Address
- Current Phone Numbers
- City/Province or Country of Birth
- Name of Agency Submitting Request
- Reason for Risk Assessment
- Assigned Worker
- Submitting Designate
- Designate Phone
- Designate Email
- Request Date

---

## 🔄 Form Logic

The XLSForm includes basic conditional logic for fields that depend on a previous selection.

For example, additional identification information can be requested when the user selects the corresponding identification option.

This helps keep the digital form organized and prevents unnecessary fields from being displayed when they are not applicable.

---

## 🛠️ Tools & Technologies

The project uses:

- **ODK XLSForm**
- **Microsoft Excel**
- **GitHub**

The XLSForm format is used to define the structure, questions, choices, requirements, and logic of the digital form.

---

## 🧪 Form Validation & Testing

The XLSForm will be validated and tested using an ODK-compatible XLSForm testing tool.

Testing will be used to verify:

- Form structure
- Question types
- Required fields
- Choice lists
- Conditional fields
- Form navigation
- Overall form functionality

Any validation errors identified during testing will be corrected before the final submission.

---

## 📁 Repository Structure

The repository currently contains:

```text
criminal-risk-assessment-xlsform/
│
├── Criminal_Risk_Assessment_XLSForm.xlsx
│
└── README.md
````

The demonstration video will be added to the repository later.

---

## 📊 Project Workflow

The overall workflow followed for this assignment is:

```text
Criminal Risk Assessment PDF
            ↓
Identify Form Fields
            ↓
Create XLSForm
            ↓
Configure Survey Sheet
            ↓
Configure Choices Sheet
            ↓
Configure Settings Sheet
            ↓
Add Required Fields & Logic
            ↓
Validate & Test XLSForm
            ↓
Upload to GitHub
            ↓
Record Demonstration Video
            ↓
Final Submission
```

---

## 🎥 Video Demonstration

**Video demonstration will be added here after recording.**

The video will demonstrate the completed XLSForm and explain the implementation.

---

## 📌 Assignment Submission

The completed project will be submitted through the required WhatsApp group using the specified format:

```text
Your Name - GitHub Repository Link
```

---

## 👩🏻‍💻 Author

**Smitha U M**

Computer Science and Engineering Student

---

## 📚 Reference

The ODK XLSForm documentation and testing resources provided with the assignment were used as references for developing and validating the form.

```
