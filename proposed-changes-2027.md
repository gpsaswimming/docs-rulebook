# Proposed Changes for 2027

Working list of proposed rulebook changes for the 2027 season. Each item notes the location(s), the issue, and a proposed fix. Nothing here is adopted — this is a staging document for Board/Rules review.

---

## Exhibition swimmers — who marks them, and where it's stated

**Status:** Draft / needs review

**Locations:**
- `officials.md:151` — Coaches section: "Are responsible for declaring all entries in SwimTopia and ensuring that all exhibition entries are flagged as such."
- `conduct-of-meets.md:98` — Maximum Scoring Entrants: "All other entrants from a team shall be marked as exhibition."
- `conduct-of-meets.md:119` — Entry deadline: teams "Ready to Merge" by 12:00 PM.
- `conduct-of-meets.md:122–123` — Home GPSA Rep verifies exhibition-requirement compliance and relocates exhibition swimmers.

**Issue:**
1. The coach's obligation to flag exhibition entries lives only in `officials.md`. The participation rule that *creates* exhibition swimmers (`conduct-of-meets.md:98`) states entries "shall be marked as exhibition" in the passive voice and never names the coach as the responsible party or points to where the duty is defined. A reader in the participation section can't tell *who* marks them or *where*.
2. The cross-reference in `officials.md:151` points to "Pre-Meet Requirements... for entry deadlines," but the actual deadline (`conduct-of-meets.md:119`, "Ready to Merge" by 12:00 PM) doesn't itself mention exhibition flagging. The chain works but is loose.

**Proposed fix:**
- Add a cross-reference (or an explicit "the coach is responsible for flagging these in SwimTopia") at `conduct-of-meets.md:98`, so the obligation is discoverable from the rule that generates it.
- Optionally tighten the `officials.md:151` cross-reference so it lands on the specific deadline item.

---

## Removal of participants during a meet — scattered authority and gaps

**Status:** Draft / needs review

**Locations:**
- `officials.md:47` — Referee: controls abusive language/actions by "any swimmer or spectator"; warn-first, then has the offender ejected via the home-team GPSA Rep and pool manager.
- `officials.md:165,167` — Marshal (Optional): with Referee concurrence, may remove "anyone" behaving unsafely, using profane/abusive language, or disrupting the meet.
- `conduct-of-meets.md:51–57` — Suspended/Banned Individuals: request-to-leave, escalating to forfeit if they refuse.
- `code-of-conduct/index.qmd:43,47` — Code of Conduct violations "during meets will be reported to the Referee for disposition"; removal from GPSA is a Board-level sanction after the fact.

**Issue:**
The rulebook has no single, general "removal for breaking the rules or Code of Conduct" authority. Instead it has three narrow, partly overlapping pathways with gaps:
1. **On-the-spot removal is tied only to abusive/unsafe/disruptive behavior**, not to rule-breaking generally. A participant flagrantly violating competition rules (short of disruption) has no removal pathway — only DQ/scoring remedies.
2. **The only broad removal power (Marshal, "anyone") is optional.** When no Marshal is appointed, the fallback is the narrower referee clause (`officials.md:47`), limited to "abusive language or actions" and scoped to "swimmer or spectator."
3. **Coaches and GPSA Reps sit in a gray zone.** `officials.md:47` names only swimmers/spectators; the Marshal clause says "anyone" but is optional. A misbehaving coach has no clear on-site removal path.
4. **The Code of Conduct → Referee handoff is vague.** "Disposition in accordance with GPSA rules" (`code-of-conduct/index.qmd:43`) doesn't cite a specific removal mechanism; the reader must connect it to `officials.md:47`/`:167`.

**Proposed fix:**
- Decide whether GPSA wants a general on-site removal authority for rule/Code-of-Conduct violations (not just abusive/disruptive behavior), and where it should live.
- Consolidate or cross-reference the removal authorities so they read as one coherent escalation ladder (warn → cease/desist → remove → forfeit).
- Clarify who removal applies to — swimmers, spectators, coaches, and GPSA Reps.
- Make the Code of Conduct "disposition" language point to the specific removal mechanism.

---

## Tied dual meet — how it counts toward division standings

**Status:** Draft / needs Board decision

**Locations:**
- `scoring.md:15–17` — "Ties" only covers ties *within an event* (points for the tying and next positions are added and split). Silent on a whole dual meet ending in a tie.
- `awards.md:21` — Division Awards tiebreaker for teams with "identical records": head-to-head first, then total points scored in dual meets against the other tied teams.

**Issue:**
The 2026 season produced the league's first tied dual meet (Beaconsdale 209 – Wythe 209, both Blue division). The rulebook does not define:
1. **How a tie weights a team's standing.** Records now need a W‑L‑**T** shape, but there's no rule for whether a tie counts as a half-win, is ignored, or something else when ordering the division for trophies. (The results archive has been fixed to track ties in a separate column and to stop miscrediting a tie as an away win / home loss, but it orders by wins only pending this decision.)
2. **How a tie interacts with the `awards.md:21` tiebreaker.** The head-to-head rule assumes the tied teams' dual meet had a winner. If that meet was itself a tie, head-to-head is inconclusive and the rule should say it falls through to the total-points step.

**Proposed fix:**
- Board to decide how a tied dual meet counts toward division standings (e.g., half-win / ignored / other) and state it in `scoring.md` or `awards.md`.
- Amend `awards.md:21` so the tiebreaker explicitly handles a tied head-to-head meet (fall through to total points among tied teams).

---

## Missing or unusable time — no rule for a swim with no valid time

**Status:** Draft / needs review

**Locations:**
- `conduct-of-meets.md:157–166` — Time Recording: lists the recording methods and collection process, but stops at "the timer records the swimmer's time."
- `conduct-of-meets.md:83` — "stopwatches are recommended as backup even if using a timing system."
- `officials.md:121` — Head Timer: starts a watch on every race; "the time of this watch shall be used if a Lane Timer's watch fails."
- `officials.md:171,173` — Timing Equipment Operator advises the Referee of system problems; acknowledges meets may run *without* backup stopwatches.

**Issue:**
The rulebook covers how times are captured and a per-lane fallback (the Head Timer's watch when a Lane Timer's watch fails), but is silent on the case where a swim ends up with **no valid time at all** — a system or timer failure with no usable backup. It does not state:
1. **What to record.** There is no rule that a swim with no valid time is recorded as a no-time (published as "NT"), nor any prohibition on fabricating a time or substituting the swimmer's seed time.
2. **The precedence of electronic vs. backup times.** That an electronic time is official unless the system fails, in which case a backup time is used, is only *implied* (via `officials.md:121` for hand timing, and the Time Drops wiki page) — never stated as a general rule.
3. **Who decides.** Nothing assigns the call — clear the time vs. attempt to reconstruct it — to the referee.

Because GPSA scores by place, a missing time never affects the outcome; the gap is about the *record*, not the score. Interim decision-guidance now lives in the wiki ([Official Times](https://wiki.gpsaswimming.org/official-times), plus the Referee and Scorekeeper guides) as a practice standard, pending a rule.

**Proposed fix:**
- Add a "No valid time" provision to `conduct-of-meets.md` Time Recording: a swim with no usable time and no backup is recorded as a no-time (published "NT"); a time shall not be fabricated or taken from the swimmer's seed.
- State the precedence explicitly: an electronic time is official unless the timing system fails, in which case the backup (Head Timer / stopwatch) time is used; if no backup time exists, the swim is a no-time.
- Assign the call to the referee (in consultation with both GPSA Representatives when the cause is unclear).

---
