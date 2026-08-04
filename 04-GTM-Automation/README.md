# 🤖 GTM Email Discovery & Validation Automation using n8n

> Built an automated workflow using **n8n**, **HTTP APIs**, and **Google Sheets** to generate business email patterns, validate email addresses, and create outreach-ready contact lists.

---

# 📌 Business Problem

Sales teams often know a prospect's **first name**, **last name**, and **company domain**, but do not have a verified business email.

Manually generating multiple email combinations and validating each email through verification tools is repetitive, time-consuming, and difficult to scale.

This workflow automates the entire process—from generating email patterns to validating them—helping GTM teams prepare accurate contact data for outbound campaigns.

---

# 🎯 Objectives

- Automate business email generation
- Validate email addresses using an API
- Reduce manual prospect research
- Improve lead quality
- Build outreach-ready contact lists

---

# 🛠 Technologies Used

- n8n
- Google Sheets
- HTTP Request Node
- Email Verification API
- JSON
- Workflow Automation

---

# 🔄 Workflow

```text
Google Sheets
(First Name + Last Name + Domain)
                │
                ▼
Generate Email Patterns
                │
                ▼
HTTP Request Node
                │
                ▼
Email Verification API
                │
                ▼
Process JSON Response
                │
                ▼
Select Valid Email
                │
                ▼
Update Google Sheets
```

---

# 📸 Step 1 – Complete n8n Workflow

The workflow automates the entire email verification process by connecting Google Sheets, generating multiple email combinations, validating each email through an API, and updating the final verified email automatically.

![n8n Workflow](../assets/images/n8n-workflow.png)

---

# 📸 Step 2 – HTTP Request Configuration

The HTTP Request node sends generated email addresses to an email verification API and receives a JSON response containing the validation status for each email.

The workflow analyses this response to identify the first valid business email.

![HTTP Request](../assets/images/01-n8n-http-validation-workflow.png)

---

# 📸 Step 3 – Email Pattern Generation

Multiple business email formats are automatically created using the prospect's first name, last name, and company domain.

Examples include:

- firstname@company.com
- firstname.lastname@company.com
- lastname@company.com
- firstinitiallastname@company.com

These generated patterns are stored in Google Sheets before validation.

![Email Pattern Generation](../assets/images/02-email-pattern-generation-sheet.png)
---

# 📸 Step 4 – Final Validation Results

After validating every generated email, the workflow automatically updates Google Sheets with:

- Final Verified Email
- Email Validation Status
- Completion Status

This creates an outreach-ready contact database without manual intervention.

![Final Validation Results](../assets/images/03-final-email-validation-results.png)

---

# 📊 Business Impact

This automation:

- Reduced manual email verification effort
- Improved lead data accuracy
- Accelerated outbound prospecting
- Standardised email validation
- Built GTM-ready contact lists
- Reduced repetitive research tasks

---

# 💡 Skills Demonstrated

- n8n Workflow Development
- GTM Automation
- HTTP API Integration
- Email Verification
- Google Sheets Automation
- JSON Processing
- Lead Enrichment
- Sales Operations
- Workflow Design

---

# 🚀 Future Improvements

- Apollo API Integration
- CRM Synchronisation
- Bulk Lead Enrichment
- AI-Based Lead Scoring
- Automated Outreach Sequences

---

## 🔗 Related Projects

- 🎯 [ICP Research](../01-ICP-Research)
- 🚀 [Lead Generation](../02-Lead-Generation)
- 🌐 [Website Technology Detector](../03-Website-Technology-Detector)

🏠 [Back to Portfolio Home](../)
