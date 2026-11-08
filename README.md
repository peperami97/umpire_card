# Cricket Umpires Record Cards Suite

Professional, field-tested, print-ready cricket umpire record cards designed for match officials across four distinct cricket formats:
1. **T20 Limited Overs** (20 Overs / Side)
2. **T50 One-Day** (50 Overs / Side)
3. **Timed Match: 110 Split** (*Saracens Hertfordshire Premier Cricket League* regulations)
4. **Multiday Matches** (2-Day, 3-Day, and 4-Day multi-innings fixtures)

All cards are formatted as standard **two-sided A4 documents** (Page 1: 1st Innings & Setup; Page 2: 2nd Innings, Target/Chase, Regulations & Sign-Off). They are fully optimized for printing double-sided on cardstock (160–220 gsm) or folding into standard umpire pocket wallets and PVC protective sleeves.

---

## Quick Navigation & Files

| Format | Interactive HTML | Ready-to-Print PDF | Match Structure |
| :--- | :--- | :--- | :--- |
| **Portal Hub** | [`index.html`](file:///home/ben/Work/index.html) | — | Master selector & reference guide |
| **T20 Limited Overs** | [`t20_umpire_card.html`](file:///home/ben/Work/t20_umpire_card.html) | [`pdfs/t20_umpire_card.pdf`](file:///home/ben/Work/pdfs/t20_umpire_card.pdf) | 20 ov / side &bull; Max 4 ov/bowler |
| **T50 One-Day** | [`t50_umpire_card.html`](file:///home/ben/Work/t50_umpire_card.html) | [`pdfs/t50_umpire_card.pdf`](file:///home/ben/Work/pdfs/t50_umpire_card.pdf) | 50 ov / side &bull; Max 10 ov/bowler |
| **Timed: 110 Split (Herts)** | [`timed_110_umpire_card.html`](file:///home/ben/Work/timed_110_umpire_card.html) | [`pdfs/timed_110_umpire_card.pdf`](file:///home/ben/Work/pdfs/timed_110_umpire_card.pdf) | 110 ov pool &bull; Max 58 ov 1st inn &bull; Last Hr |
| **Multiday (2/3/4 Day)** | [`multiday_umpire_card.html`](file:///home/ben/Work/multiday_umpire_card.html) | [`pdfs/multiday_umpire_card.pdf`](file:///home/ben/Work/pdfs/multiday_umpire_card.pdf) | 4 Innings &bull; Sessions &bull; Follow-on |

---

## Detailed Format Specifications

### 1. T20 Limited Overs Record Card
* **Duration:** 20 overs per innings (1 innings per side).
* **Bowler Over Limit:** Maximum **4 overs** per bowler (or $\frac{\text{Total Overs}}{5}$ in rain-shortened matches).
* **Powerplay (PP):**
  * **Overs 1 to 6 (Mandatory PP):** Maximum **2 fielders** permitted outside the 30-yard fielding circle.
  * **Overs 7 to 20 (Non-PP):** Maximum **5 fielders** permitted outside the 30-yard fielding circle.
  * *Rain reductions:* PP adjusted dynamically per standard playing conditions table.
* **Over Rate & Timing Control:**
  * Standard allocation: **85 minutes** per innings (or 80 minutes under certain league rules).
  * Checkpoint milestones: Over 5 (+21m), Over 10 (+42m), Over 15 (+63m), Over 20 (Target Cut-Off Time).
  * **In-Match Penalty:** If over 20 has not commenced by the target cut-off time, only **4 fielders** (instead of 5) are permitted outside the circle for all remaining overs.
* **Special Deliveries:**
  * **Free Hit:** Awarded for all No-Balls (front-foot, fielding restriction, or above-waist height).
  * **Short-Pitched Bouncers:** Maximum **1 short delivery** above shoulder height per over. (Dedicated `[ ]` tick box on card).
* **Rain / DLS Calculation:** Minimum **5 overs** per side required to constitute a match. Dedicated recalculation box for time lost, revised overs, revised PP, and DLS target.

---

### 2. T50 One-Day Limited Overs Record Card
* **Duration:** 50 overs per innings (1 innings per side).
* **Bowler Over Limit:** Maximum **10 overs** per bowler (reduced proportionally in delayed matches).
* **Over-by-Over Grid:** Structured into two parallel 25-over columns (Overs 1–25 and Overs 26–50) with dedicated callouts:
  * **PP1 (Overs 1–10):** Mandatory Powerplay (max 2 fielders outside circle).
  * **PP2 (Overs 11–40):** Standard fielding restriction (max 4 fielders outside circle).
  * **PP3 (Overs 41–50):** Final death overs (max 5 fielders outside circle, or league-specific variation).
* **Drinks Breaks:** Pre-scheduled at the end of **Over 17** and **Over 34** (5 minutes each, highlighted in yellow).
* **Over Rate Target:** 3 hours 30 minutes (210 minutes total, ~14.3 to 17 overs/hour).
* **Bowler Analysis Grid:** Accommodates up to 8 bowlers with a **10-over tick tracker** (`[1][2][3][4][5][6][7][8][9][10]`), maidens, runs, wickets, extras, and youth fast bowling category.
* **Bouncers:** Maximum **2 short-pitched deliveries** above shoulder height per over (3rd called No-Ball).
* **DLS / Rain Calculations:** Minimum **20 overs** per side required for a valid match.

---

### 3. Timed Match: 110 Split (*Saracens Hertfordshire Premier Cricket League*)
Strictly modeled on the traditional declaration / timed match playing conditions specified in the Hertfordshire Premier Cricket League handbooks:
* **Total Match Overs Pool:** **110 Overs** shared between both teams.
* **1st Innings Batting Cap:**
  * The team batting first can bat a maximum of **58 overs**.
  * If Team 1 has not declared or been bowled out by the end of the 58th over, their innings is **compulsorily closed**.
* **2nd Innings Allocation ("The Split / Carry-Over Formula"):**
  $$\text{Team 2 Overs} = 110 - \text{Overs Bowled in 1st Innings}$$
  * Guaranteed base: **52 overs** (if Team 1 bats the full 58 overs).
  * **Tactical Declaration Incentive:** If Team 1 declares after 45 overs, Team 2 receives $110 - 45 = \mathbf{65\text{ overs}}$ to chase the target!
  * The card features a dedicated **110 Split & Carry-Over Worksheet** to instantly calculate and verify available overs.
* **"The Last Hour" Regulations:**
  * Must be signaled by the umpires at the designated clock time (typically **5:30 PM** or 1 hour before scheduled close, or upon reaching the final threshold).
  * A minimum of **20 overs** (or 17 overs if delayed) must be bowled in the Last Hour.
  * The card includes a **1 to 20 Countdown Checklist** to cross off overs as they are completed.
* **Hertfordshire League Bonus Points System:**
  * **Batting Bonus Points (awarded starting from 110 runs!):**
    - 110 runs = 1 pt
    - 125 runs = 2 pts
    - 140 runs = 3 pts
    - 155 runs = 4 pts
    - 170 runs = 5 pts
    - 185 runs = 6 pts
    - 200 runs = 7 pts
    - 215 runs = 8 pts
    - 230 runs = 9 pts
    - 245 runs = 10 pts *(Maximum 10 batting bonus points)*
  * **Bowling Bonus Points:**
    - 3 wickets = 1 pt
    - 5 wickets = 2 pts
    - 7 wickets = 3 pts
    - 9 wickets = 4 pts
    - All out 10 wickets = 5 pts *(Maximum 5 bowling bonus points)*
  * **Result Tracking:** Outright Win, Winning Draw, Losing Draw, Tie, Abandoned.
* **Bowler Limits:** **No individual bowler over limit** (unlimited overs permitted). ECB Fast Bowling Directives apply for youth bowlers.

---

### 4. Multiday Match Record Card (2-Day, 3-Day, 4-Day)
* **Match Scope:** Complete 4-innings coverage (Team A 1st Innings, Team B 1st Innings, 3rd Innings of match, 4th Innings chase).
* **Daily Session Quotas:**
  * Scheduled for **96 to 100 overs per day** (minimum 15 overs per hour).
  * **Session 1 (Morning):** 11:00 to 13:00 (Lunch interval: 40 minutes).
  * **Session 2 (Afternoon):** 13:40 to 15:40 (Tea interval: 20 minutes).
  * **Session 3 (Evening):** 16:00 to Stumps (with up to 30 mins / 8 overs added for lost time).
  * Dedicated **Session-by-Session Over Rate Log** for Day 1, Day 2, and Day 3.
* **Follow-On Calculator:**
  * 4-Day / 5-Day Match: **200 runs lead** required to enforce.
  * 3-Day Match: **150 runs lead** required.
  * 2-Day Match: **100 runs lead** required.
  * Immediate status toggle: `[ ] YES` or `[ ] NO`.
* **New Ball Log:** Available after **80 overs** (or 85/100 overs depending on competition). Trackers for over taken, score, and overs bowled with new ball across all innings.
* **Final Day "Last Hour":** Countdown tracker for the mandatory **minimum 15 overs** commencing 60 minutes before scheduled close of play on the final day.
* **Law 24 (Player Absence):** Penalty time tracking table to log when a player left the field, when they returned, and the time they become eligible to bowl or bat.

---

## Universal Umpiring Regulations Included on All Cards

### ECB Fast Bowling Directives (Youth Pace Bowlers)
Under ECB regulations (standard across UK leagues and recreational cricket), junior fast bowlers must strictly adhere to spell limits and daily maximums:

| Age Category | Maximum Overs per Spell | Maximum Overs per Day | Minimum Rest Period |
| :--- | :---: | :---: | :--- |
| **Under 19** | **7 overs** | **21 overs** | Equal overs from that end |
| **Under 17** | **6 overs** | **18 overs** | Equal overs from that end |
| **Under 15** | **5 overs** | **16 overs** | Equal overs from that end |
| **Under 13** | **4 overs** | **8 overs** | Equal overs from that end |

*Note on Rest:* A bowler who reaches their spell cap cannot bowl again until the same number of overs have been bowled from that same end (or an equivalent amount of time has elapsed).

### MCC Law 41 (Unfair Play) & Law 42 (Player Conduct)
Every card provides tick boxes and log space for:
* **Running on the pitch:** 1st warning, 2nd & final warning, 5 penalty runs.
* **Dangerous bowling (Beamers / High Full Pitches):** 1st warning, 2nd warning, suspension from bowling for remainder of innings.
* **Player Conduct (Law 42):** Level 1 (warning + repeat penalty), Level 2 (5 penalty runs), Level 3 (temporary suspension / sin bin), Level 4 (removal from match).

---

## Printing & Practical Field Advice

1. **Cardstock:** Print on **160gsm to 220gsm cardstock** (matte white or light cream). This prevents pencil and ballpoint ink from bleeding through to the other side when pressing down on the field.
2. **Duplex Setting:** In your printer dialog, select:
   * **Page Size:** A4
   * **Scale:** 100% (or "Fit to Printable Area")
   * **Two-Sided Printing:** **Flip on Long Edge** (Portrait)
3. **Folding & Storage:**
   * **Option A (Full A4):** Keep on a lightweight plastic umpire clipboard.
   * **Option B (A5 Folded):** Fold cleanly down the middle; each card becomes a compact A5 booklet that fits directly into standard umpire pocket wallets.
   * **Option C (PVC Sleeves):** Keep inside a clear A5/A4 waterproof scorecard wallet during damp English weather.
