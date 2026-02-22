# Systematic Literature Review Strategy

> **A literature review is not a reading list --- it is a structured analysis of what the field knows, does not know, and where it is heading.** This guide provides a repeatable methodology for conducting thorough literature reviews, whether for a paper's Related Work section, a thesis chapter, or a standalone survey.

---

## Phase 1: Define the Scope

Before reading a single paper, define what you are looking for.

### 1.1 Formulate Research Questions

Write 3--5 specific questions your review should answer:

- **RQ1:** What methods have been proposed for [specific task]?
- **RQ2:** What datasets and evaluation metrics are commonly used?
- **RQ3:** What are the reported performance levels, and how do they compare?
- **RQ4:** What assumptions and limitations are common across methods?
- **RQ5:** What open challenges remain?

### 1.2 Define Inclusion/Exclusion Criteria

Be explicit about what papers you will and will not include:

| Criterion | Include | Exclude |
|-----------|---------|---------|
| **Date range** | 2018--present | Before 2018 (unless seminal) |
| **Venue quality** | Peer-reviewed journals and top conferences | Non-peer-reviewed blog posts, white papers |
| **Language** | English | Non-English |
| **Relevance** | Directly addresses [your task/method] | Tangentially related |
| **Study type** | Empirical studies, theoretical analyses | Editorials, opinion pieces |

### 1.3 Choose Your Databases

Use multiple databases to avoid coverage gaps:

| Database | Strengths | URL |
|----------|-----------|-----|
| **Google Scholar** | Broadest coverage, citation tracking | scholar.google.com |
| **Semantic Scholar** | AI-powered relevance, citation graphs | semanticscholar.org |
| **IEEE Xplore** | Authoritative for EE/CS | ieeexplore.ieee.org |
| **ACM Digital Library** | Computing-focused | dl.acm.org |
| **arXiv** | Preprints, cutting-edge work | arxiv.org |
| **DBLP** | Computer science bibliography | dblp.org |
| **PubMed** | Biomedical/health sciences | pubmed.ncbi.nlm.nih.gov |
| **Web of Science** | Citation indexing, impact metrics | webofscience.com |
| **Scopus** | Broad scientific coverage | scopus.com |

---

## Phase 2: Search and Collect

### 2.1 Develop Search Queries

Build queries systematically using Boolean operators:

```
Primary query:
("topological data analysis" OR "persistent homology" OR "TDA")
AND ("feature extraction" OR "feature representation")
AND ("image classification" OR "computer vision")

Narrower query:
("persistence diagram" OR "persistence landscape")
AND ("convolutional neural network" OR "deep learning")

Broader query:
("topological" OR "homological")
AND ("machine learning" OR "pattern recognition")
```

> **Tip:** Run your queries on multiple databases. Google Scholar finds things that IEEE Xplore misses, and vice versa.

### 2.2 Snowball Sampling

After finding an initial set of papers, expand your search:

**Forward snowballing:** For each key paper, check "Cited by" on Google Scholar. Papers that cite your key papers are likely relevant.

**Backward snowballing:** Check the reference list of each key paper. The papers they cite may be important predecessors you missed.

**Author tracking:** Identify the key researchers in the area and check their recent publication lists.

### 2.3 Set a Stopping Criterion

You cannot read everything. Stop searching when:

- New searches return papers you have already seen (saturation)
- You have covered the major venues for the last 3--5 years
- Your advisor confirms the coverage is sufficient
- You have 50--150 papers for a thesis chapter, 20--40 for a paper's Related Work

---

## Phase 3: Screen and Filter

### 3.1 Three-Pass Screening

**Pass 1 --- Title and Abstract (30 seconds per paper):**
- Read the title, abstract, and keywords
- Decision: Include, Exclude, or Maybe
- Aim to reduce your list by 50--60%

**Pass 2 --- Skim (5--10 minutes per paper):**
- Read the introduction, section headings, figures/tables, and conclusion
- Check the methodology at a high level
- Decision: Include or Exclude
- Aim to reduce by another 30--40%

**Pass 3 --- Full Read (30--60 minutes per paper):**
- Read the remaining papers in full
- Take structured notes (see Phase 4)
- This is your final set of papers for the review

### 3.2 Track Your Decisions

Keep a spreadsheet or database with:

| Column | Purpose |
|--------|---------|
| Paper ID | Unique identifier (BibTeX key) |
| Title | Full title |
| Authors | First author et al. |
| Year | Publication year |
| Venue | Journal/conference name |
| Screening decision | Include / Exclude / Maybe |
| Exclusion reason | Why it was excluded (if applicable) |
| Relevance score | 1--5 (how central to your review) |
| Notes | Key findings, methods, limitations |

---

## Phase 4: Read and Extract

### 4.1 Structured Note-Taking Template

For each included paper, extract the following:

```
## [BibTeX Key] - Short Title

**Full citation:** Authors, Title, Venue, Year
**Problem addressed:**
**Key method/contribution:**
**Datasets used:**
**Evaluation metrics:**
**Main results (quantitative):**
**Strengths:**
**Limitations (stated by authors):**
**Limitations (observed by me):**
**Relevance to my work:**
**Key quotes (with page numbers):**
**Questions/follow-ups:**
```

### 4.2 Build a Comparison Matrix

As you read, build a comparison table:

| Paper | Year | Method Type | Dataset(s) | Metric | Best Result | Code Available |
|-------|------|-------------|------------|--------|-------------|----------------|
| Author A | 2022 | CNN-based | CIFAR-10 | Accuracy | 95.2% | Yes |
| Author B | 2023 | GNN-based | CIFAR-10 | Accuracy | 96.1% | No |
| Author C | 2023 | TDA+ML | CIFAR-10 | Accuracy | 93.8% | Yes |

This matrix becomes invaluable when writing the Related Work section and positioning your contribution.

### 4.3 Identify Themes and Clusters

Group papers by approach, not by chronology:

- **Cluster 1:** Methods based on approach X
- **Cluster 2:** Methods based on approach Y
- **Cluster 3:** Hybrid approaches
- **Cluster 4:** Theoretical analyses

Each cluster will typically become a subsection in your literature review.

---

## Phase 5: Synthesize and Write

### 5.1 Writing Structure Options

**Thematic (recommended):** Organize by topic/approach. Best for most reviews.

```
2. Related Work
   2.1 Deep Learning Approaches
   2.2 Topological Methods
   2.3 Hybrid Approaches
   2.4 Summary and Positioning
```

**Chronological:** Organize by timeline. Best for showing field evolution.

```
2. Evolution of the Field
   2.1 Early Methods (2010--2015)
   2.2 Deep Learning Era (2016--2020)
   2.3 Current Directions (2021--present)
```

**Methodological:** Organize by technique type.

```
2. Related Work
   2.1 Feature Extraction Methods
   2.2 Representation Learning Methods
   2.3 Classification Frameworks
```

### 5.2 Writing Tips

- **Synthesize, do not just summarize.** "Author A did X. Author B did Y." is a list, not a review. Instead: "While CNN-based methods [A, B] achieve high accuracy, they lack interpretability. GNN-based methods [C, D] address this but sacrifice computational efficiency."

- **Be critical but fair.** Point out limitations, but do not be dismissive. Every published paper passed peer review.

- **End each subsection with a gap.** After reviewing a category, explain what is still missing. This sets up YOUR contribution.

- **Position your work explicitly.** The last paragraph should say: "Unlike prior work that [limitation], our approach [difference]. Our work is closest to [X] but differs in [key way]."

### 5.3 Citation Density

A rough guide for citation density:

| Section | Citations per paragraph |
|---------|----------------------|
| Introduction | 2--4 |
| Related Work | 3--8 |
| Methodology | 0--2 (mostly self-referencing) |
| Experiments | 1--3 (baselines and datasets) |
| Conclusion | 0--1 |

---

## Phase 6: Maintain and Update

### 6.1 Set Up Alerts

- **Google Scholar Alerts:** Set up keyword alerts for your topic
- **Semantic Scholar:** Follow key authors and topics
- **arXiv alerts:** Subscribe to relevant categories (cs.CV, cs.LG, stat.ML, etc.)
- **Conference notifications:** Track paper acceptance lists for top venues

### 6.2 Regular Review Sessions

- Dedicate 2--3 hours per week to reading new papers
- Add relevant papers to your reference manager immediately
- Update your comparison matrix as the field evolves
- Review your gap analysis every 3--6 months

---

## Tools for Literature Review

| Tool | Purpose | Free? |
|------|---------|-------|
| **Zotero** | Reference management, PDF storage | Yes |
| **Mendeley** | Reference management, social features | Yes |
| **Paperpile** | Reference management, Google Docs integration | Paid |
| **Connected Papers** | Visual literature graph exploration | Free (limited) |
| **Litmaps** | Citation-based literature mapping | Free (limited) |
| **Research Rabbit** | Paper discovery and recommendations | Yes |
| **Elicit** | AI-powered literature search and extraction | Free (limited) |
| **Notion / Obsidian** | Structured note-taking | Free / Free |
| **Rayyan** | Systematic review screening tool | Yes |

---

## Common Mistakes

1. **Reading without a plan.** Aimless reading feels productive but wastes time. Always search with specific questions.
2. **Only reading abstracts.** Abstracts can be misleading. Read the methodology and results of key papers.
3. **Ignoring older papers.** Foundational work from 10--20 years ago often provides crucial context.
4. **Only reading your sub-field.** Adjacent fields may have solved your problem using different terminology.
5. **Hoarding papers.** Collecting 500 papers and reading none is worse than reading 50 papers deeply.
6. **Writing as you read.** Read first, synthesize second. Writing too early locks you into a premature structure.
7. **Not tracking what you have read.** You WILL forget which papers you have read if you do not track them.

---

> **Final thought:** A literature review is never truly "done." The field keeps moving. But at some point, you need to stop reading and start writing. Set a deadline, do your best, and accept that there will always be one more paper you could have included. The goal is thoroughness, not completeness.
