# QA Interview — Complete Preparation Guide

> Based on real interview transcripts from your actual interviewer (Shashid, Manager — Search & Assistant). Every question, every mistake, every answer that worked — all in one place.

---

## How to use this guide

Read it once, top to bottom, to get the full picture. Then go back and focus on **Part 6** (the 7 quality tools) and **Part 4** (precision and recall) — those are the two places where every single candidate in that session failed, and where you have the biggest opportunity to stand out. **Part 3** (QA responsibilities) and **Part 7** (RCA and PCCP) are your next priority.

Shashid is not looking for a perfect candidate. He is looking for someone who clearly understands what QA work actually is, can communicate it without going in circles, and shows they took the interview seriously enough to prepare. You have now seen every question he asks, every mistake every candidate made, and the exact answers that worked. That is a significant advantage. Use it.

---

## Part 1 — Who is your interviewer and what does he want?

**The interviewer: Shashid (Sardar Mahal), Manager — Search & Assistant**

He runs batch interviews in one sitting. He is friendly at the start but moves fast. He has no patience for vague answers. He interrupts when you repeat yourself. He is not trying to fail you — but he will not ask the same question five times either.

### What he is testing

- Do you actually understand what a QA does every day?
- Can you explain technical concepts (precision, recall) in plain words?
- Did you prepare, or did you just show up?
- Can you give real examples from real work?

### His biggest signals

- He repeats the question in different words when the answer is wrong
- He asks "what did you prepare?" to catch lazy candidates
- He asks candidates to move to a private space — he wants full attention
- He ends every interview with "I wish you all the best" — neutral, gives nothing away

### His biggest fear as a hiring manager

Promoting someone who does not actually understand the QA role. He has seen many raters who think QA = just checking cases. Wrong. QA is about improving the whole team's quality — giving feedback, running RCA, conducting huddles, supporting OJT batches. He wants someone who gets that difference.

---

## Part 2 — Every question he asks (and why)

He asked the same 7–8 questions to every candidate. This is a structured scorecard, not a freeform conversation.

### Question 1 — Opener
**"Tell me about yourself. Which team? How long?"**

He is checking your base experience. Keep it under 60 seconds. End with: *"I specifically prepared for this QA role by reviewing..."*

### Question 2 — Most important
**"What are the roles and responsibilities of a QA?"**

The core question. Every candidate answered it vaguely and got pushed back. He wants a structured, numbered list — not a paragraph. See Part 3 for the exact answer.

### Question 3 — People skills
**"What is effective feedback? What is the sandwich method?"**

He wants to know if you can give feedback without making a reviewer feel bad. He also wants a real example — not just the theory. One candidate (Winky) gave an actual example from the floor and it impressed him. See Part 5 for the full answer.

### Question 4 — Technical must-know
**"What is precision and recall? What are the formulas? What is TP/TN/FP/FN?"**

Most candidates got the formula right but explained the concept wrong. He specifically asks "what is TP?" after the formula — he wants to know if you understand what it means in your actual work, not just the math. See Part 4 for the full breakdown.

### Question 5 — Differentiator (everyone failed this)
**"What quality tools do we use? Have you heard of Pareto chart / histogram / fishbone?"**

This is where every candidate blanked. Not a single person could name the 7 quality tools. If you know these, you immediately stand out. See Part 6 for the complete list.

### Question 6 — Policy knowledge
**"What is sensitive vs non-sensitive content?"**

He wants the platform-specific answer (ads, video, imagery) — not a general answer. He also asks how comfortable you are reviewing adult content. Say: *"It is part of the job."*

### Question 7 — Trap for unprepared people
**"What did you prepare for this interview?"**

Naveen said "I didn't prepare anything." Near-certain rejection. Answer with a confident list of at least 5–6 topics.

### Question 8 — Achievement
**"What is your biggest achievement in the last 2 years?"**

Must be specific. "I got positive feedback from a client during a shadow session" worked. "I got promoted" did not.

---

## Part 3 — QA roles and responsibilities (the full answer)

Give this as a numbered list. Never as a paragraph.

> **"A QA has five main areas of work. First — audits: Koala every Monday, safety net daily, stratified throughout the week, random audits for the OJT batch, and tool tests. Second — quality reports: weekly reports for Koala, safety net, and stratified samples. Third — daily communication: SOD (start of day) huddle with the team and a MOM (minutes of meeting) email dropped after every meeting. Fourth — feedback: one-on-one sessions with reviewers who made errors, using the sandwich method. Fifth — OJT batch support: random account audits each week and weekly quality reports for new joiners. A QA also handles client escalations through RCA and gives refresher sessions when there are policy updates."**

### The 5 types of audits

| Audit type | When | Priority |
|---|---|---|
| Koala | Every Monday | First priority — complete on Monday |
| Safety net | Monday to Friday | Clear on the same day they arrive |
| Stratified | Throughout the week | After Koala and safety net are done |
| Random audits | Weekly | For OJT batch — pick accounts randomly |
| Tool test | Periodic | Tool-based accuracy and consistency check |

### What a QA does every single day

1. SOD huddle — give updates, clear doubts
2. Drop MOM email after every huddle
3. Complete assigned audits for the day
4. Give one-on-one feedback to reviewers who made errors
5. Clarify policy doubts from reviewers throughout the day
6. Give refresher sessions when policy changes or errors are widespread
7. Monitor OJT batch — audit their work, prepare their quality reports
8. If a client escalation comes in — prepare RCA (see Part 7)

### Bonus — Meta QA (say this, no one else did)

When a QA cannot resolve a doubt independently, they escalate to Meta QA. Meta QA has cross-workflow and cross-vendor visibility. If Meta QA also cannot resolve it, they connect with the client directly or with other vendor QAs — then cascade the answer back down to all QAs, who inform their reviewers. It is the escalation chain above a regular QA.

---

## Part 4 — Precision, recall, accuracy (the full technical answer)

### Step 1 — Understand TP / TN / FP / FN in your workflow

In trust and safety work, accounts are either **bad** (should be suspended/actioned) or **ok** (should be released/approved).

| Term | Full name | Meaning in your workflow | Good or bad? |
|---|---|---|---|
| TP | True Positive | Bad account correctly marked bad — correct suspension | Good |
| TN | True Negative | Ok account correctly released — correct release | Good |
| FP | False Positive | Ok account wrongly suspended — over-flagging | Bad |
| FN | False Negative | Bad account wrongly released — under-flagging | Bad (more dangerous) |

### Step 2 — The formulas

**Precision** = TP ÷ (TP + FP)
> Of all the cases we suspended, how many were actually bad? Measures over-flagging.

**Recall** = TP ÷ (TP + FN)
> Of all the actual bad cases, how many did we catch? Measures under-flagging / misses.

**Accuracy** = (TP + TN) ÷ (TP + TN + FP + FN)
> Of all decisions made, how many were correct? Total correct decisions out of total decisions.

### Step 3 — What Shashid will ask after the formula

He will ask: *"What is TP?"* — do not just say "true positive." Say:

> *"TP in our workflow means a bad account that the reviewer correctly identified and actioned. For example, if a policy-violating ad was correctly suspended by the reviewer, that is a true positive."*

### Memory trick

- **Precision** = "are the suspensions right?" — catches over-flagging
- **Recall** = "did we catch all the bad ones?" — catches under-flagging
- High precision = fewer wrong suspensions
- High recall = fewer bad accounts slipping through

---

## Part 5 — Feedback and the sandwich method

### What is feedback?

Feedback is when a QA sits down with a reviewer who made an error and explains: what the error was, why it was an error, how to avoid it next time. The goal is improvement, not blame.

### The sandwich method — 3 layers

**Layer 1 — Positive:** Start by appreciating something real and genuine.
> *"Over the last 6 months, your production has been very consistent and your communication with the team is excellent."*

**Layer 2 — Constructive:** Explain the error clearly and specifically.
> *"I noticed a policy error in this case — you applied label X but according to our guideline, this account should have been released because of Y. Let me show you the policy section."*

**Layer 3 — Positive:** End on encouragement and confidence.
> *"I know this was a tricky case. Your overall accuracy is strong and I am confident this will not repeat once you go through the policy again."*

### A complete example to say in the interview

> *"One of my co-reviewers had been working for about 18 months and got a policy error flagged. I gave them feedback using the sandwich method. I started by saying — your production and quality over the past year have both been above average, and the team trusts your judgment. Then I said — I noticed this specific case where you suspended an account that was actually a borderline release under the policy. The misclick happened because the policy updated recently and I want to walk you through the new guideline. Then I ended by saying — you are one of the more reliable reviewers on our floor and I know once you review this policy, it will not happen again. After that I monitored their next 10 cases and there was no repeat error."*

---

## Part 6 — The 7 quality tools (the answer no one gave)

Every candidate blanked on this. If you know these, you will immediately separate yourself from the entire batch Shashid interviewed.

**Memory phrase:** *"Fish Check Control Histo-Para Scatter Strat"*
Say it 5 times out loud right now.

### 1. Fishbone diagram (Ishikawa / cause-and-effect)
A diagram shaped like a fish skeleton. The "head" is the problem. The "bones" are all the possible causes. Used to brainstorm every possible reason why a problem is happening. Example: why is the team's precision dropping? Bones might show — unclear policy, lack of refreshers, tool issues, uncalibrated new batch.

### 2. Check sheet
A simple structured form where you record data as it happens. Example: a sheet tracking how many errors each reviewer made this week, categorised by error type. The most basic data collection tool.

### 3. Control chart
A line graph that shows how a process changes over time. Has a central average line and upper/lower limits. If data goes outside the limits, something unusual is happening. Used to monitor if a reviewer's accuracy is going out of normal range.

### 4. Histogram
A bar chart showing how often something happens. Example: how many reviewers had 0–2 errors, 3–5 errors, 6+ errors this week. Shows the distribution of performance across the team.

### 5. Pareto chart
A special bar chart where bars go from most common to least common. Based on the 80/20 rule — 80% of problems are caused by 20% of causes. Used to find which error type is responsible for most of the quality drop, so you fix that first.

### 6. Scatter diagram
A graph with dots showing the relationship between two things. Example: does working speed (production) affect accuracy? If fast reviewers have more errors, the scatter diagram will show that pattern.

### 7. Stratification
Separating data by category to find hidden patterns. Example: instead of looking at all errors together, you separate them by floor, shift, workflow, or reviewer tenure. Helps identify if one specific group is causing the problem, not the whole team.

---

## Part 7 — RCA and 5Y analysis

### What is RCA?

RCA = Root Cause Analysis. Finding the real reason behind a mistake — not just the surface reason.

Example: a reviewer suspended an account wrongly. Surface reason = "they made an error." Real reason = "the policy changed last week and they were not informed." If you only address the surface, the error will happen again. RCA fixes the root.

### The 5Y method

Ask "Why?" five times in a row. Each answer goes deeper.

1. **Why was the account wrongly suspended?** — The reviewer applied the wrong policy label.
2. **Why did they apply the wrong label?** — They did not know about the updated policy guideline.
3. **Why did they not know about the update?** — The refresher session was not attended by this reviewer.
4. **Why did they miss the refresher?** — It was not marked mandatory and attendance was not tracked.
5. **Why was attendance not tracked?** — No formal MOM or sign-off process was in place for that refresher.

**Root cause:** No attendance tracking for refreshers.
**Fix:** Make all refreshers mandatory, take sign-off, drop MOM email. Error will not repeat for the whole team.

### What to do when a client escalation comes in

1. Receive the error flagged by client (via bug format or email)
2. Review the account yourself — confirm if it is actually an error
3. If it is an error — prepare RCA using the 5Y method
4. Determine: reviewer miss or non-reviewer miss (system issue, policy ambiguity)?
5. If reviewer miss — connect with the reviewer, give feedback using sandwich method
6. Closely monitor that reviewer for the next few weeks
7. If errors continue for 3–4 weeks — move reviewer to PCCP

### What is PCCP?

PCCP = Performance Counseling and Coaching Program. If a reviewer continues making errors even after feedback and monitoring, they are placed into PCCP for 4 weeks of structured monitoring. If errors still continue, the process escalates to termination as per HR policy. As a QA, your job is to do everything possible before it reaches that stage.

---

## Part 8 — Sensitive vs non-sensitive content

### Sensitive content — examples

- Adult and explicit content (18+)
- Online gambling and betting ads
- Weapons — guns, explosives, knives
- Drugs and controlled substances
- Dangerous products (DPS)
- Graphic imagery — realistic body parts in non-medical context
- Content promoting violence or self-harm
- Strongly restricted = most explicit; moderately restricted = borderline (libido products, supplements)

### Non-sensitive content — examples

- Standard retail and e-commerce ads
- Online booking (flights, hotels, entertainment)
- Food delivery and restaurant ads
- Educational content
- General entertainment
- Tech products and software

### How to answer the comfort question

Shashid asked every candidate: *"How comfortable are you watching adult videos and explicit content?"*

Answer: *"It is part of the job. I approach it as a professional task — it does not make me uncomfortable. I understand we are here to moderate and ensure policy compliance, not to judge the content personally."*

---

## Part 9 — Your achievement answer

### What does NOT work

- "I got promoted to ER team." — Says what happened to you, not what you achieved.
- "I maintained good quality." — Vague, no outcome.
- "I worked hard." — Not an achievement.

### Structure that works

**Situation** → **What you did** → **Result**

Strong examples:
- *"I was selected to give a shadow session during a client visit. The client gave positive feedback directly to my manager and said my explanations were clear and accurate."*
- *"For the last 6 months I have maintained a zero-error record — zero errors flagged by QA or by client."*
- *"I identified a recurring policy confusion in my team, raised it with my QA, and helped design a refresher session. After the session, that error type dropped significantly in our weekly report."*

---

## Part 10 — What to say when asked "What did you prepare?"

> *"I prepared the following areas specifically for this QA role. One — QA roles and responsibilities including the full audit cycle and daily tasks like SOD, MOM, and refresher sessions. Two — Precision, recall, and accuracy — the formulas and the meaning of TP, TN, FP, FN in our workflow. Three — Feedback methodology, including the sandwich method with a real example. Four — RCA and the 5Y analysis method for error root cause. Five — The 7 quality tools including fishbone, Pareto chart, control chart, histogram, scatter diagram, check sheet, and stratification. Six — Sensitive vs non-sensitive content policy in the context of ads and platform content."*

---

## Part 11 — What every candidate did wrong

| Candidate | What went wrong | What you must not repeat |
|---|---|---|
| Naveen | Said "I didn't prepare anything." Shashid asked "why are you not serious?" | Never admit zero preparation |
| Saiprasanna | Wrong formula, visibly nervous, said "I'll prepare better next time" at the end | Wrong formulas and self-defeating closing statements |
| Shruthika | Said "precision is to calculate the bad cases" — too vague | Give concept clearly, not just a word association |
| Barat | Said "RCA recall" when asked what RCA stands for — confused the terms | Know your acronyms cold |
| Winky (best) | Main gaps: quality tools, initial sensitive content answer | Even the best candidate had gaps — you can do better |

---

## Part 12 — Your question to ask at the end

> *"What does the first 30 days look like for a new QA joining the team? Is there a calibration period or do new QAs start auditing independently right away? I want to understand how to ramp up the right way."*

**Backup question:**
> *"What is the most common mistake you see new QAs make in their first few weeks — the thing that takes the longest to correct?"*

---

## Part 13 — Day before and day of checklist

### Day before — do these

- [ ] Memorise the 7 quality tools by name and one-line description. Say them out loud 5 times.
- [ ] Write TP, TN, FP, FN definitions in your own words using your workflow context.
- [ ] Write out precision, recall, accuracy formulas from memory. Explain each in one sentence without the formula.
- [ ] Practise your achievement answer: situation, what you did, result. Under 45 seconds.
- [ ] Practise the sandwich feedback method with a real or made-up example.
- [ ] Write out the full QA daily routine from memory.
- [ ] Sit with a QA for 20–30 minutes if possible. Tell Shashid you did this.

### Day of interview — moment by moment

- [ ] Camera on immediately when the call connects. Do not wait to be asked.
- [ ] Be in a quiet, private place before the call starts.
- [ ] "Tell me about yourself" — under 60 seconds, end with what you prepared.
- [ ] Roles and responsibilities — numbered list, all 5 areas.
- [ ] Precision — concept first, formula second, TP/FP in workflow terms third.
- [ ] Quality tools — list all 7 confidently. Volunteer before he asks.
- [ ] "What did you prepare?" — deliver your full list without hesitation.
- [ ] End with your prepared closing question.

---

*This guide is based on direct transcript analysis of your actual interviewer's session. Every insight is grounded in what actually happened — not general interview advice.*
