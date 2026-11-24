# Supplier Copy Foundation

This folder contains the Supplier-domain configuration for Astro Product Copy Foundation. The repository also supports future domain foundations for Mitra and Buyer.

## Current configuration

- **File:** [astro-copy-config-v0.3.1-supplier-terminology.json](./astro-copy-config-v0.3.1-supplier-terminology.json)
- **Version:** `0.3.1-pilot-draft`
- **Status:** Working pilot baseline; **not final BPI policy**
- **Canonical domain:** `supplier` (normalize legacy `vendor` domain selection to `supplier`)
- **Enabled Supplier guidelines:** 4 approved items, selected by `reviewStatus === "approved" && enabledForPilot === true`

This is **one complete Foundation JSON**, containing:
- Global copy principles and formatting rules
- Component patterns and decision guardrails
- Supplier guidelines, applicability, approval states, and exceptions
- Supplier glossary and terminology guidance

## Important behavior

- In user-visible Supplier-domain copy, prefer **Supplier** over **Vendor** and **Seller** regardless of target user (including internal users). Flag terminology violations without automatically changing original source text.
- Never invent business rules, document requirements, consequences, or system behavior. Request missing material context.
- Do not treat guidelines on hold, rejected, or pending confirmation as approved requirements.
- Review copy for clarity, accuracy, conciseness, and user action. A wording rewrite is not always necessary.
- Do not modify Figma layer names, code identifiers, or backend schema to enforce user-facing copy terminology.

## Integration with Figma Plugin and Chrome Extension

1. Load the same canonical config into each tool's runtime (GitHub storage alone does not update a deployed plugin/extension).
2. Confirm the applicable `global` and `domains.supplier` objects actually reach the AI audit request.
3. Filter Supplier guidelines by approval and enabled status.
4. Keep the review instruction, context handling, and response schema consistent across tools.
5. Test with the Supplier Invoice trial page and known before/after examples before claiming parity.

**If the extension says "third Foundation JSON was not found":** inspect its source loader and expected filenames. Do **not** create placeholder JSONs or combine outdated v0.3 with v0.3.1 just to silence the message.

## Remaining review items

- Confirm the exact rejected BPI guideline from the full final review record.
- Some Supplier rules and glossary entries remain draft, hold, or pending confirmation.
- Validate plugin/extension behavior, security, publishing, and API-key handling independently.

Keep this repo **private**; do not commit API keys, actual Supplier data, or other secrets.
