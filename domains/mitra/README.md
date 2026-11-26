# Mitra Copy Guidelines

**Current trial config:** [v0.1.1 — Approved for Pilot](./mitra-guidelines-v0.1.1-pilot-approved.json) · **9 enabled guidelines**.

**Original source snapshot:** [v0.1.0 — Research Draft](./mitra-guidelines-v0.1-draft.json) (preserved unchanged).

## Approval scope and source

On **26 November 2026**, the project owner requested Mitra guidelines be marked `approved` and `enabledForPilot` **for internal hands-on testing**. This is **not** formal Ops/BPI approval and does **not** independently validate field-user research hypotheses.

Derived from earlier Mitra/Fulfillment field-user discussions about:
- Direct, contextual, task-focused instructions
- Clear object, required action, and next step
- Error reasons and recovery where confirmed
- Avoiding unfamiliar internal English/system jargon
- Reducing unnecessary SPV clarifications
- Copy in UI, SOP, Working Instructions, OJT and operational communications

The uploaded Astro Playbook's `2.4. Our Tone.pdf` differentiates Fulfillment from Buyer. The serious / straightforward / simple tone is a provisional reference, **not a signed-off Mitra voice guide**.

## Pilot guidelines

Nine candidate rules now enabled for pilot testing. `glossaryCandidates` remain **unconfirmed terminology references**; do not enforce them as official glossary.

### Safety and business constraints

- Never invent operational steps, scan quantities, statuses, SLA, permissions, recovery, escalation or ownership.
- Identify the exact user role and workflow; Mitra is not always equivalent to all Fulfillment or WMS users.
- Do not import Supplier-specific terminology restrictions or Buyer style rules.
- User approval to pilot does not approve business facts.

## Integration

The `v0.1.1` file has `reviewStatus: approved`, `enabledForPilot: true`, `approvalScope: pilot_only`. Plugin/extension runtimes must explicitly load it; GitHub files do not sync themselves.

Future work: Validate actual UI/SOP/OJT samples with Operations, Design and researchers; establish a proper Mitra glossary and approval owner.
