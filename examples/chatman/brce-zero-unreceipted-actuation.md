# SPR — BRCE and Zero Unreceipted Actuation

- SELECT, CONSTRUCT, and DO are different authority domains.
- Planning may select possibilities without gaining execution authority.
- Construction may manufacture executable intent without actuating it.
- DO requires explicit admission through the bounded execution path.
- BRCE is the exclusive DO path.
- Zero unreceipted actuation is a system invariant, not a logging preference.
- Raw input, model output, proof output, semantic derivation, and hooks have no ambient execution authority.
- Hooks manufacture intents; hooks never actuate directly.
- Authority must be explicit, scoped, revocable, and bound to the exact subject.
- Execution must produce a receipt that can be independently checked.
- A side effect without a receipt is a protocol violation even when the side effect was desired.
- Replay verifies that the same admitted intent traverses the same lawful boundary.
