# AI Voice Agents and Automation Systems for Service Businesses

I build AI voice agents and automation systems that answer calls, qualify leads, book appointments, update CRMs, and trigger follow-ups. My services also include service-business website development and B2B outbound infrastructure.

**Stack:** Retell AI, Bland AI, Synthflow, GoHighLevel, n8n, Twilio, Supabase, Next.js, Smartlead, InboxKit

**Try the voice agent:** [Interactive Retell preview](https://agent.retellai.com/preview/agent_ed761677e80ef1b36cf0a5b94e) (browser call, no phone number needed)

## Projects

| Project | Business problem | What I built | Evidence in this repo |
|---|---|---|---|
| [Bail-bonds intake receptionist](projects/bail-bonds-intake.md) | Urgent calls arrive after hours or while staff are busy | Voice agent that collects intake details, respects knowledge limits and escalates to a licensed agent | Qualification design, test scenarios, anonymized prospect response |
| [Retell AI conversational agent](projects/retell-conversational-agent.md) | Scripted bots fail when callers interrupt, change topic or give partial answers | Adaptive conversation design with branching, interruption handling and handoff rules | Live preview link, routing diagram, evaluator tests |
| [GoHighLevel speed-to-lead automation](projects/speed-to-lead-crm.md) | New leads go cold while nobody responds | Form or missed-call trigger to AI callback or SMS, discovery questions, CRM write, booking or callback task | Workflow specification, acceptance checklist, architecture diagram |
| [Service-business websites and lead capture](projects/service-business-websites.md) | Visitors cannot find the phone number or the form goes nowhere | Responsive sites with click-to-call, lead forms and integration-ready submissions | Scope and acceptance checklist, anonymized enquiry example |
| [B2B outbound outreach systems](projects/outbound-email-systems.md) | Cold email bounces, lands in spam or gets no replies | Prospect sourcing, verification, sending infrastructure, sequences and reply handling | Workflow, tooling, anonymized reply and campaign dashboard |

## Services at a glance

Concept graphics with fictional sample data; each links to its project page.

| | |
|---|---|
| [![Conversational AI agent](assets/05_Overview_Conversational_AI_Agent.jpg)](projects/retell-conversational-agent.md) | [![AI receptionist](assets/06_Overview_AI_Receptionist.jpg)](projects/bail-bonds-intake.md) |
| [![Speed-to-lead automation](assets/07_Overview_Speed_to_Lead.jpg)](projects/speed-to-lead-crm.md) | [![Cold email systems](assets/08_Overview_Cold_Email_Systems.jpg)](projects/outbound-email-systems.md) |
| [![Websites that convert](assets/09_Overview_Websites_That_Convert.jpg)](projects/service-business-websites.md) | |

## Executive assistant practice projects (fictional data)

Six practice projects showing how I would run common executive assistant work. Real client work is confidential, so I do not post real schedules, inboxes or systems. Everything here is rebuilt on a made-up company and made-up people, and none of it is paid client work. [Read why](CONFIDENTIALITY.md). See also [how I work](how-i-work.md).

| Project | What it shows |
| --- | --- |
| [Executive week and London trip](projects/ea-01-executive-week-and-trip.md) | Calendar conflicts, three time zones, travel options against a rule |
| [Inbox triage and morning brief](projects/ea-02-inbox-triage.md) | Sorting 25 emails, unsent drafts, a two minute brief |
| [Client onboarding board](projects/ea-03-client-onboarding-board.md) | The same week one plan in Trello and Asana |
| [Meeting prep, minutes and action items](projects/ea-04-meeting-minutes-and-actions.md) | Agenda, minutes from a fictional transcript, tracked actions |
| [Offsite budget and lodging shortlist](projects/ea-05-offsite-budget.md) | Options against a cap, a budget sheet with formulas |
| [Documents, slides, spreadsheets and designs](projects/ea-06-documents-slides-and-designs.md) | A briefing note, a kickoff deck, a budget workbook with formulas, a monday.com board and three Canva designs. Editable files are in [samples](samples) |

### A look at the work

Recreated illustrations and renders of the sample files. Each links to its project page.

| | | |
| --- | --- | --- |
| [![Executive week](assets/ea-s1-week.png)](projects/ea-01-executive-week-and-trip.md) | [![Inbox triage](assets/ea-s2-inbox.png)](projects/ea-02-inbox-triage.md) | [![Trello board](assets/ea-s3-board.png)](projects/ea-03-client-onboarding-board.md) |
| [![Asana project](assets/ea-s13-asana-project.png)](projects/ea-03-client-onboarding-board.md) | [![Minutes and actions](assets/ea-s4-minutes.png)](projects/ea-04-meeting-minutes-and-actions.md) | [![Offsite budget](assets/ea-s5-budget.png)](projects/ea-05-offsite-budget.md) |
| [![monday.com board](assets/ea-s12-monday-board.png)](projects/ea-06-documents-slides-and-designs.md) | [![Kickoff deck](assets/ea-s8-powerpoint-deck.png)](projects/ea-06-documents-slides-and-designs.md) | [![Briefing note](assets/ea-s7-word-briefing.png)](projects/ea-06-documents-slides-and-designs.md) |
| [![Canva invitation](assets/ea-s9-canva-invitation.png)](projects/ea-06-documents-slides-and-designs.md) | [![Canva agenda](assets/ea-s10-canva-agenda.png)](projects/ea-06-documents-slides-and-designs.md) | [![Canva weekly update](assets/ea-s11-canva-weekly-update.png)](projects/ea-06-documents-slides-and-designs.md) |

![Tools used and how I describe my level in each](assets/ea-s16-tools-used.png)

## How a typical system fits together

```mermaid
flowchart LR
  A[Inbound call or web form] --> B[Voice agent on Retell or Bland]
  B --> C{Intent and qualification}
  C -->|Qualified| D[n8n workflow]
  C -->|Urgent or sensitive| E[Human transfer or callback task]
  D --> F[GoHighLevel contact, pipeline stage, notes]
  D --> G[Calendar booking or scheduling task]
  D --> H[Permitted SMS or staff alert]
  F --> I[Follow-up workflow]
```

Each box is a component I design, configure and test. Which boxes are live in a given project depends on the client's platforms, consent rules and budget, and the project pages say which parts are implemented and which are proposed.

## What a connected agent should handle

1. **Answer calls:** take incoming and after-hours calls, identify the enquiry, answer approved business questions, escalate urgent or sensitive requests to a person.
2. **Qualify prospects:** ask what service is needed, where, when and how urgently, adapting questions to the answers received.
3. **Book appointments:** check calendar availability where integrated, and distinguish a confirmed booking from sending a scheduling link.
4. **Update CRM records:** create or update contacts, notes, opportunities, tags and pipeline stages without creating duplicates.
5. **Follow up:** trigger permitted SMS messages, reminders, staff alerts or callback tasks.
6. **Handle exceptions:** interruptions, background noise, unanswered questions, human handoffs, webhook failures and calendar errors.

## Speed to lead

Speed to lead is the time between a new enquiry and the first meaningful response. A **30-second initial response is a design target**, not a measured benchmark or a guarantee. Actual speed depends on provider latency, automation rules and testing.

## Voice-agent design considerations

Prompts and business knowledge; branching and follow-up questions; interruption sensitivity and natural turn-taking; response pacing; background-noise handling; calm phrasing under stress; unsupported-answer boundaries; transfer and callback rules. The linked Retell preview is a way to **try the conversation**, not proof that every setting or integration is active.

## Tools and integration boundaries

- **Voice:** Retell AI and Bland AI (built and tested). Synthflow (used to generate and configure receptionist agents; no separate shipped build documented in this repo yet). Vapi and GoHighLevel Voice AI (familiar, no shipped build in this repo).
- **CRM and workflows:** GoHighLevel, n8n, REST APIs and webhooks, Supabase, contact records and lead-routing logic.
- **Telephony and messaging:** Twilio, A2P 10DLC registration, consent capture, STOP handling, delivery monitoring.
- **Possible integrations, scoped per project:** Cal.com, Calendly, Google Calendar, HubSpot, Zoho, Frappe CRM, Notion, Slack, Jotform, Jobber, Housecall Pro, ServiceTitan.
- **U.S. texting:** A2P 10DLC registration is required for business texting on long codes. Registration by itself does not grant permission to message; documented consent and opt-out handling are still needed.

## Evidence and privacy

These are **demonstrations, design samples and technical documentation**. The images in `assets/` are either recreated and anonymized illustrations based on real outreach and demonstrations, or concept graphics with fictional sample data (marked as such); they are not pixel-exact screenshots, verified testimonials or performance reports. Example scenarios use fictional information. The executive assistant projects are practice work rebuilt on invented data because real client work is confidential; [read why](CONFIDENTIALITY.md). Credentials, client records, personal contact details and direct phone-demo numbers are excluded. Work enquiries and pre-contract communications stay on Upwork where required.
