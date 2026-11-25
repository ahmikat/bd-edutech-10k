---
language:
- bn
- en
task_categories:
- text-classification
license: other
pretty_name: BD-EduTech-10k
---

# BD-EduTech-10k

BD-EduTech-10k contains 10,088 Bangla, Banglish and English comments from Bangladeshi educational technology platforms. It supports sentence-level sentiment classification, multi-label aspect-category detection and aspect-category sentiment analysis (ACSA).

## Dataset

The comments were collected from YouTube, Facebook, Google Play Store and Reddit, covering providers such as 10 Minute School, Shikho, Bohubrihi, Udvash and ACS. The paper describes the two-phase human annotation procedure in Section III. Direct account identifiers were excluded during collection.

| Sentence sentiment | Count      |
| ------------------ | ----------:|
| Positive           | 3,461      |
| Neutral            | 3,378      |
| Negative           | 3,249      |
| **Total**          | **10,088** |

There are 6,170 single-category comments and 3,918 dual-category comments (38.84%). Single-category ACSA labels inherit sentence sentiment; dual-category comments receive separate aspect sentiment labels. The six categories and their CSV columns are defined in `label_schema.json`.

## Files and splits

| File                  | Rows  |
| --------------------- | -----:|
| `data/train.csv`      | 7,062 |
| `data/validation.csv` | 1,515 |
| `data/test.csv`       | 1,511 |



## Annotation and data quality

`annotation_guidelines.pdf` describes the annotation procedure and label definitions based on Section III of the paper.  The supplied annotations are preserved, including eight rows with category/ACSA presence differences documented in `label_schema.json`.

## Access and use

This dataset is released for research and educational use under the terms in `LICENSE`. The supplied comment text is preserved. Users must respect commenter privacy, applicable platform terms and third-party rights. The dataset is intended for aggregate analysis, not decisions about individuals.

## Authors and citation

- Aftab Hossain Mikat — Rajshahi University of Engineering & Technology (RUET)
- Tamjid Hasan Fahim — Rajshahi University of Engineering and Technology (RUET)
- Md. Shadikur Rahman Shadiq — Rajshahi University of Engineering and Technology (RUET)
- Sazzad Ahmed — Khulna University of Engineering & Technology (KUET)

Primary contact: drmikat@gmail.com

Associated paper: *BD-EduTech-10k: Multi-Task Aspect-Category Analysis for Trilingual EduTech Feedback* (2026). See `CITATION.cff` for citation details.
