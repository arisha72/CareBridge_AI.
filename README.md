# CareBridge AI
**Helping families care for loved ones from anywhere.**

CareBridge AI is a proposed family healthcare coordination product focused on helping older adults manage everyday health routines while keeping authorised family members informed when support is needed.

> **Project status:** Product concept / portfolio case study. This repository documents the product proposal and its planned MVP. It does not contain a deployed application or a clinically validated medical system.

## The problem
When older adults live separately from their children or caregivers, routine healthcare information can become fragmented. Medication schedules, prescription details, symptoms, and emergency contacts may sit across paper notes, phone calls, and messaging apps. Families can struggle to know whether a dose was acknowledged or whether help is needed.

CareBridge explores a coordinated experience for:
- Older adults who need simple, accessible ways to manage daily health routines.
- Family members who support them remotely.
- Caregivers who may help maintain schedules and respond to alerts.

## Product concept
A shared family-care workspace that connects medication routines, prescription information, family communication, and emergency preparedness.

### Proposed MVP
| Capability | User value | MVP behaviour |
|---|---|---|
| Medication planner | Makes schedules easier to follow | Create schedules, send reminders, record user-reported dose status |
| Prescription capture | Reduces manual re-entry | Capture an image and extract candidate text for human verification |
| Family dashboard | Improves remote visibility | Show consented adherence events and relevant alerts |
| Family notes | Keeps family communication in one place | Send and view text or voice notes |
| Emergency profile | Makes key information easier to find | Store emergency contacts and user-entered health details |
| SOS flow | Helps initiate a response | User-triggered alert to configured contacts with location only after permission |

## Product principles
1. **Human confirmation for clinical information.** OCR output must never silently become an active medication instruction.
2. **Consent-led sharing.** Older adults control which family members can view their information.
3. **Accessible by default.** Large touch targets, plain language, voice-friendly flows, and low-friction navigation.
4. **Fail-safe emergency design.** Clearly communicate whether an alert was sent and whether a contact acknowledged it. Never imply that an ambulance has been dispatched unless an integration confirms it.
5. **Decision support, not diagnosis.** The product does not diagnose, prescribe, or change treatment.

## Repository guide
- [`docs/PRD.md`](docs/PRD.md) — product requirements and acceptance criteria
- [`docs/personas-and-journeys.md`](docs/personas-and-journeys.md) — target users and key journeys
- [`docs/roadmap.md`](docs/roadmap.md) — phased scope and prioritisation
- [`docs/architecture.md`](docs/architecture.md) — conceptual system architecture and data flow
- [`docs/metrics-and-validation.md`](docs/metrics-and-validation.md) — pilot metrics and validation plan
- [`docs/safety-privacy.md`](docs/safety-privacy.md) — healthcare safety, consent, and privacy principles
- [`research/assumptions-and-evidence.md`](research/assumptions-and-evidence.md) — claims that require external validation
- [`docs/original-concept.pdf`](docs/original-concept.pdf) — cleaned copy of the original idea document
- [`docs/original-concept.docx`](docs/original-concept.docx) — editable source document

## Proposed technology direction
The original concept considered Flutter or React Native, FastAPI or Node.js, PostgreSQL, OCR services, speech services, and cloud infrastructure. These are options, not implemented choices. The architecture document keeps provider choices replaceable.

## Current limitations
- No production code, live integrations, or deployed prototype are included.
- No user research findings are claimed in this repository; interviews and pilot testing are proposed next steps.
- Market sizing, industry statistics, pricing, CAC, LTV, and competitor comparisons from the original idea document are hypotheses pending source verification.
- Emergency calling, location sharing, OCR, speech recognition, and health-data storage require technical, legal, security, and operational validation before launch.

## Suggested next steps
1. Interview older adults, family caregivers, and professional caregivers.
2. Test the medication reminder and family-sharing flows with low-fidelity prototypes.
3. Define consent, account recovery, and emergency escalation behaviour.
4. Build a narrow MVP before attempting predictive healthcare features.
5. Run a small usability pilot and report observed results separately from targets.

## Disclaimer
CareBridge AI is a product concept for portfolio and learning purposes. It is not a medical device, emergency service, or substitute for professional medical advice. Do not use this concept repository to make clinical decisions.
