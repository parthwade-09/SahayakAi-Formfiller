# AI Sahayak – Voice Based Form Filler

## 1. Project Information

**Project Name:** AI Sahayak – Smart Voice-Based Form Filler  
**Team Name:** Team Edamame  
**Team Leader:** Parth Wade  
**Tech Lead:** Ritesh Verma  
**Category:** AI for Bharat – Community & Public Systems  
**Theme:** Inclusion, Accessibility, Civic Access

---

## 2. Problem Statement

Many citizens in India face difficulties filling government and public service forms due to:

- Low digital literacy
- Language barriers
- Complex English forms
- Lack of typing skills
- Dependence on cyber cafes or agents
- Time and money loss

As a result, people fail to access schemes like scholarships, pensions, subsidies, and welfare programs.

---

## 3. Proposed Solution

AI Sahayak is a voice-first AI assistant that helps users fill government forms automatically using speech.

Users speak answers in their local language and the system:

- Converts speech to text
- Understands answers using NLP
- Detects form fields
- Auto-fills the form
- Generates ready-to-submit PDF

**No typing required.**

---

## 4. Objectives

- Enable voice-based form filling
- Support regional languages
- Reduce dependency on agents
- Improve accessibility for rural users
- Work in low bandwidth conditions
- Provide simple and intuitive interface

---

## 5. Target Users

- Rural citizens
- Elderly users
- Farmers
- Students applying for scholarships
- Daily wage workers
- Government help centers (CSCs)

---

## 6. Functional Requirements

### FR1 – Voice Input
System shall accept user responses through microphone.

**Acceptance Criteria:**
- AC1.1: User can activate voice recording via button or voice command
- AC1.2: System provides visual feedback during recording
- AC1.3: User can stop recording manually or automatically after silence detection

### FR2 – Speech to Text
System shall convert voice to text using STT.

**Acceptance Criteria:**
- AC2.1: Audio is converted to text with >85% accuracy for clear speech
- AC2.2: Conversion completes within 3 seconds for 10-second audio clips
- AC2.3: System handles background noise gracefully

### FR3 – Language Support
System shall support multiple Indian languages.

**Acceptance Criteria:**
- AC3.1: System supports at least Hindi and English initially
- AC3.2: User can select preferred language before starting
- AC3.3: Language selection persists across sessions

### FR4 – Intent Understanding
System shall extract required information (name, age, address, etc.)

**Acceptance Criteria:**
- AC4.1: System correctly identifies personal information fields (name, age, gender, etc.)
- AC4.2: System extracts dates in various spoken formats
- AC4.3: System normalizes addresses to standard format
- AC4.4: System handles spelling corrections for names

### FR5 – Form Detection
System shall identify form fields automatically using OCR/templates.

**Acceptance Criteria:**
- AC5.1: System detects common government form fields with >90% accuracy
- AC5.2: System supports PDF and image form formats
- AC5.3: System handles both structured and semi-structured forms

### FR6 – Auto Filling
System shall populate detected fields with extracted data.

**Acceptance Criteria:**
- AC6.1: System maps extracted data to correct form fields
- AC6.2: System validates data format before filling (e.g., date format, phone number)
- AC6.3: System highlights fields that couldn't be auto-filled

### FR7 – PDF Generation
System shall export filled forms as downloadable PDF.

**Acceptance Criteria:**
- AC7.1: Generated PDF maintains original form layout
- AC7.2: Filled data is clearly visible and properly formatted
- AC7.3: PDF is generated within 5 seconds
- AC7.4: PDF file size is optimized for mobile sharing

### FR8 – User Verification
System shall allow users to review and edit before submission.

**Acceptance Criteria:**
- AC8.1: User can view all filled fields in a summary view
- AC8.2: User can edit any field manually
- AC8.3: System highlights fields with low confidence scores
- AC8.4: User must explicitly confirm before PDF generation

### FR9 – Low Bandwidth Mode
System shall function in low internet environments.

**Acceptance Criteria:**
- AC9.1: System works with 2G/3G connections
- AC9.2: Audio is compressed before upload
- AC9.3: System provides offline fallback for basic operations
- AC9.4: Progress is saved locally and synced when connection improves

### FR10 – Secure Data Handling
System shall ensure privacy and secure storage.

**Acceptance Criteria:**
- AC10.1: All data transmission uses HTTPS
- AC10.2: Personal data is encrypted at rest
- AC10.3: User data is deleted after PDF generation (or within 24 hours)
- AC10.4: System complies with data privacy regulations
- AC10.5: No third-party tracking or analytics on sensitive data

---

## 7. Non-Functional Requirements

### NFR1 – Performance
- Response time < 3 seconds for voice-to-text conversion
- Form filling completes within 2 minutes for standard forms
- PDF generation < 5 seconds

### NFR2 – Usability
- Simple, intuitive UI requiring minimal instructions
- Large buttons and clear visual feedback
- Support for low-literacy users

### NFR3 – Compatibility
- Mobile responsive (works on smartphones)
- Supports Android 8+ and iOS 12+
- Works on low-end devices (2GB RAM minimum)

### NFR4 – Scalability
- Handle 1000+ concurrent users
- Support multiple form templates
- Extensible architecture for adding new languages

### NFR5 – Security
- Data encryption in transit and at rest
- No permanent storage of sensitive information
- Secure API endpoints

### NFR6 – Reliability
- 99% uptime during business hours
- Graceful degradation in low bandwidth
- Error recovery and retry mechanisms

---

## 8. Constraints

- Limited team size (hackathon team)
- First-year level tech stack
- Must run on low-end devices
- Short hackathon timeline
- Limited budget for cloud services

---

## 9. Assumptions

- Users have basic smartphone access
- Government forms follow structured format
- Internet available at least intermittently
- Users can speak clearly in their chosen language
- Forms are in digital format (PDF/image)

---

## 10. Success Metrics

- **Time saved:** Reduce form filling time by 50%
- **Accuracy:** >90% field accuracy without manual correction
- **User satisfaction:** >4/5 rating from test users
- **Error reduction:** <5% manual errors in filled forms
- **Adoption:** Increase in scheme participation by target users

---

## 11. Unique Selling Proposition (USP)

- Voice-first civic assistant
- Multilingual support for Indian languages
- Bharat-focused solution
- No typing required
- Low data usage
- Social impact driven
- Accessible to low-literacy users

---

## 12. Future Enhancements

- WhatsApp integration for form submission
- SMS alerts for application status
- Direct submission to government portals
- Document scanning and OCR
- AI chatbot for scheme guidance and eligibility
- Fully offline mobile app
- Support for 10+ Indian languages
- Integration with Aadhaar for auto-fill
- Voice-based OTP verification
