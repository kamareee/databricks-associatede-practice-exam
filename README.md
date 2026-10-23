# Databricks Data Engineer Associate: Practice Exam

A full-length, 45-question mock exam for the **Databricks Certified Data Engineer Associate** certification, weighted to the exam guide that took effect on **4 May 2026**.

It is a single self-contained HTML page (`index.html`) with no build step and no dependencies apart from Google Fonts, so it runs on GitHub Pages or straight from your file system.

> Unofficial practice material. Not affiliated with or endorsed by Databricks. All questions are original; none of the official sample questions are reproduced.

## Modes

| Mode | Timer | Feedback |
|---|---|---|
| **Timed exam** | 90-minute countdown; auto-submits at zero | None until you submit. Flag questions and return to them, as in the proctored exam. |
| **Practice** | Elapsed time only | Check each answer and read the explanation before moving on. |

Both modes finish on a results screen with:

- your overall score against a 70% target line
- a score for each section
- a review list you can filter by incorrect or skipped questions, flagged questions, or section

Each reviewed question shows its explanation and links to the relevant Databricks docs.

Keyboard: `A`–`D` (or `1`–`4`) selects an answer, `←`/`→` moves between questions, `F` flags.

## Blueprint coverage

The question count for each section is 45 × the published weight, rounded. CI/CD and Troubleshooting both come to 4.5; one was rounded down and the other up.

| # | Section | Weight | Questions |
|---|---|---:|---:|
| 1 | Databricks Intelligence Platform | 6% | 3 |
| 2 | Data Ingestion and Loading | 21% | 9 |
| 3 | Data Transformation and Modeling | 22% | 10 |
| 4 | Working with Lakeflow Jobs | 16% | 7 |
| 5 | Implementing CI/CD | 10% | 4 |
| 6 | Troubleshooting, Monitoring, and Optimization | 10% | 5 |
| 7 | Governance and Security | 15% | 7 |
| | **Total** | **100%** | **45** |

Questions appear in a fixed mixed order, as on the real exam. Every question is single-answer with four options, and correct answers are spread evenly across A–D.

## Run it

**On GitHub Pages**

1. Make sure the repository is public. GitHub Free publishes Pages only from public repositories.
2. Go to **Settings → Pages**.
3. Under **Build and deployment**, set **Source** to **Deploy from a branch**. Set the branch to `main` and the folder to `/ (root)`, then click **Save**.
4. After a minute or two the site is live at `https://kamareee.github.io/databricks-associatede-practice-exam/`.

`.nojekyll` tells Pages to serve the files as they are, without a Jekyll build.

**Locally:** open `index.html` in a browser.

## How progress is stored

- Attempts are saved in your browser's `localStorage`, separately for each site and each browser. Your phone and your laptop keep separate attempts, and nothing is sent anywhere.
- The timer counts real elapsed time. Closing the tab does not pause it. When you reopen the page, it resumes with the time left, or submits if time has run out.
- Starting a new attempt asks you to confirm before it discards one that is in progress.

## Caveats

- **Pass mark.** The May 2026 guide does not publish one. The 70% line is a target only.
- **Unscored items.** The real exam can include unscored questions, with extra time allowed for them.
- **DENY.** The guide lists DENY as an objective. However, the SQL `DENY` statement applies only to legacy `hive_metastore` objects. Unity Catalog's ABAC DENY policies are in Beta and, per current docs, cover only the MANAGE ACCESS CONTROL privilege. The relevant question explains this.
- **Freshness.** Facts were checked against Databricks documentation on 23 October 2026. Beta features (ABAC and ABAC DENY policies) and product names (Lakeflow, Declarative Automation Bundles) may change.
- **Doc links.** A few links point to a parent docs page where the exact page couldn't be confirmed.

## Sources

- [Data Engineer Associate exam guide (May 2026)](https://www.databricks.com/sites/default/files/2026-05/databricks-certified-data-engineer-associate-exam-guide-may-2026-000.pdf). Its five retired sample questions make a good warm-up.
- [Certification page](https://www.databricks.com/learn/certification/data-engineer-associate)
- [Databricks documentation](https://docs.databricks.com/aws/en/)
