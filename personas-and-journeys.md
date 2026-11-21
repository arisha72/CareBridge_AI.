# Personas and User Journeys

These are **provisional personas** derived from the product concept, not research-validated profiles.

## Persona 1 — Older adult / care recipient
- Wants independence and control over daily routines.
- May find complex app navigation, small text, or repeated data entry difficult.
- Needs reminders that are understandable and easy to acknowledge.
- Concern: family monitoring may feel intrusive if sharing is not transparent.

## Persona 2 — Adult child / remote family supporter
- Lives in another city or country.
- Wants a reliable view of shared routine-care updates without repeatedly calling.
- Needs clear distinctions between confirmed events and missing information.
- Concern: false reassurance from stale or incomplete data.

## Persona 3 — Informal caregiver
- Helps with daily routines, appointments, or medication organisation.
- Needs clear task information and permission-limited access.
- Concern: unclear responsibility when a reminder is missed or an alert is not acknowledged.

## Journey A — Set up a medication reminder
1. Care recipient opens medication planner.
2. Enters medication details and schedule from the clinician's instructions.
3. Reviews the schedule and confirms it.
4. Receives a reminder at the selected time.
5. Records taken, skipped, or leaves it unconfirmed.
6. If sharing is enabled, the authorised family dashboard reflects the event.

**Failure states to design:** reminder delivery fails; device is offline; schedule is incomplete; user reports a dose after the reminder window.

## Journey B — Add a prescription
1. User captures a prescription image.
2. System extracts candidate text.
3. Extracted fields are marked unverified.
4. User checks each field against the original prescription.
5. Ambiguous or unclear details are not guessed.
6. User confirms the schedule or seeks clarification from a qualified professional.

## Journey C — Trigger an SOS
1. User intentionally activates SOS.
2. App shows the contacts and information to be shared.
3. User confirms.
4. System attempts to deliver the alert and optional location.
5. User sees delivery status; contacts can acknowledge.
6. If delivery fails, the app displays a clear fallback instruction and does not imply help is on the way.
