# Mortgage Calculator

A single-file mortgage calculator that runs entirely in the browser. No build step, no
dependencies to install, no server — open `index.html` and it works.

**Live demo:** https://YOUR-USERNAME.github.io/mortgage-calculator/

## Features

**Loan setup**
- Fixed-rate and adjustable-rate (ARM) mortgages
- ARM modelling: fixed period, adjustment interval, expected rate step, lifetime caps and floors
- Payment recalculated at every rate adjustment against the remaining balance and term

**Full monthly cost**
- Principal & interest, property tax (percentage or flat), home insurance, HOA, and other costs
- PMI applied automatically below 20% down, dropped the month the balance crosses your LTV threshold

**Points & closing costs**
- Discount points with a configurable rate reduction per point
- Break-even analysis: how long you must keep the loan for points to pay for themselves
- Closing costs paid out of pocket or rolled into the loan
- Cash-due-at-closing total

**Extra payments**
- Recurring monthly, annual (in a chosen calendar month), and one-time lump sums
- Interest saved and time cut, measured against a baseline schedule with no extras

**Budget**
- Take-home (net) pay, entered annually or monthly
- Unlimited custom expense lines — car payment, phone, utilities, anything
- Money left over each month, outgoings as a share of take-home pay, and an affordability verdict

**Comparison & refinance**
- Save up to 4 complete scenarios and compare them side by side, best value highlighted per row
- Refinance analysis with closing costs, cash-out, break-even, and lifetime savings

**Amortization**
- Full schedule in yearly or monthly view, including per-period rate changes on ARMs

## Deploying to GitHub Pages

1. Create a repository and push these files to the default branch.
2. Go to **Settings → Pages**.
3. Under **Source**, choose **Deploy from a branch**, pick your branch and the `/ (root)` folder.
4. Save. The site is live at `https://YOUR-USERNAME.github.io/REPO-NAME/` within a minute or two.

`index.html` must stay at the repository root for Pages to serve it as the landing page.

## Files

| File | Description |
|---|---|
| `index.html` | The calculator — self-contained HTML, CSS, and JavaScript |
| `mortgage-calculator.xlsx` | Spreadsheet version with live formulas; import into Excel or Google Sheets |

## Notes

- Chart.js is loaded from a CDN; everything else is inline.
- Nothing is transmitted anywhere. All figures stay in your browser.
- Saved comparison scenarios live in memory and reset when the page is reloaded.
- If your 401(k) is deducted before your pay reaches you, it is already excluded from
  take-home pay — add it as an expense line only if you contribute separately.

## Disclaimer

For planning and estimation only. Actual loan terms, escrow amounts, PMI rules, and closing
costs vary by lender and jurisdiction. Confirm any figure with your lender before relying on it.
