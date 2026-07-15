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

## Correcting a time after the meet is certified

**Status:** Rules Committee agreed — needs drafting into rule text

**Locations:**
- `conduct-of-meets.md:195–196` — Home GPSA Rep "Lock out changes in Meet Maestro and transfer results" and submit within 24 hours. This is the closest thing to a "certification" moment, but the rulebook never uses that term or says what may change afterward.
- `conduct-of-meets.md:210–225` — Post-Meet Protests / Rules Committee Authority: the only existing post-meet correction pathways, but they are *protest-driven* and *score-driven*, not a general procedure for fixing a bad recorded **time**.

**Issue:**
The rulebook has no concept of a meet being "certified," and no procedure for correcting an individual recorded time after results are finalized. It does not state who may change a time, under what circumstances, or in which direction. Because GPSA scores by place, a bad time never changes a meet outcome — but it corrupts the swimmer's record and any time-based standards/seeding downstream, so a bounded correction path is needed.

**Rules Committee decision (to be drafted):**
After a meet is certified, a recorded time may be reviewed and changed only through one of two pathways:
1. **Both GPSA Representatives and the Referee** convene to review the flagged times; or
2. **The Rules Committee** reaches out to the affected teams to review the flagged times.

In *either* pathway, the only times that may be changed are **obvious timing errors** — e.g., a 50-length time recorded against a 100-length event, or a physically impossible time — and only where the error gave the swimmer a **faster** time than it should have been. If the recorded error made the swimmer **slower** than actual, it may **not** be changed.

**Proposed fix:**
- Define "certified" (tie it to the `:195` lockout / transfer, or to a later confirmation step) so "after certification" has a fixed meaning.
- Add the two review pathways and the one-directional "faster-only" correction rule to the Post-Meet or Protests section.
- Clarify what "flagged times" means and who flags them (results tooling / GPSA Reps) so the trigger for a review is unambiguous.

---

## Timing-system hierarchy during the meet — electronic time is primary

**Status:** Rules Committee agreed — needs drafting into rule text

**Locations:**
- `conduct-of-meets.md:160,162` — Electronic Timing System (Time Drops) captures times automatically; Lane Timer Sheets "may be used ... as backup with electronic timing systems."
- `officials.md:121` — Head Timer's watch "shall be used if a Lane Timer's watch fails."
- **Related staging item above** — "Missing or unusable time" already flags that the precedence of electronic vs. backup times is only *implied*, never stated. This decision supplies that rule; the two items should be drafted together.

**Issue:**
The rulebook implies but never states that the electronic time governs. There is no rule preventing a watch time from being substituted simply because it is more favorable to the swimmer.

**Rules Committee decision (to be drafted):**
The hierarchy of timing systems must be upheld. When Time Drops is in use, a watch time may be used **only** if Time Drops had a system error or failure for that swim. A watch time being more favorable is **not**, by itself, grounds to use it over the electronic time.

**Proposed fix:**
- State the precedence explicitly in Time Recording: the electronic (Time Drops) time is official unless the system failed for that swim, in which case the backup (Head Timer / watch) time is used.
- Prohibit substituting a backup time merely because it is faster/more favorable.
- Draft alongside the "Missing or unusable time" item so precedence and no-valid-time rules read as one provision.

---

## Timer configuration per lane — 1 or 3 on one system, 2 only when split

**Status:** Rules Committee agreed — needs drafting into rule text

**Locations:**
- `conduct-of-meets.md:89` — "By mutual agreement of both GPSA Representatives, teams may use two or three timers per lane instead of the standard one timer per lane."
- `officials.md:123` — Lane Timer "may simultaneously operate two dissimilar devices (one watch and one button) but not two similar devices."
- `officials.md:135` — "a. If two timers are used, the times must be averaged. If three timers are used, the middle time must be used."

**Issue:**
The current two/three-timer allowance (`conduct-of-meets.md:89`) and the averaging rule (`officials.md:135a`) permit two timers on the **same** system (e.g., two watches averaged). The Committee's decision disallows that configuration, so the existing averaging rule for two timers no longer fits and must be amended.

**Rules Committee decision (to be drafted):**
Timers shall be staffed either **one (1) or three (3) per lane using the same timing system**. A **two (2)-timer** configuration is permitted **only** when the timers are split across systems — one on Time Drops and one on a watch as backup — never two on the same system.

**Proposed fix:**
- Revise `conduct-of-meets.md:89` to state the allowed configurations: 1 or 3 per lane on one system, or 2 only when split (Time Drops + watch backup).
- Amend `officials.md:135a` — the "two timers averaged" case no longer applies to two same-system timers; averaging is not used for the split (Time Drops + watch) configuration, where the electronic time governs per the hierarchy item above.
- Reconcile with `officials.md:123` (one person operating two dissimilar devices) so device-count vs. timer-count rules don't contradict.

---
