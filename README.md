# Nothing to Declare: internal version

**Private. Contains real names. Do not share outside Straive.**

This is the named version of the [public dashboard](https://eshwarpotturi.github.io/nothing-to-declare/). It shows every flagged author by name, with links to the paper, Google Scholar, ORCID and their record in the US government's Open Payments database.

## How to open it

1. Click `index.html` above, then **Download raw file** (the download icon at the top right).
2. Double-click the downloaded file. It opens in your browser and needs no internet connection except for the links.

## What is in it

- 2,878 papers and 15,652 checked US authors (October 2023 to October 2026). 1,523 authors in 835 papers (3 in 10) did not declare payments.
- **Checked by hand:** 10 cases with every dated payment record, plus the results of 43 random hand checks and what each error taught us.
- A red flag is a question for an editor, not a finding of misconduct.

## Rebuilding it

Run `python run.py` then `python pipeline/s5_full.py` in the public repository, and copy `private/full/nothing-to-declare-full.html` here as `index.html`.
