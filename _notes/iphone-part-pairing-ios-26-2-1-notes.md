# iOS 26.2.1 — iPhone Part Pairing Failure (Technical Notes)

> Canonical article (Russian):  
> https://service36.ru/blog/privyazka-displeya-akkumulyatora-iphone-ios-262-2621/

## Scope
Devices:
- iPhone 12 and newer

Components:
- Display
- Battery

System:
- Repair Assistant
- Genuine / Genuine Used pairing

---

## Known Good Behavior (≤ iOS 26.2)

Repair Assistant successfully:
- paired genuine used displays
- restored True Tone
- paired genuine used batteries
- restored Battery Health
- paired service parts
- accepted some diagnostic parts

---

## Broken Behavior (iOS 26.2.1)

Observed consistently:
- Repair Assistant launches
- diagnostics complete
- pairing step fails silently

Applies to:
- genuine used parts
- service parts
- parts with original controllers and flexes

No successful pairing cases observed.

---

## Symptoms

- “Unknown Part” warning persists
- True Tone unavailable
- Battery Health unavailable
- No user-facing error explaining failure

---

## Likely Failure Points (Hypotheses)

- backend eligibility check failure
- request/response mismatch between OS and Apple servers
- changed pairing flags not handled server-side
- silent rejection without error propagation

---

## Important Notes

- This behavior contradicts Apple’s published repair policy
- No documentation indicates an intentional change
- Behavior matches previous Apple pairing regressions

---

## Recommendation

Treat iOS 26.2.1 as a **broken release** for part pairing.
Do not assume policy changes until officially documented.
