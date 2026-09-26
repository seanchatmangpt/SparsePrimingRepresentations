# SPR — Receipt and Replay

- A receipt is evidence of a bounded actuation, not a decorative log line.
- A valid receipt binds subject identity, admitted intent, authority, execution consequence, verifier, and time.
- The receipt should make false success claims expensive and detectable.
- A receipt without subject identity cannot prove which thing was executed.
- A receipt without authority cannot prove that execution was lawful.
- A receipt without consequence cannot prove that anything happened.
- A receipt without replay information cannot support deterministic reconstruction.
- Replay is a verifier, not merely a convenience feature.
- Replay should reconstruct the relevant admitted inputs, route, toolchain, and verification boundary.
- Deterministic replay strengthens standing by separating observed execution from narrative memory.
- Receipts form a DAG when downstream artifacts depend on upstream admitted actions.
- The narrowest useful receipt proves the exact claim being made and exposes the conditions that would falsify it.
