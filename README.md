# Nothing to Declare: internal version

**Private. Contains real names. Do not share outside Straive.**

This is the named version of the [public dashboard](https://eshwarpotturi.github.io/nothing-to-declare/). It shows every flagged author by name, with links to the paper, Google Scholar, ORCID and their record in the US government's Open Payments database.

## Live site

https://eshwarpotturi.github.io/nothing-to-declare-internal/

Tabs: The study, Food and beverage, By publisher, and **Check a DOI** (link straight to it: `/#doi`).

## Check a DOI

Enter a DOI to see whether the authors' declaration matches US payment records (Open Payments, 2020 to 2025).

- **Paper in the study (2,878 papers):** shows the study's own result: valid, invalid, limited declaration or cannot check, with the payments behind it.
- **Any other DOI:** checked live. The paper and its declaration come from Europe PMC. Payments come from the Open Payments API for US authors in the 36 months before the paper was submitted. Authors are matched by name and place, so each result links to the Open Payments record to check by hand.
- **What can be checked:** the paper must be in Europe PMC (PubMed and PubMed Central), and its full text must be in PubMed Central so the declaration can be read. That depends on open access, not on the publisher: Wiley, Springer, Elsevier and Oxford papers are covered when they are open access. The page says which of these applies: "Paper not found" (not in Europe PMC) or "Paper found, declaration not readable" (no full text). For the second, a button looks up payments anyway.
- **Check this paper live as well:** on a study paper, re-runs the live check so the two results can be compared.

## How to open it

1. Click `index.html` above, then **Download raw file** (the download icon at the top right).
2. Double-click the downloaded file. It opens in your browser and needs no internet connection except for the links.

## What is in it

- 2,878 papers and 15,652 checked US authors (October 2023 to October 2026). 1,492 authors in 814 papers (nearly 3 in 10) did not declare payments.
- **Checked by hand:** 10 cases with every dated payment record, plus the results of 43 random hand checks and what each error taught us.
- A red flag is a question for an editor, not a finding of misconduct.

## Rebuilding it

Run `python run.py` then `python pipeline/s5_full.py` in the public repository, and copy `private/full/nothing-to-declare-full.html` here as `index.html`.
