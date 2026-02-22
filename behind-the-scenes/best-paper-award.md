# Behind the Scenes: Winning the Best Paper Award at ICIVC-2021

> **TDA Feature Extraction for Image Classification**
> International Conference on Intelligent Vision and Computing (ICIVC-2021)
> Prof. Milan Amrut Joshi

---

## Why I Am Writing This

Most academics will tell you about their published papers. Few will tell you about the messy, uncertain, sometimes frustrating process that led to them. I am writing this because I wish someone had shown me, early in my career, that award-winning papers do not emerge fully formed. They are forged through persistence, pivots, and more failed experiments than anyone admits.

If you are a PhD student reading this and wondering whether your research will ever amount to anything --- this story is for you.

---

## The Origin: A Question Nobody Was Asking

The idea that eventually became the ICIVC-2021 Best Paper started not with a flash of inspiration, but with a nagging question: **Why are we throwing away the topological structure of data before feeding it into classifiers?**

At the time, the computer vision community was largely focused on deeper architectures, better augmentation strategies, and larger datasets. Topological Data Analysis (TDA) existed as a beautiful mathematical framework, but it was confined mostly to theoretical mathematics and a few niche applications in materials science and neuroscience. Very few people were seriously applying TDA to mainstream computer vision tasks.

I had been reading about persistent homology --- a way to capture the "shape" of data at multiple scales --- and kept thinking: images have rich topological structure. Connected components, loops, voids --- these are meaningful features that convolutional filters might not explicitly capture. What if we extracted these features and used them alongside (or instead of) traditional features?

It was a cross-pollination idea: take a tool from algebraic topology and apply it to a problem in computer vision. The kind of idea that could be brilliantly innovative or completely useless. I had no way of knowing which one until I tried.

---

## The Early Experiments: Nothing Worked (At First)

The first three months were humbling. I implemented a basic pipeline:

1. Take an image
2. Convert it to a point cloud or filtration
3. Compute persistent homology
4. Extract persistence diagrams
5. Vectorize the diagrams (persistence landscapes, Betti curves, etc.)
6. Feed the vectors into a standard classifier

**The initial results were terrible.** The TDA features alone performed worse than a simple CNN baseline. It was not even close. I remember staring at accuracy numbers in the low 70s on CIFAR-10, while basic ResNet was hitting 93+.

I had two options: give up on the idea, or dig deeper to understand WHY it was not working.

I chose to dig.

---

## The Breakthrough: It Was a Representation Problem

After weeks of analysis, I realized the issue was not that topological features were uninformative --- it was that the standard vectorization methods were losing critical information. Persistence diagrams are rich mathematical objects, but flattening them into fixed-size vectors threw away the geometric relationships between features.

The breakthrough came when I developed a new feature extraction approach that preserved more of the topological structure during vectorization. Instead of treating persistence diagrams as simple summary statistics, I designed a method that captured:

- The **distribution** of topological features across scales
- The **interactions** between different homological dimensions
- The **spatial relationships** that standard persistence landscapes averaged out

The moment I saw the accuracy numbers jump by double digits on my test set, I knew I was onto something. It was a late evening, and I remember rechecking the numbers three times because I did not believe them.

---

## The Writing: Harder Than the Research

Getting the results was the easy part (relatively speaking). Explaining WHY the method worked to an audience that likely had never heard of persistent homology --- that was the real challenge.

I rewrote the introduction five times. Each version tried a different angle:
- Version 1: Started with TDA theory. Too dry. Lost the reader in two paragraphs.
- Version 2: Started with the limitations of CNNs. Too aggressive. Sounded like I was attacking the whole field.
- Version 3: Started with a motivating example. Better, but still too technical too fast.
- Version 4: Started with the observation that images have shape, and shape has mathematical meaning. This one clicked.
- Version 5: Refined version 4 with clearer figures and a gentler introduction to topology.

The figures were equally challenging. How do you explain persistence diagrams to someone who has never seen one? I spent an entire week on a single figure that showed the progression from image to point cloud to persistence diagram to classification, making sure each step was visually intuitive.

---

## Choosing the Venue

Here is an honest admission: ICIVC was not my first choice of venue.

I initially targeted a more prestigious conference. The paper was desk-rejected because the reviewers felt the intersection of TDA and image classification was "too niche" for their program. That rejection stung, and I spent a few days questioning whether the work was publishable at all.

My decision to submit to ICIVC came from a careful reading of their call for papers. They explicitly mentioned "novel feature extraction methods" and "mathematical approaches to computer vision" as topics of interest. The scope was a perfect match. Sometimes the right venue is not the most famous one --- it is the one where your audience actually lives.

---

## The Review Process

The reviews for ICIVC came back positive but demanding. Two of the three reviewers were genuinely engaged with the work:

**What they liked:**
- The novelty of the approach (applying TDA to image classification was new to them)
- The thoroughness of the experimental evaluation
- The clarity of the figures explaining topological concepts

**What they pushed back on:**
- They wanted more comparison with traditional feature extraction methods
- One reviewer asked for a computational complexity analysis
- They wanted to see results on more diverse datasets

I had three weeks to revise. I added two more baseline comparisons, wrote up the complexity analysis (which was actually favorable for our method), and added results on a medical imaging dataset that happened to work well with topological features.

---

## The Conference and the Award

The conference was held in 2021, during a period when many academic events were still navigating between virtual and in-person formats. I presented the work and answered questions from an engaged audience.

The Best Paper Award announcement came as a genuine surprise. I did not attend the conference expecting to win anything. When my name was called, my first thought was: "Wait, they must mean someone else." My second thought was: "All those months of failed experiments were worth it."

---

## What I Learned

### 1. Cross-disciplinary ideas are high-risk, high-reward

Applying methods from one field to another can fail spectacularly or succeed brilliantly. The key is having enough depth in both fields to know whether the combination is principled, not just novel.

### 2. Failed experiments are data

My three months of initial failures taught me more about TDA feature extraction than any textbook. Each failure narrowed the search space and eventually pointed me toward the right approach. I would not have found the breakthrough without the failures that preceded it.

### 3. Writing is not a chore --- it is part of the research

Rewriting the introduction five times was not wasted effort. Each version forced me to think more clearly about what the contribution actually was. By the time I finished writing, I understood my own work better than when I finished the experiments.

### 4. Venue fit matters more than venue prestige

The paper that won Best Paper at ICIVC might have been a borderline accept (or reject) at a more prestigious venue. Not because the work was weak, but because the audience matters. At ICIVC, the reviewers and attendees were looking for exactly this kind of work. At a large general ML conference, it might have been lost in the noise.

### 5. Rejection is redirection

The desk rejection from my first-choice venue forced me to find a venue that was actually a better fit. If that first venue had accepted the paper, it might have been published with less visibility and impact than it ultimately received. The rejection, painful as it was, led to a better outcome.

### 6. Persistence (no pun intended) is the most important research skill

The ability to keep working through months of negative results, through rejections, through the uncertainty of not knowing whether an idea will pan out --- that is what separates researchers who publish from those who do not. Talent helps. Resources help. But persistence is the foundation.

---

## Timeline Summary

| Period | Activity |
|--------|----------|
| Month 1--2 | Literature review on TDA and computer vision. Identified the gap. |
| Month 3--5 | Initial implementation and experiments. Poor results. |
| Month 5--6 | Deep analysis of failures. Identified the representation bottleneck. |
| Month 6--7 | Developed improved feature extraction method. Breakthrough results. |
| Month 7--8 | Comprehensive experiments and ablation studies. |
| Month 8--10 | Writing, rewriting, and revising the paper. Five rounds of the introduction. |
| Month 10 | Submitted to first venue. Desk rejected. |
| Month 10--11 | Minor revisions. Submitted to ICIVC-2021. |
| Month 12 | Reviews received. Revised and resubmitted within 3 weeks. |
| Month 13 | Accepted. Presented. Won Best Paper Award. |

Total: About 13 months from first reading about TDA to holding the award.

---

## Advice for PhD Students

1. **Do not wait for the perfect idea.** Start with a good question and let the research refine it. My "perfect" idea arrived in month 6, not month 1.

2. **Keep a research journal.** I wrote down what I tried, what failed, and why I thought it failed. This journal was invaluable when I needed to trace back my reasoning.

3. **Talk to people outside your sub-field.** My TDA knowledge came from attending a topology seminar that had nothing to do with my main research area. Cross-pollination requires exposure.

4. **Write early, write often.** Do not wait until all experiments are done. Writing clarifies thinking, and your future self will thank your past self for those messy first drafts.

5. **Celebrate the small wins.** The first experiment that beat a baseline by even 0.5%. The first figure that looked genuinely good. The first paragraph that read well. These moments sustain you through the hard parts.

6. **A Best Paper Award does not change who you are.** It is wonderful recognition, and I am proud of it. But the work was valuable before the award, and it would have been valuable without it. The award is a bonus. The contribution to knowledge is the real reward.

---

> *"The only difference between a published paper and an unpublished paper is that the authors of the published paper did not give up."*

---

*Prof. Milan Amrut Joshi*
*mlnjsh@gmail.com | GitHub: mlnjsh*
