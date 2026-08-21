# 🛡️ Criminal Risk Assessment – ODK XLSForm

<p align="center">

**A structured digital implementation of the Criminal Risk Assessment Request using ODK XLSForm**

</p>

<p align="center">

`ODK XLSForm` • `Microsoft Excel` • `Form Logic` • `Validation` • `GitHub`

</p>

---

## 📌 Project Overview

This project implements the provided **Criminal Risk Assessment Request** as a structured **ODK XLSForm**.

The original document was analyzed and translated into a digital data-collection form while preserving its major sections, information requirements, predefined choices, required fields, and applicable conditional behaviour.

The completed form was then tested using fictional data and successfully validated using an ODK XLSForm testing environment.

---

## 🎯 Project Objective

The objective of this assignment is to demonstrate the ability to:

- 📄 Analyze an existing paper-based form
- 🔍 Identify and classify individual form fields
- 📊 Convert the structure into an ODK XLSForm
- 🧩 Select appropriate XLSForm question types
- 🔘 Configure predefined choice lists
- 🔴 Configure required fields
- 🔄 Implement conditional form behaviour
- 🧪 Test the completed form
- ✅ Validate the final XLSForm
- 📚 Document the complete implementation

---

# ✨ Key Features

### 📋 Structured Digital Form

The paper-based Criminal Risk Assessment Request has been transformed into a structured digital form suitable for ODK-based data collection.

### 🧩 Appropriate Question Types

Different field types are used depending on the information being collected, including:

- `text`
- `date`
- `select_one`
- `select_multiple`

### 🔘 Centralized Choice Lists

Selectable options are maintained separately in the `choices` worksheet.

This keeps the form structure organized and makes choice management easier.

### 🔴 Required Field Validation

Fields identified as required in the source document are configured as mandatory in the digital form.

### 🔄 Conditional Behaviour

Additional fields can be displayed based on previous selections where applicable.

### 🧪 Form Validation

The completed XLSForm was tested using fictional information and successfully validated.

**Validation Result:**

> ✅ **Form is valid!**

---

# 🏗️ Form Architecture

The XLSForm follows the standard three-sheet structure:

```text
                    ODK XLSForm
                         │
          ┌──────────────┼──────────────┐
          ↓              ↓              ↓
       survey         choices        settings
          │              │              │
          ↓              ↓              ↓
     Questions       Options        Configuration
     & Logic         & Lists
````

### 📊 Survey Layer

Contains:

* Question types
* Field names
* Labels
* Hints
* Required settings
* Relevant conditions
* Constraints
* Appearance settings

### 🔘 Choice Layer

Contains predefined response options for selection-based questions.

### ⚙️ Configuration Layer

Contains:

* Form title
* Form ID
* Version
* Default language

---

# 📄 Source Form Analysis

The source **Criminal Risk Assessment Request** contains multiple information areas.

## ✍️ Consent Information

Includes information related to:

* Consent
* Date
* Signature
* Witness information

## 👤 Personal Information

Includes:

* First name
* Second name
* Last name
* Date of birth
* Gender
* Other names
* Address
* Phone numbers
* Place of birth

## 🪪 Identification Information

The form provides identification options including:

* Birth Certificate
* Social Insurance Card
* Manitoba Health Card
* Treaty Card
* Other identification
* Manitoba Driver's License with Photo

## 📝 Risk Assessment Request

Includes:

* Name of person being assessed
* Agency submitting the request
* Reason for risk assessment
* Assigned worker
* Previous assessment date
* Submitting designate
* Designate phone
* Designate email
* Designate fax
* Request date

The source document explicitly states that sections marked with an asterisk (`*`) are required. 

---

# 🧠 Implementation Highlights

## 1. Field Mapping

Each relevant field from the source document was mapped to an appropriate XLSForm question type.

Example:

| Source Information | XLSForm Type      |
| ------------------ | ----------------- |
| First Name         | `text`            |
| Date of Birth      | `date`            |
| Gender             | `select_one`      |
| Identification     | `select_multiple` |
| Request Date       | `date`            |
| Agency Name        | `text`            |

---

## 2. Choice Management

Selection-based questions use centralized choice lists.

For example:

```text
Gender
├── Male
└── Female
```

Identification:

```text
Identification
├── Birth Certificate
├── Social Insurance Card
├── Manitoba Health Card
├── Treaty Card
├── Other
└── Manitoba Driver's License
```

---

## 3. Required Fields

Required information from the source document is represented using XLSForm's required-field configuration.

This ensures that important request information cannot be skipped during form completion.

---

## 4. Conditional Logic

The form uses conditional behaviour where additional information depends on a previous selection.

For example:

```text
Select Identification
        │
        ├── Other
        │     ↓
        │  Specify ID
        │
        └── Driver's License
              ↓
        Enter Licence Number
```

This keeps the form cleaner and avoids displaying unnecessary fields.

---

# 🧪 Testing & Validation

Testing was performed using fictional data to verify the behaviour of the completed form.

### 🔍 Validation Checklist

| Test Area          | Result   |
| ------------------ | -------- |
| Form structure     | ✅ Passed |
| Question types     | ✅ Passed |
| Choice lists       | ✅ Passed |
| Required fields    | ✅ Passed |
| Conditional fields | ✅ Passed |
| Form navigation    | ✅ Passed |
| Form validation    | ✅ Passed |

### 🟢 Final Validation

The completed form successfully returned:

**`Form is valid!`**

A screenshot of the validation result is included in the repository.

---

# 🔐 Data & Privacy

All information used during testing and demonstration is **fictional test data**.

No real personal information is intentionally used in the testing dataset.

The test data is used only for:

* 🧪 Form validation
* 📸 Demonstration screenshots
* 🎥 Video demonstration

---

# 📸 Validation Evidence

The repository includes visual evidence of successful validation.

```text
screenshots/
└── xlsform-validation.png
```

The screenshot demonstrates that the completed form successfully passed validation.

---

# 📚 Documentation

Detailed documentation is available in the `docs/` directory.

| Document               | Purpose                        |
| ---------------------- | ------------------------------ |
| 📋 `form-overview.md`  | Overview of the source form    |
| 🗂️ `field-mapping.md` | Source field → XLSForm mapping |
| 🧪 `testing.md`        | Testing and validation process |
| 🔐 `test-data.md`      | Fictional testing dataset      |

---

# 📊 Project Workflow

```text
┌──────────────────────────────────┐
│ Criminal Risk Assessment PDF     │
└────────────────┬─────────────────┘
                 ↓
        🔍 Analyze Form
                 ↓
        📝 Identify Fields
                 ↓
        📊 Build XLSForm
                 ↓
      ┌──────────┼──────────┐
      ↓          ↓          ↓
   Survey     Choices    Settings
      └──────────┼──────────┘
                 ↓
       🔄 Add Form Logic
                 ↓
        🔴 Configure Rules
                 ↓
          🧪 Test Form
                 ↓
          ✅ Validate
                 ↓
          📸 Capture Evidence
                 ↓
          🐙 GitHub Upload
                 ↓
          🎥 Demo Video
                 ↓
          📤 Final Submission
```

---

# 🛠️ Tools & Technologies

| Tool                     | Purpose                           |
| ------------------------ | --------------------------------- |
| 📊 ODK XLSForm           | Digital form development          |
| 📗 Microsoft Excel       | XLSForm authoring                 |
| 🐙 GitHub                | Version control & project hosting |
| 🧪 ODK XLSForm Validator | Form validation                   |
| 📝 Markdown              | Project documentation             |

---

# 📦 Repository Structure

```text
criminal-risk-assessment-xlsform/
│
├── 📄 Criminal_Risk_Assessment_Request.pdf
├── 📊 Criminal_Risk_Assessment_XLSForm.xlsx
├── 📖 README.md
├── 📌 CHANGELOG.md
├── 🌐 LIVE_FORM.md
├── 🖼️ xlsform-validation.png
│
├── 📁 docs/
│   ├── 📋 form-overview.md
│   ├── 🗂️ field-mapping.md
│   ├── 🧪 testing.md
│   └── 🔐 test-data.md
│
└── 🎥 assignment-demo.mp4
```

---

# 🎥 Demonstration Video

The demonstration video will showcase the complete implementation.

### The demonstration will cover:

1. 📄 Source PDF
2. 📊 XLSForm structure
3. 📋 Survey worksheet
4. 🔘 Choices worksheet
5. ⚙️ Settings worksheet
6. 📱 Generated digital form
7. 🧪 Fictional test data
8. 🔄 Form behaviour
9. ✅ Successful validation
10. 🐙 GitHub repository

**🎥 Video: To be added**

---

# 🎯 Learning Outcomes

Through this assignment, the following practical skills were demonstrated:

* 📊 XLSForm development
* 🧩 Form field design
* 🔘 Choice-list management
* 🔄 Conditional form logic
* 🧪 Form testing
* ✅ Form validation
* 📚 Technical documentation
* 🐙 GitHub project organization

---

# 🚀 Future Improvements

Potential improvements for a production-ready implementation could include:

* 📱 Deployment to an ODK-compatible mobile workflow
* 🔐 Additional data validation rules
* 📊 Automated submission and reporting workflows
* 🔄 Expanded conditional logic
* 🧪 Additional edge-case testing
* 📈 Integration with a backend data-processing workflow

These improvements are outside the current assignment scope.

---

# 📌 Assignment Submission

The completed project will be submitted through the required WhatsApp group using the specified format:

```text
Your Name - GitHub Repository Link
```

---

# 👩🏻‍💻 Author

**Smitha U M**

Computer Science and Engineering Student

---

# 📚 References

* ODK XLSForm Documentation
* ODK XLSForm Testing Resources
* Provided Criminal Risk Assessment Request Form

```
