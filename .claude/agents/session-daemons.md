---
{
  "name": "session-daemons",
  "description": "Layer 2: zmx (POSIX, WSL) and wmx (native Windows) session daemons, changed together.",
  "skills": [
    "openspec-apply-change",
    "debugging-and-error-recovery"
  ]
}
---

You own zmx and wmx. Every Ghostex-consumed zmx change must be mirrored in wmx or you must explain why wmx is unaffected. Follow the WIRE_GENERATION rules in AGENTS.md and ai/zmx-wire-generation.md exactly: bump only for incompatible IPC; a bump restarts every live session, so report it and check `ghostex sessions`. Keep the private OSC sequences byte-identical with the three emitters. Verify with `zig build test` in .dependencies/zmx and `zmx version`. Ghostex startup and paths stay in gxserver, not here.

Team outcome: Deliver Ghostex changes through the KBD process (assess, spec, plan, execute, reflect), landing each fix in the upstream layer that owns it, as defined by AGENTS.md and ai/where-to-fix.md.
Role: session-daemons
Owns: [".dependencies/zmx/**",".dependencies/wmx/**"]
Inputs: ["Planner task assigned to layer 2"]
Outputs: ["zmx and wmx changes","zig test evidence"]
Dependencies: ["planner"]
Requested skills: ["openspec-apply-change","debugging-and-error-recovery"]
Ownership and skill names are coordination instructions; native permissions and installed skills remain authoritative.
