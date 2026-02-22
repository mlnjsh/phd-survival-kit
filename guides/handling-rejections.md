# How to Handle Paper Rejections

> **Every successful researcher has a pile of rejection letters.** If you have never been rejected, you are not aiming high enough. This guide covers the practical and emotional sides of dealing with rejection, and how to turn a rejection into a stronger resubmission.

---

## The Reality of Rejection

Let this sink in:

- **Top ML conferences** (NeurIPS, ICML, ICLR) reject 70--80% of submissions
- **Top CV conferences** (CVPR, ECCV, ICCV) reject 73--80% of submissions
- **Top journals** (IEEE TPAMI, IJCV) reject 80--90% of submissions
- Many papers that are eventually published at top venues were **rejected at least once** before acceptance

Rejection is the default outcome. Acceptance is the exception. Knowing this does not make it hurt less, but it does put things in perspective.

---

## Types of Rejection

Understanding what type of rejection you received helps determine your next steps.

### Desk Rejection (Without Review)

**What it means:** The editor decided the paper is not suitable without sending it to reviewers.

**Common reasons:**
- Paper is outside the journal's scope
- Paper does not meet minimum quality standards
- Formatting is completely wrong
- Paper is too similar to a previously published work

**What to do:**
- Read the editor's reason carefully
- If it is a scope issue, resubmit to a more appropriate venue immediately (no revision needed)
- If it is a quality issue, significant revision is needed before resubmitting anywhere

### Rejection After Review

**What it means:** Reviewers read your paper and the editor decided it does not meet the bar.

**Types of reviewer recommendations:**
- **Reject (strong):** Fundamental flaws in methodology or contribution
- **Reject (weak):** Significant issues but potentially fixable
- **Major revision (but editor decides reject):** The editor weighed the reviews and decided against the paper

### Conference Rejection

**What it means:** Your paper scored below the acceptance threshold. Conference rejections are usually final for that venue (no revision opportunity).

---

## The Emotional Side

### What You Will Feel (And Why It Is Normal)

1. **Anger:** "The reviewers are incompetent! They did not even understand my paper!"
2. **Despair:** "I am not good enough. Maybe I should quit research."
3. **Denial:** "The review process is broken. My paper is clearly good."
4. **Embarrassment:** "What will my advisor/colleagues think?"

All of these feelings are completely normal. Every researcher experiences them. Here is how to handle them:

### The 48-Hour Rule

**Do not read the reviews carefully on the day you receive them.** Skim them once to understand the decision, then close the email. Wait at least 48 hours before reading them in detail and planning your response. Your emotional brain needs time to cool down before your analytical brain can do useful work.

### Reframing Strategies

| Unhelpful Thought | Reframe |
|-------------------|---------|
| "I am a failure" | "My paper was rejected, not me. This is one paper, one submission, one set of reviewers." |
| "The reviewers are idiots" | "If three independent reviewers misunderstood something, maybe my writing was not clear enough." |
| "I wasted months of work" | "The work is done and the results are real. I just need to present them better or find the right venue." |
| "Everyone else gets accepted easily" | "You are seeing their successes, not their rejections. Ask any senior researcher about their rejection history." |
| "My advisor will be disappointed" | "Your advisor has been rejected many times. They understand. Talk to them." |

### Talk to Someone

- Your advisor (they have been through this many times)
- Your lab mates (they are going through it too)
- A mentor outside your immediate group (fresh perspective helps)
- A friend or family member (they cannot fix the paper but they can listen)

Do not isolate yourself. Rejection feels worse when you carry it alone.

---

## The Practical Side: Analyzing Reviews

### Step 1: Classify Each Comment

After the 48-hour cooling period, go through each reviewer comment and classify it:

| Category | Description | Action Required |
|----------|-------------|-----------------|
| **Valid and easy** | Reviewer found a genuine issue that is straightforward to fix | Fix it |
| **Valid and hard** | Reviewer found a genuine issue that requires significant work | Plan the work, estimate effort |
| **Misunderstanding** | Reviewer misunderstood your paper | Rewrite the relevant section for clarity |
| **Scope disagreement** | Reviewer thinks the topic is not important or relevant | Consider if you are targeting the wrong venue |
| **Impossible/unreasonable** | Reviewer asks for something infeasible | Address as best you can; explain constraints |
| **Contradictory** | Two reviewers give opposite feedback | Use your judgment; follow the stronger argument |

### Step 2: Identify Patterns

If multiple reviewers flag the same issue, it is almost certainly a real problem. Pay special attention to:

- Issues raised by **2 or more reviewers** (consensus problems)
- Comments from the **most knowledgeable reviewer** (they understand the field best)
- The **meta-reviewer's summary** (this is usually the most balanced assessment)

### Step 3: Create a Revision Plan

Build a concrete plan with priorities:

```
CRITICAL (must fix before resubmitting anywhere):
1. Add ablation study (Reviewer 1, Reviewer 3)
2. Fix the theoretical proof in Section 4 (Reviewer 2)
3. Add experiments on 2 more datasets (All reviewers)

IMPORTANT (significantly improves the paper):
4. Rewrite introduction for clarity (Reviewer 1)
5. Add comparison with Method X (Reviewer 3)
6. Improve figure quality (Reviewer 2)

MINOR (nice to have):
7. Fix typos and grammar
8. Add more references from 2024
```

---

## Decision Tree: What to Do Next

### Option A: Revise and Resubmit to the Same Venue

**When to do this:**
- The journal explicitly invites resubmission (some say "reject and resubmit")
- The reviews are constructive and you can address all major concerns
- The journal is the right fit for your paper

**How to do it:**
- Address ALL reviewer comments thoroughly
- Write a detailed response letter (use the Response to Reviewers template)
- Highlight all changes in the revised manuscript
- Resubmit within 3--6 months (too long and the field may have moved on)

### Option B: Revise and Submit to a Different Venue

**When to do this:**
- The rejection was based on scope mismatch
- The reviews suggest the paper needs a different audience
- You want faster turnaround at a different tier of venue

**How to do it:**
- Still address the reviewers' valid points (even though you are going elsewhere)
- Reformat for the new venue's requirements
- Consider whether the paper should be shortened (journal to conference) or expanded (conference to journal)

### Option C: Major Overhaul

**When to do this:**
- Reviews identify fundamental methodological flaws
- The contribution is not strong enough for your target venues
- You realize the paper needs substantially more work

**How to do it:**
- Treat it as a new project, not a revision
- Redesign experiments, strengthen theory, or change the approach
- This may take 3--6 months of additional work
- The result will be a much stronger paper

### Option D: Shelve the Paper

**When to do this (rare but sometimes correct):**
- The idea is fundamentally flawed and cannot be salvaged
- The field has moved on and the contribution is no longer relevant
- Your time is better spent on a different project

**How to do it:**
- Discuss with your advisor before making this decision
- Extract what you learned and apply it to future work
- You can always revisit the idea later with fresh perspective

---

## Turning Rejection into Strength

### Use Reviewer Comments as Free Consulting

Reviewers are experts who spent hours reading your paper and providing feedback. That is free expert consulting. Even harsh reviews contain useful information.

### Track Your Rejection History

Keep a record:

```
Paper: "TDA-based Feature Extraction for Image Classification"
- Submission 1: CVPR 2021 (Rejected, scores 3/5/4)
  Key feedback: insufficient experiments, unclear motivation
- Submission 2: ECCV 2022 (Rejected, scores 5/6/4)
  Key feedback: good work but incremental contribution
- Submission 3: ICIVC 2021 (Accepted, Best Paper Award)
  Key learning: right venue, improved paper, matched audience
```

Tracking this helps you see progress and patterns. A paper that scores 3/5/4 on the first try and 5/6/4 on the second is improving, even though both were rejections.

### Build Resilience Over Time

With experience, rejection becomes less painful:
- **First rejection:** Devastating (feels like a personal failure)
- **Fifth rejection:** Frustrating (but you know the drill)
- **Twentieth rejection:** Routine (just another data point)
- **Fiftieth rejection:** Expected (you are aiming high and that is good)

---

## What NOT to Do

1. **Do not argue with reviewers via email.** If you disagree, address it in the revision, not in angry correspondence.
2. **Do not resubmit without changes.** Even if you think the reviewers were wrong, improve the paper.
3. **Do not badmouth reviewers publicly.** The research community is small. Word gets around.
4. **Do not give up on the paper after one rejection.** Most published papers were rejected at least once.
5. **Do not submit to a predatory journal out of desperation.** A predatory publication is worse than no publication.
6. **Do not compare yourself to others.** You are seeing their highlights, not their rejection folders.

---

## Perspective from Experience

Some of the most influential papers in the history of computer science were initially rejected:

- Papers that go on to win test-of-time awards were often rejected on their first submission
- Senior researchers with hundreds of publications still get rejected regularly
- Getting rejected from a top venue and then winning a Best Paper Award at another venue is more common than you think

The rejection is not the end of the story. It is a plot twist.

---

> **The single most important thing you can do after a rejection:** Talk to your advisor within a week, make a plan within two weeks, and start revising within a month. Papers that sit untouched after rejection for more than 3 months rarely get resubmitted. Momentum matters.

> **Remember:** The paper that eventually wins an award is often the same paper that was rejected elsewhere first. The difference is not the paper --- it is the perseverance of the authors.
