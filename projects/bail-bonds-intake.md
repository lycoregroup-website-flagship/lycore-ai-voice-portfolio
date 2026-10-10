# U.S. Bail-Bonds AI Intake Receptionist

**Type:** conversational voice-agent demonstration for U.S. bail-bond agencies.

## Business problem

Urgent bail enquiries may arrive after hours or while staff are busy. An AI receptionist can collect the minimum useful intake information and route the caller to a qualified person without giving legal advice or promising an outcome.

## Intake and qualification design

- Ask whether the enquiry concerns the caller or someone else.
- Ask where the arrest happened and which jail or county is involved, if known.
- Collect appropriate callback details and clarify the urgency.
- Respect the agency's service-area and business-hour rules.
- Explain that case-specific bond questions need a qualified team member.
- Identify when to transfer, notify staff or request a callback.

## Try fictional scenarios

- “My brother was arrested last night. I don't know what jail he's at. What do you need from me?”
- “I'm calling about someone arrested in another county. Can your agency help?”
- “I need to speak to a licensed bail agent. Can you arrange a callback?”

Do not supply real arrested-person details in a test. No claim is made about a production deployment or measured service outcomes. The publicly callable demonstration number is intentionally not included in this Upwork-facing repository.

**Engineering evidence:** conversation prompts, qualification paths, escalation rules, knowledge boundaries and example call tests. CRM writes and live transfers should only be described as built if verified.
