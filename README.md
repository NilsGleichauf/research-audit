# Column Decoder (MVP)

Open a messy research spreadsheet and get a draft data dictionary: what each column seems to hold, what looks inconsistent, and which columns could identify a patient.

**Live demo:** https://nilsgleichauf.github.io/research-audit/

## How to use

1. Open the link above.
2. Click **Use demo sheet (fake patients)**, or choose your own spreadsheet.
3. Check that the sheet and header row are right, then read the column table.

You can also download `sample_fake_dataset.xlsx` from this repo and load it with **Choose File**. It's the same kind of made-up data, no real patients.

## Privacy

The file is read inside your browser tab. Nothing is uploaded or stored. The demo sheet is made up and contains no real patient data.

## What works so far

- Finds the header row automatically and skips title rows and blank rows
- Guesses the type of each column and how many cells are filled
- Summarizes the values in each column
- Flags problems like text in a number column or mixed date formats
- Rates how likely each column is to identify a patient

## Not built yet

The dataset summary and the PubMed suggestions are placeholders. With more time they would come from a language model running locally on the lab computer, so no patient data leaves it.

## Why

New lab members often inherit Excel files with cryptic column names and no documentation. This tool gives them a first map of the data before they start working with it.

Built for ENG-SCI 30 (Harvard, Fall 2026), Assignment 2b.
