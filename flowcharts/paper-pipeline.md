# Paper Writing Pipeline: From Idea to Publication

> **This flowchart maps the entire journey of a research paper.** Each stage has concrete deliverables and decision points. Use this as a project management tool, not just a reference.

---

## The Complete Pipeline

```
                          PAPER WRITING PIPELINE
                     From Idea to Published Paper

    +------------------+
    |   RESEARCH IDEA  |
    | (Observation,    |
    |  Question, Gap)  |
    +--------+---------+
             |
             v
    +------------------+
    | LITERATURE REVIEW|----> Is the gap real? ----> NO ----> Pivot/Refine idea
    | (2-4 weeks)      |                                          |
    +--------+---------+                                          |
             | YES                                                |
             v                                          +---------+
    +------------------+
    | PROBLEM          |
    | FORMULATION      |
    | (1 week)         |
    | - Define scope   |
    | - Set objectives |
    | - Choose metrics |
    +--------+---------+
             |
             v
    +------------------+
    | METHODOLOGY      |----> Does it work? -----> NO ----> Debug / Redesign
    | DEVELOPMENT      |      (on toy data)                      |
    | (4-8 weeks)      |                                         |
    | - Design method  |                               +---------+
    | - Implement code |
    | - Initial tests  |
    +--------+---------+
             | YES
             v
    +------------------+
    | FULL EXPERIMENTS |----> Results good? -----> NO ----> Iterate method
    | (2-4 weeks)      |      (vs baselines)                     |
    | - Benchmark data |                                         |
    | - Run baselines  |                               +---------+
    | - Ablation study |
    | - Statistics     |
    +--------+---------+
             | YES
             v
    +------------------+
    | WRITING PHASE    |
    | (3-6 weeks)      |
    | - See detailed   |
    |   breakdown below|
    +--------+---------+
             |
             v
    +------------------+
    | INTERNAL REVIEW  |----> Major issues? -----> YES ----> Revise
    | (1-2 weeks)      |                                       |
    | - Advisor review |                                       |
    | - Peer feedback  |                             +---------+
    | - Self-review    |
    +--------+---------+
             | NO
             v
    +------------------+
    | JOURNAL/VENUE    |
    | SELECTION        |
    | (1 week)         |
    | - See journal    |
    |   selection guide|
    +--------+---------+
             |
             v
    +------------------+
    | PRE-SUBMISSION   |
    | CHECKLIST        |
    | (2-3 days)       |
    | - Format check   |
    | - Final proofread|
    | - Cover letter   |
    +--------+---------+
             |
             v
    +------------------+
    |    SUBMIT!       |
    +--------+---------+
             |
             v
    +------------------+
    | WAIT FOR REVIEWS |  Typical timelines:
    | (1-6 months)     |  - Conference: 1-3 months
    |                  |  - Journal: 2-6 months
    +--------+---------+
             |
             v
        +---------+
        | DECISION|
        +----+----+
             |
    +--------+--------+--------+
    |        |        |        |
    v        v        v        v
 ACCEPT   MINOR    MAJOR    REJECT
    |     REVISION REVISION    |
    |        |        |        |
    v        v        v        v
 Camera   Revise   Revise   Analyze
 Ready    (2-4     (1-3     reviews
 Prep     weeks)   months)     |
    |        |        |        v
    |        v        v     Revise &
    |     Resubmit Resubmit resubmit
    |        |        |    elsewhere
    |        v        v        |
    |     +--+--------+--+     |
    |     | SECOND ROUND |     |
    |     | DECISION     |     |
    |     +------+-------+     |
    |            |              |
    +-----+------+------+------+
          |
          v
    +------------------+
    |   CAMERA READY   |
    | (1-2 weeks)      |
    | - Final format   |
    | - Copyright form |
    | - De-anonymize   |
    +--------+---------+
             |
             v
    +------------------+
    |   PUBLISHED!     |
    +------------------+
             |
             v
    +------------------+
    | POST-PUBLICATION |
    | - arXiv upload   |
    | - Social media   |
    | - Update website |
    | - Presentation   |
    +------------------+
```

---

## Writing Phase Breakdown

The writing phase deserves its own detailed breakdown because it is where most people struggle with time management.

```
                    WRITING PHASE DETAIL
                    (3-6 weeks total)

    WEEK 1: SKELETON
    +--------------------------------------------------+
    | Day 1-2: Create outline with section headings     |
    | Day 3:   Draft all figures and tables             |
    | Day 4-5: Write figure captions and table headers  |
    | Day 6-7: Write the Experiments section            |
    +--------------------------------------------------+
                            |
                            v
    WEEK 2: CORE CONTENT
    +--------------------------------------------------+
    | Day 1-3: Write the Methodology section            |
    | Day 4-5: Write the Results & Discussion section   |
    | Day 6-7: Write the Related Work section           |
    +--------------------------------------------------+
                            |
                            v
    WEEK 3: BOOKENDS
    +--------------------------------------------------+
    | Day 1-2: Write the Introduction                   |
    | Day 3:   Write the Conclusion                     |
    | Day 4:   Write the Abstract                       |
    | Day 5-7: First complete self-review and revision  |
    +--------------------------------------------------+
                            |
                            v
    WEEK 4: POLISH
    +--------------------------------------------------+
    | Day 1-2: Address self-review comments             |
    | Day 3-4: Send to advisor / co-authors for review  |
    | Day 5-7: Buffer for advisor feedback turnaround   |
    +--------------------------------------------------+
                            |
                            v
    WEEK 5-6: FINALIZE
    +--------------------------------------------------+
    | Incorporate feedback from advisor / co-authors     |
    | Final formatting and proofreading                  |
    | Prepare supplementary material                     |
    | Prepare cover letter (if journal)                  |
    +--------------------------------------------------+
```

> **Key insight:** Write the sections in this order: Experiments -> Methodology -> Results -> Related Work -> Introduction -> Conclusion -> Abstract. The Introduction and Abstract are hardest to write well, and they depend on everything else being finalized.

---

## Revision Phase Breakdown

```
                    REVISION WORKFLOW
              (After receiving reviews)

    +------------------+
    | Receive Reviews  |
    +--------+---------+
             |
             | Wait 48 hours (cool down)
             v
    +------------------+
    | Read Reviews     |
    | Carefully        |
    +--------+---------+
             |
             v
    +------------------+
    | Classify Each    |
    | Comment:         |
    | - Valid (fix)    |
    | - Misunderstand  |
    |   (clarify)     |
    | - Disagree       |
    |   (explain)     |
    +--------+---------+
             |
             v
    +------------------+
    | Create Revision  |
    | Plan with        |
    | Timeline         |
    +--------+---------+
             |
             v
    +------------------+
    | Discuss Plan     |
    | with Advisor     |
    +--------+---------+
             |
             v
    +------------------+       +------------------+
    | Revise Paper     |<----->| Write Response   |
    | (parallel)       |       | to Reviewers     |
    +--------+---------+       | (parallel)       |
             |                 +--------+---------+
             v                          |
    +------------------+                |
    | Internal Review  |<---------------+
    | of Revised       |
    | Version          |
    +--------+---------+
             |
             v
    +------------------+
    | Submit Revised   |
    | Manuscript +     |
    | Response Letter  |
    +------------------+
```

---

## Time Estimates by Stage

| Stage | Typical Duration | Can Be Parallelized? |
|-------|-----------------|---------------------|
| Literature review | 2--4 weeks | Partially (with problem formulation) |
| Problem formulation | 1 week | Partially (with lit review) |
| Methodology development | 4--8 weeks | No (sequential) |
| Experiments | 2--4 weeks | Partially (run experiments while starting to write) |
| Writing | 3--6 weeks | Partially (sections can be written in parallel by co-authors) |
| Internal review | 1--2 weeks | No (need complete draft) |
| Pre-submission prep | 2--3 days | No (final step) |
| Waiting for reviews | 1--6 months | Yes (work on other projects!) |
| Revision | 2--12 weeks | No (depends on review feedback) |

**Total: 4--10 months** from idea to first submission, depending on project complexity.

---

## Tips for Staying on Track

1. **Set weekly milestones**, not just a final deadline
2. **Write every day**, even if it is just 200 words. Consistency beats bursts.
3. **Do not wait for perfect results** to start writing. Write the methodology and related work while experiments are running.
4. **Use version control** (Git) for your LaTeX source. You will thank yourself later.
5. **Share drafts early and often.** A bad first draft shared with your advisor is more useful than a good draft you share the night before the deadline.

---

> **The most dangerous moment** in the pipeline is after experiments are done but before writing starts. This is where papers die. The excitement of getting results fades, and the drudgery of writing looms. Push through it. Set a writing start date before you finish experiments, and stick to it.
