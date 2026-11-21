# Safety, Privacy, and Trust

CareBridge handles potentially sensitive health-related information. Safety and privacy are core product requirements, not later enhancements.

## Clinical boundaries
- The product is not a diagnostic or prescribing system.
- Do not recommend a dose, change a schedule, or interpret symptoms as a diagnosis.
- OCR output is a draft. A user must verify every relevant field before use.
- Unclear prescriptions should be referred to a qualified clinician or pharmacist.
- Reminder acknowledgement is a user report, not evidence of ingestion.

## Consent and access
- Sharing is opt-in, granular, visible, and revocable.
- The care recipient should be able to review who has access.
- Family members receive only the minimum information required for the agreed purpose.
- Provide clear account recovery and a process for handling loss of capacity or disputed access; obtain legal and clinical guidance before defining this.

## Emergency experience
- SOS must be user-initiated and clearly explain what will be shared.
- Do not promise ambulance dispatch or emergency response unless a verified integration supports it.
- Show alert delivery, failure, and acknowledgement as distinct states.
- Define offline and no-response fallbacks before launch.
- Avoid false reassurance from a successful push-notification request; delivery does not mean a person has read the alert.

## Data protection baseline
- Collect only data required for a stated feature.
- Encrypt data in transit and at rest.
- Use least-privilege access and secure secrets management.
- Maintain audit logs for access and permission changes.
- Define retention, deletion, backup, breach response, and vendor data-processing requirements.
- Avoid placing sensitive health information in analytics events or application logs.

## Pre-launch reviews
Obtain qualified review of applicable Indian privacy and health regulations, medical-device implications, emergency-service integrations, consent language, data residency, and contracts with OCR / speech / cloud vendors. This document is a product checklist, not legal advice.
