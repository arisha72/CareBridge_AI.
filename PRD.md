# Product Requirements Document — CareBridge AI

**Document status:** Draft product proposal  
**Product stage:** Concept / pre-validation  
**Primary market hypothesis:** Indian families supporting older adults remotely

## 1. Product summary
CareBridge AI is a family healthcare coordination concept. It aims to help older adults manage routine medication tasks and make selected information visible to trusted family members, with explicit consent.

## 2. Problem statement
Older adults and remote family members may rely on disconnected tools for medication schedules, prescription details, health updates, and emergency contacts. This can create missed reminders, repeated calls, uncertainty, and delays in sharing important information.

This problem statement is a hypothesis to validate through interviews; it should not be treated as a measured finding.

## 3. Goals
- Make medication schedules easier to create and follow.
- Let users record whether a scheduled dose was taken, skipped, or left unconfirmed.
- Give authorised family members a clear view of shared routine-care updates.
- Reduce friction when retrieving emergency contacts and essential user-entered information.
- Keep the experience usable for people with limited confidence using smartphones.

## 4. Non-goals for the MVP
- Diagnosing conditions or predicting medical events.
- Recommending, changing, or calculating medication doses.
- Automatically interpreting an OCR result as a confirmed prescription.
- Replacing doctors, pharmacists, caregivers, or emergency services.
- Continuous passive monitoring or fall detection.
- Medication ordering, insurance, hospital, or ambulance dispatch integrations.

## 5. Users and permissions
**Older adult / care recipient:** owns their profile and controls sharing permissions.  
**Family supporter:** sees only information the care recipient has authorised.  
**Caregiver (future role):** receives limited task access explicitly granted by the care recipient.

A family relationship alone must not grant access to private health information.

## 6. Core user stories and acceptance criteria

### A. Medication schedule
**Story:** As a care recipient, I want to add a medication schedule so that I can receive reminders at the times I choose.

Acceptance criteria:
- User can enter medicine name, schedule, start date, optional end date, and instructions as supplied by their clinician.
- The app displays the saved schedule for user review before activation.
- Reminder status is recorded as `taken`, `skipped`, or `unconfirmed`; the system does not infer ingestion.
- Editing or deleting a schedule is auditable and visible to the account owner.
- The app clearly states that reminders do not replace clinician instructions.

### B. Prescription capture
**Story:** As a care recipient, I want to capture a prescription so that I can reduce manual data entry.

Acceptance criteria:
- Image capture requires user permission.
- OCR output is labelled as an unverified draft.
- Medicine name, strength, dosage, and frequency are shown for manual review.
- No schedule is activated until the user confirms the extracted details.
- Unreadable or ambiguous fields are flagged for pharmacist/clinician clarification rather than guessed.

### C. Family sharing
**Story:** As a care recipient, I want to choose which family member can see my routine-care updates.

Acceptance criteria:
- Sharing is opt-in and revocable.
- The user can see who has access and what information is shared.
- A family member receives access only after an invitation is accepted.
- Revoking access prevents future access and triggers a clear confirmation.

### D. Family dashboard
**Story:** As an authorised family supporter, I want to see shared medication events so that I can follow up when something remains unconfirmed.

Acceptance criteria:
- Dashboard distinguishes taken, skipped, and unconfirmed.
- A missed reminder is not represented as proof that medication was not taken.
- Data freshness and last update time are visible.
- The dashboard does not expose information outside the granted permission scope.

### E. Emergency profile and SOS
**Story:** As a care recipient, I want my emergency details to be available to trusted contacts when I trigger an SOS.

Acceptance criteria:
- User can maintain emergency contacts and optional profile fields.
- SOS requires an intentional user action and displays what will be shared.
- Location is shared only with permission and only when device capability is available.
- The interface distinguishes `alert sent`, `delivery failed`, and `contact acknowledged`.
- The product does not claim emergency services have been contacted unless a verified integration confirms it.

## 7. MVP prioritisation
**P0:** account/profile, consent and sharing controls, medication schedule, reminder/event status, emergency contacts.  
**P1:** family dashboard, family notes, prescription capture with manual verification.  
**Later:** voice interface, IVR, teleconsultation, wearables, fall detection, predictive insights, service marketplace.

## 8. Functional requirements
- Authentication and secure account recovery.
- Role- and consent-based access control.
- Medication schedule CRUD and reminder delivery.
- Event history with timestamps and status.
- OCR capture pipeline with explicit review step.
- Notification preferences and delivery status.
- Audit log for sensitive access and permission changes.

## 9. Non-functional requirements
- Accessibility: readable typography, high contrast, large controls, plain language.
- Reliability: retry and failure states for notifications; no silent success.
- Security: encryption in transit and at rest, least-privilege access, secure secrets management.
- Privacy: data minimisation, retention controls, deletion workflow, and clear consent.
- Observability: monitor notification failures, OCR confidence, and application errors without logging unnecessary health details.

## 10. Open questions
- Which reminder channels are most usable: in-app, push, SMS, or voice call?
- What level of health information do older adults want to share?
- How should the product handle a phone being switched off or offline?
- What is the safest fallback when an emergency contact does not respond?
- Which language and accessibility needs should be supported first?
