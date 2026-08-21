# World in Context — Workflow Map

Αυτό είναι ο απλός χάρτης του συστήματος — όχι δεύτερο MASTER.

## Η λογική σε μία γραμμή
**MASTER = κανόνες → AGENT = εκτέλεση → ARCHIVE = μνήμη**

## 1. MASTER
`agent/WORLD-IN-CONTEXT-MASTER.md`

Η canonical πηγή για τους μόνιμους editorial και Daily Run κανόνες.

Αν αλλάζει μόνιμος κανόνας:
**MASTER + CHANGELOG**.

## 2. AGENT
`agent/agent-v2.md`

Η λειτουργική περιγραφή του `world-in-context-agent-v2`.
Ο Agent εφαρμόζει το MASTER. Δεν είναι δεύτερο MASTER.

## 3. SUPPORT FILES
- `agent/source-registry.json` — μητρώο πηγών
- `agent/source-policy-v1.md` — κανόνες πηγών/cross-check
- `agent/editorial-rules.json` — machine-readable editorial rules
- `agent/CHANGELOG.md` — ιστορικό μόνιμων αλλαγών

## 4. ARCHIVE
- `data/archive-story-schema.json` — δομή archive
- `data/stories.json` — διαχρονική μνήμη ongoing stories
- `data/daily/YYYY-MM-DD.json` — ημερήσιο record κάθε briefing

## 5. DAILY FLOW
MASTER
→ Archive / Continuity
→ Main Source Sweep
→ Regional Blind-Spot Sweep
→ Verification
→ Shortlist + Editorial Scoring
→ Proposed Cards + Level 2
→ HUMAN APPROVAL
→ Same-Day Delta Check ~19:00
→ Editorial Lock
→ Final Cards + Level 2 Analysis
→ QA
→ HTML / Visual Production
→ Social + UTM
→ Publication
→ Archive Update / Measurement

## 6. DAILY START
**World in Context — Briefing [DATE]**

`Ξεκίνα το σημερινό briefing με το world-in-context-agent-v2 και εφάρμοσε το MASTER / Daily Run Protocol. Μην προχωρήσεις σε HTML ή εικόνες πριν από editorial έγκριση.`

## 7. 19:00 DELTA
**World in Context — Same-Day Delta Check [DATE]**

`Εφάρμοσε το SAME-DAY DELTA CHECK του MASTER χρησιμοποιώντας ως baseline τις ήδη εγκεκριμένες κάρτες της σημερινής ημέρας. Μην κάνεις αλλαγές χωρίς editorial έγκριση.`

## 8. ΤΙ ΔΕΝ ΧΡΕΙΑΖΕΤΑΙ ΣΤΟ ACTIVE /agent/
Το παλιό ξεχωριστό `daily-run-protocol-v1.md` δεν χρειάζεται ως δεύτερη ενεργή πηγή κανόνων, επειδή το Daily Run Protocol υπάρχει πλέον στο canonical MASTER.

Αν θέλεις να το κρατήσεις ιστορικά, βάλε το σε `archive/legacy/`.
