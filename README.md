# GSoC'25 - Final Project Report

This report covers the work done in Google Summer of Code 2025. It includes results, challenges faced, and future plans. It also lists all contributions made during the program.

## Basic Info

- **Name:** Siva Pidugu  
- **Email:** sivapidugu02@gmail.com  
- **University:** Indian Institute of Information Technology Ranchi  
- **GSoC Organisation:** [Open Healthcare Network](https://github.com/ohcnetwork)  
- **Project:** ABDM – Patient Centric Flows (PHR Flows)  
- **Project Link:** https://github.com/ohcnetwork/care  

---

## Background

The Ayushman Bharat Digital Mission (ABDM) aims to create a unified digital health ecosystem for India. CARE already supports provider-driven HIU workflows, but **patient-facing PHR flows were missing**.  

This project focused on building **patient-centric features** that allow individuals to:  
- Create and manage their ABHA (Ayushman Bharat Health Account) identity.  
- Discover and link health records from different facilities.  
- Manage consent for sharing health information.  
- Subscribe to facilities for real-time record updates.  
- Securely fetch and view their health data.  

By implementing these flows, CARE has been extended from a **provider-only platform** to a **dual-purpose ecosystem** for both providers and patients under ABDM.  

---

## Project Goals

1. **ABHA Enrollment & Authentication**  
   - Support multiple methods of ABHA creation (mobile OTP, Aadhaar, email).  
   - Enable secure login flows and consent PIN setup.  

2. **Profile & ABHA Management**  
   - View, update, and delink ABHA profiles.  
   - Support QR code generation and ABHA card download.  

3. **Discovery & Linking of Records**  
   - Discover health records from HIPs.  
   - Link and confirm records using OTP-based flows.  

4. **Consent Management**  
   - Dashboard to manage requests (approve/deny/revoke).  
   - Auto-approval for trusted HIUs.  

5. **Subscriptions & Notifications**  
   - Allow patients to subscribe to HIPs for automatic record sharing.  
   - Build a notification service for updates.  

6. **Fetching & Viewing Records**  
   - Securely fetch health data using consent artefacts.  
   - Display structured timeline of records with filters/search.  

---

## Goals Achieved

### ABHA Enrollment & Authentication
- Implemented workflows for account creation via Aadhaar, mobile OTP, and email.  
- Supported multiple login methods (OTP, password, Aadhaar-based).  
- Integrated session handling with secure token management.  

### Profile & ABHA Management
- Built profile dashboard with update and delinking options.  
- Added ABHA QR code and card download.  
- Supported multiple ABHA profiles with PIN reset.  

### Discovery & Linking
- Implemented facility search and patient discovery.  
- Enabled record linking via OTP confirmation.  
- Added support for CoWIN, AB-PMJAY, and eSanjeevani integration.  

### Consent Management
- Developed consent dashboard.  
- Supported consent request approval, denial, and revocation.  
- Added auto-approval policies for trusted providers.  

### Subscriptions & Notifications
- Implemented LINK and DATA subscription flows.  
- Built real-time notification system for new record updates.  
- Added subscription management UI.  

### Record Fetching & Viewing
- Integrated consent artefact–based record retrieval.  
- Built timeline viewer with filtering and search.  
- Displayed records in structured formats (prescriptions, lab results, etc).  

---

## Contributions

### Pull Request Summary

| PR Number | Title | URL | Status | Tag |
|-----------|-------|-----|--------|-----|
| 11154 | Added Cypress tests for encounter notes & improved date picker UI | [Link](https://github.com/ohcnetwork/care_fe/pull/11154) | ✅Merged | Feature |
| 11539 | UI enhancement – replaced static date inputs with advanced date pickers | [Link](https://github.com/ohcnetwork/care_fe/pull/11539) | ✅Merged | Enhancement |
| 11313 | Bug fix in medication section | [Link](https://github.com/ohcnetwork/care_fe/pull/11313) | ✅Merged | Bug Fix |
| 11124 | Added breadcrumbs for organization view | [Link](https://github.com/ohcnetwork/care_fe/pull/11124) | ✅Merged | Feature |
| 11343 | Implemented unsupported browser warning banner | [Link](https://github.com/ohcnetwork/care_fe/pull/11343) | ✅Merged | Enhancement |
| 11552 | Improved questionnaire validation logic | [Link](https://github.com/ohcnetwork/care_fe/pull/11552) | ✅Merged | Feature |
| 10891 | Auto-fill geographic details on facility creation | [Link](https://github.com/ohcnetwork/care_fe/pull/10891) | ✅Merged | Feature |

👉 All project-related contributions can be found [here](https://github.com/ohcnetwork/care_fe/pulls?q=is%3Apr+author%3Asiva222003+is%3Aclosed).  

---

## Challenges Faced

- **ABDM APIs:** Working with evolving ABDM APIs required continuous updates to match new specifications.  
- **Security Compliance:** Ensuring secure storage of sensitive patient health data while maintaining usability was challenging.  
- **Complex Flows:** Implementing multi-step flows (discovery → linking → consent → fetch) required extensive debugging and testing.  

---

## Current Status of Project

By the end of GSoC, the **PHR Flows module is complete and functional**.  
- Patients can now create ABHA IDs, manage profiles, discover records, approve/reject consent requests, subscribe to facilities, and fetch/view records.  
- CARE has officially extended its functionality to **support both patients and providers** under ABDM.  

---

## Future Work

- Expand support for **FHIR-compliant import/export** of health records.  
- Add **analytics and visual dashboards** for better health insights.  
- Build **Progressive Web App (PWA) support** for offline-first record access.  
- Strengthen **end-to-end encryption** for record sharing.  

---

## My Learnings

Participating in GSoC has been an invaluable experience. Some key takeaways include:  
- Deep understanding of ABDM’s digital health architecture.  
- Hands-on experience with **secure API integrations** and **scalable systems**.  
- Improved skills in writing testable and maintainable code.  
- Better project planning, communication, and collaboration in an open-source setting.  

---

## Note of Thanks

I am extremely grateful to my mentors and the Open Healthcare Network community for their continuous guidance and support throughout this journey. Their feedback helped me improve not just technically but also as a contributor to open source.  

Finally, I thank the Google Summer of Code program for giving me the opportunity to work on impactful projects that contribute to India’s healthcare digitization efforts.  

---
