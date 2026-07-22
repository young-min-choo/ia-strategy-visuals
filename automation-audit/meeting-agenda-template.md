# Department Head Meeting Agenda — Process & Automation Discovery

**Meeting length:** 45-60 minutes  
**Participants:** You (engineering team lead) + department head  
**Pre-meeting:** You should have already collected intake questionnaires from 1-2 ICs on this team. Bring notes.

---

## 0. Framing (3 min)

> "I'm conducting an audit across all departments to understand recurring processes and identify where automation could save your team time and reduce errors. This isn't about cutting headcount — it's about removing the repetitive work that gets in the way of the work you'd rather be doing. Everything we discuss stays between us unless you want it shared."

**Ask up front:** "Is there anything off-limits or sensitive I should be aware of before we start?"

---

## 1. Department Overview (5 min)

- "Walk me through your team's core responsibilities."
- "How many people are on the team, and what are their roles?"
- "What does a typical week look like for your department?"

**Goal:** Get the lay of the land. Listen for mentions of systems, tools, and recurring activities — note them.

---

## 2. Process Mapping (15-20 min)

Work through the team's recurring processes. For each one the head mentions (or that came up in the IC questionnaires), capture:

| Dimension | Ask |
|---|---|
| **What** | "Describe the process step by step." |
| **Who** | "Who on your team does this? How many people total?" |
| **Frequency** | "How often does this happen? Daily? Weekly? Triggered by what?" |
| **Duration** | "Roughly how long does each occurrence take?" |
| **Tools** | "What systems, tools, or spreadsheets are involved?" |
| **Error rate** | "How often does this need to be redone or corrected?" |
| **Dependencies** | "Does this depend on input from another person or department?" |
| **Existing automation** | "Is any part of this already automated or semi-automated?" |

**Pro tip:** If the head's description doesn't match what the ICs reported in the questionnaire, gently probe. The gap between "official process" and "what actually happens" is often the most valuable finding.

> "I noticed [X] mentioned they do [Y step] that takes about [Z] — is that something you're aware of?"

---

## 3. Pain Points (10 min)

Ask directly — these surface the highest-value automation targets:

- **"What's the task your team dreads the most?"**
- **"Where do you see the most errors or rework?"**
- **"What takes longer than it should?"**
- **"Have you tried to automate anything before? What happened?"** (Listen for: failed because no engineering support, tool limitations, or political resistance)
- **"If engineering could make one thing disappear from your team's workload, what would it be?"**

---

## 4. Cross-Departmental Handoffs (5-10 min)

- **"Which departments do you hand work off to, or receive work from?"**
- **"Which handoffs are the slowest or most painful?"**
- **"Is there information you need from another department that's hard to get?"**
- **"Are there approval processes that bottleneck your team?"**

**Goal:** Map the cross-department edges. When you've met with all heads, compare notes — a handoff mentioned by both sides is a high-confidence automation target.

---

## 5. Seasonal / Temporal Spikes (5 min)

- **"Does your workload spike at certain times?"**
- **"What changes during those periods?"**
- **"Do you have enough capacity during spikes, or is it a crunch?"**

**Why:** Spikes often involve the most manual, least optimized work — high automation value.

---

## 6. Data & Reporting (5 min)

- **"What reports does your team produce, and for whom?"**
- **"How are those reports assembled — manual, exported, automated?"**
- **"Is there data you wish you had access to but can't easily get?"**

**Why:** Reporting is frequently the easiest, highest-ROI automation target. Someone spending 3 hours every Monday assembling a spreadsheet from 4 systems = immediate win.

---

## 7. Wrap-Up (3-5 min)

- **"Is there anything I should have asked but didn't?"**
- **"Who else on your team should I talk to if I want to dig deeper into any of these?"**
- **"How would you feel about us piloting an automation on one of these processes?"** (Gauges openness to change)

---

## Post-Meeting: Your Notes Template

Fill this out immediately after the meeting, while it's fresh.

```
Department:
Date:
Head interviewed:
ICs surveyed beforehand:

## Processes Identified
| # | Process | Frequency | Duration | # People | Error Rate | Tools | Automated? | Notes |
|---|---------|-----------|----------|----------|------------|-------|------------|-------|
| 1 |         |           |          |          |            |       |            |       |
| 2 |         |           |          |          |            |       |            |       |

## Estimated Hours/Month per Process
| # | Process | (Frequency × Duration × People) = Hours/mo | Feasibility (1-5) | Impact (1-5) | Priority Score |
|---|---------|-------------------------------------------|-------------------|--------------|----------------|
| 1 |         |                                           |                   |              |                |
| 2 |         |                                           |                   |              |                |

## Cross-Department Handoffs Noted
- → [Department]: [Description]
- ← [Department]: [Description]

## Key Quotes / Insights
- 

## Follow-Up Actions
- [ ] Talk to [person] about [process]
- [ ] Check feasibility of automating [process]
- [ ] Cross-reference with [other department]'s notes
```

---

## Scoring Guide (for your priority list, after all meetings)

**Feasibility (1-5):**
1 = Requires human judgment, unstructured data, or manual systems with no API
2 = Partially feasible, some manual steps would remain
3 = Feasible with moderate engineering effort
4 = Feasible with low effort, clean data
5 = Trivial — could be a script in an afternoon

**Impact (1-5):**
1 = <2 hours/month saved
2 = 2-8 hours/month saved
3 = 8-20 hours/month saved
4 = 20-50 hours/month saved
5 = 50+ hours/month saved, or eliminates a critical error source

**Priority = Impact × Feasibility**
- 20-25: Do first
- 12-19: Plan for next quarter
- 5-11: Backlog
- <5: Probably not worth it