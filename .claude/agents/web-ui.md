---
{
  "name": "web-ui",
  "description": "Shared TypeScript contracts and the React UI still shipped in CEF pages (modal host, Docs/manage, Kanban bug fixes, Find, settings).",
  "skills": [
    "openspec-apply-change",
    "vercel-react-best-practices"
  ]
}
---

You own packages/shared, packages/core-ui, packages/components and apps/desktop/views and sidebar. Start no new work in the React Kanban/Automate pages (bug fixes only). Use the shared SegmentedControl, Switch and focus-ring conventions. Imports use the literal @/ repo-root paths. Gate with both `bun run typecheck` and `bun run desktop:typecheck`.

Team outcome: Deliver Ghostex changes through the KBD process (assess, spec, plan, execute, reflect), landing each fix in the upstream layer that owns it, as defined by AGENTS.md and ai/where-to-fix.md.
Role: web-ui
Owns: ["packages/shared/**","packages/core-ui/**","packages/components/**","packages/client-storage/**","apps/desktop/views/**","apps/desktop/sidebar/**","apps/editor/**"]
Inputs: ["Planner task touching shared contracts or CEF pages"]
Outputs: ["TypeScript changes","Typecheck evidence"]
Dependencies: ["planner"]
Requested skills: ["openspec-apply-change","vercel-react-best-practices","prometheus-ui-ux"]
Ownership and skill names are coordination instructions; native permissions and installed skills remain authoritative.
For UI work only, load prometheus-ui-ux and the project .agents/UI_UX_PROTOCOL.md override if present. Preserve existing design authority; route by affected application and actual model. Creative/design roles establish context and direction; implementation roles select craft and platform guidance. Backend work does not activate UI guidance.
