# 🧪 XLSForm Testing

## 📌 Overview

The Criminal Risk Assessment XLSForm is designed to be validated and tested before final submission.

Testing helps ensure that the form structure, question types, choices, required fields, and conditional logic are configured correctly.

---

## 🔍 Testing Process

The following steps will be followed to test the XLSForm:

### 1. 📊 Validate the XLSForm

Upload the Excel XLSForm to an ODK-compatible XLSForm validation tool.

The validation process checks whether the workbook follows the expected XLSForm structure.

---

### 2. 📝 Check the Survey Sheet

Verify that:

- All required questions are present.
- Question types are appropriate.
- Field names are unique.
- Labels are clear.
- Required fields are configured correctly.
- Conditional fields contain the appropriate logic.

---

### 3. 🔘 Check the Choices Sheet

Verify that:

- All choice lists are defined.
- Choice names are unique within their lists.
- Choice labels are clear.
- Select-one and select-multiple questions reference the correct choice lists.

---

### 4. ⚙️ Check the Settings Sheet

Verify that:

- The form title is correct.
- The form ID is defined.
- The version is defined.
- The default language is specified.

---

### 5. 🔄 Test Conditional Fields

Conditional fields should appear only when their corresponding option is selected.

For example:

- Selecting **Other identification** should display the field for specifying the identification.
- Selecting **MB Driver's License with Photo** should display the licence number field.

---

### 6. ✅ Test Required Fields

Fields marked with an asterisk (`*`) in the original form should be checked to ensure that they cannot be skipped when required.

---

## 📋 Testing Checklist

- [ ] XLSForm structure validated
- [ ] Survey sheet checked
- [ ] Choices sheet checked
- [ ] Settings sheet checked
- [ ] Required fields tested
- [ ] Conditional fields tested
- [ ] Choice lists tested
- [ ] Form navigation checked
- [ ] Final form reviewed

---

## 🎯 Expected Result

The final XLSForm should successfully validate and represent the required structure and information from the original Criminal Risk Assessment Request form.

Any validation errors identified during testing should be corrected before the final project submission.
