# 🗂️ Field Mapping

## 📌 Overview

This document shows how the fields from the original **Criminal Risk Assessment Request** form were mapped into the ODK XLSForm.

The mapping helps maintain a clear connection between the original paper form and its digital implementation.

---

## 👤 Personal & Consent Information

| # | Original Form Field | XLSForm Type | Required |
|---|---|---|---|
| 1 | Date | `date` | ✅ Yes |
| 2 | Signature of person being assessed | `text` | ✅ Yes |
| 3 | Unconsented Witness | `text` | ❌ No |
| 4 | First Name | `text` | ✅ Yes |
| 5 | Second Name | `text` | ❌ No |
| 6 | Last Name | `text` | ✅ Yes |
| 7 | Date of Birth | `date` | ✅ Yes |
| 8 | Gender | `select_one` | ✅ Yes |
| 9 | Other Last Names Used | `text` | ❌ No |
| 10 | Other First Names Used / Also Goes By | `text` | ❌ No |
| 11 | Current Address | `text` | ✅ Yes |
| 12 | Current PH#s | `text` | ✅ Yes |
| 13 | City/Province or Country of Birth | `text` | ✅ Yes |

---

## 🪪 Identification Information

| # | Original Form Field | XLSForm Type | Required |
|---|---|---|---|
| 14 | Birth Certificate | `select_multiple` | — |
| 15 | Social Insurance Card | `select_multiple` | — |
| 16 | Manitoba Health Card | `select_multiple` | — |
| 17 | Treaty Card | `select_multiple` | — |
| 18 | Other (specify ID) | `text` | Conditional |
| 19 | MB Driver's License with Photo | `select_multiple` | — |
| 20 | Licence Number | `text` | Conditional |

---

## 📝 Risk Assessment Request

| # | Original Form Field | XLSForm Type | Required |
|---|---|---|---|
| 21 | Name of Person Being Assessed | `text` | ✅ Yes |
| 22 | Name of Agency Submitting Request | `text` | ✅ Yes |
| 23 | Reason for Risk Assessment | `select_multiple` | ✅ Yes |
| 24 | Assigned Worker | `text` | ✅ Yes |
| 25 | Date of Last Criminal Risk Assessment | `date` | ❌ No |
| 26 | Submitting Designate | `text` | ✅ Yes |
| 27 | Designate PH# | `text` | ✅ Yes |
| 28 | Designate Email# | `text` | ✅ Yes |
| 29 | Designate Fax# | `text` | ❌ No |
| 30 | Request Date | `date` | ✅ Yes |

---

## 🔄 Conditional Fields

Some fields are displayed based on the identification option selected.

For example:

- **Other (specify ID)** appears when `Other` identification is selected.
- **MB Driver's License licence number** appears when the Manitoba Driver's License option is selected.

This allows the digital form to remain organized and show additional information only when applicable.

---

## 📊 XLSForm Components

The mapping is implemented using the three main XLSForm worksheets:

| Worksheet | Purpose |
|---|---|
| `survey` | Defines questions, labels, required fields and form logic |
| `choices` | Defines selectable options |
| `settings` | Defines form configuration |

---

## 🎯 Mapping Objective

The objective of this mapping is to ensure that the important fields and structure of the original Criminal Risk Assessment Request are represented appropriately in the digital ODK XLSForm.
