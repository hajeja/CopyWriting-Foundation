# CopyWriting Foundation

Private workspace for Astro Product Copy Foundation, organized by **domain**. Files here supply guideline data; GitHub changes do **not** automatically update the Chrome Extension or Figma Plugin.

## Domain configs for testing

| Domain | Current active reference | Status |
| --- | --- | --- |
| Supplier | [Supplier v0.3.1](domains/supplier/astro-copy-config-v0.3.1-supplier-terminology.json) | 4 approved + enabled Supplier guidelines; others pending or hold; pilot baseline |
| Buyer | [Buyer v0.1.1](domains/buyer/buyer-guidelines-v0.1.1-pilot-approved.json) | 10 enabled; **approved for internal pilot** at user request, not formal policy |
| Mitra | [Mitra v0.1.1](domains/mitra/mitra-guidelines-v0.1.1-pilot-approved.json) | 9 enabled; **approved for internal pilot** at user request, not formal policy |

Read the [Supplier](domains/supplier/README.md), [Buyer](domains/buyer/README.md), and [Mitra](domains/mitra/README.md) notes for sources, scope and known caveats.

Historical v0.1.0 Buyer/Mitra draft JSONs are preserved for comparison, **not** for active use. Do not merge old and new versions into the AI prompt.

## Shared versus domain rules

- **Global Foundation:** writing principles, formatting, component patterns and decision guardrails. The current shared global baseline is under `global` in Supplier v0.3.1 JSON. Other domains reference that section as a transitional arrangement; the runtime must explicitly load the shared `global` and must not inherit `domains.supplier`.
- **Domain-specific Foundation:** exactly one selected domain at audit time. Do not combine Supplier, Buyer and Mitra rules or glossaries.
- **Project Memory:** business/project/feature context is separate from guidelines. It must not silently change Foundation or be assumed as formally confirmed knowledge.
- **Pilot approval:** Buyer/Mitra rules are enabled for trials. This does not prove any business claim or current design-system convention. Re-validate specific rules with domain owners before production use.

## Integration

- The Chrome Extension should support both **Audit This Page** and **Manual Copy Check** (paste text from a sheet, choose a domain and review with AI). The older regex/context-menu checker is not a substitute for the manual AI mode.
- The user must select/confirm domain when no project can be detected. For manual paste, project context is optional; domain is required.
- Confirm actual runtime rules loaded, version, enabled guideline count and applicable context before auditing.
- Preserve current Supplier working behavior; implement multi-domain loading without breaking existing audits.

Never commit API keys, confidential transactional data or secrets. Keep the repository private.
