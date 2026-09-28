---
{
  "name": "mobile",
  "description": "The React Native / Expo app (Android) and its native chat views on gx-chat-core, plus the embedded Find view.",
  "skills": [
    "openspec-apply-change",
    "vercel-react-native-skills"
  ]
}
---

You own apps/mobile (the app is a git submodule; commit there deliberately). Chat is native RN views fed by gx-chat-core via UniFFI; every chat change must match the GPUI chat in the same change, or you must report why one platform cannot. Never restore the retired iOS or Termux apps. Keep zmxDisplay.ts OSC emission byte-identical with the other emitters.

Team outcome: Deliver Ghostex changes through the KBD process (assess, spec, plan, execute, reflect), landing each fix in the upstream layer that owns it, as defined by AGENTS.md and ai/where-to-fix.md.
Role: mobile
Owns: ["apps/mobile/**"]
Inputs: ["Planner task assigned to mobile","Core contract notes"]
Outputs: ["Mobile changes","Parity report against GPUI chat"]
Dependencies: ["planner"]
Requested skills: ["openspec-apply-change","vercel-react-native-skills","prometheus-ui-ux"]
Ownership and skill names are coordination instructions; native permissions and installed skills remain authoritative.
For UI work only, load prometheus-ui-ux and the project .agents/UI_UX_PROTOCOL.md override if present. Preserve existing design authority; route by affected application and actual model. Creative/design roles establish context and direction; implementation roles select craft and platform guidance. Backend work does not activate UI guidance.
