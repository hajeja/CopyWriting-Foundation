# CopyWriting Foundation

Private workspace for Astro Product Copy Foundation, organized by **domain**. This repository stores copywriting guidance and supporting domain configuration; it does not automatically change deployed Figma Plugins or Chrome Extensions.

## Domains

| Domain | Status | Files |
| --- | --- | --- |
| **Supplier** | **v0.3.1 pilot baseline** · 4 approved/enabled Supplier guidelines; other rules pending/hold | [Guidelines and glossary](domains/supplier/README.md) |
| **Buyer** | **v0.1 extracted draft** · 10 unapproved items, derived from an uploaded UX Writing Playbook | [Draft guide](domains/buyer/README.md) |
| **Mitra** | **v0.1 research draft** · 9 unapproved items, based on prior Fulfillment/Mitra field discussions | [Draft guide](domains/mitra/README.md) |

## Working principles

- **Global Foundation** (principles, formatting, component patterns) and **domain guidance** (context, tone, glossary) should remain conceptually separate.
- For now the global baseline is stored inside [Supplier v0.3.1 JSON](domains/supplier/astro-copy-config-v0.3.1-supplier-terminology.json) under `global`; Buyer and Mitra JSON refer to that section without copying Supplier-specific guidelines. This is a **transitional reference**, not an automatic runtime import. A later loader migration can extract `global` to a dedicated shared module without changing active Supplier behavior.
- Never enforce a draft, pending, or hold rule as a confirmed policy.
- Never invent missing business rules, operational behavior, or user-facing claims.
- Keep the repository private. Don't commit actual supplier records, secrets, or API keys.

## Integration

Only Supplier v0.3.1 has been the existing pilot baseline. Buyer and Mitra files are **documentation/config drafts**; they're not enabled in the Figma plugin or Chrome extension until reviewed and wired into runtime.

Please review each domain README before using its JSON.
