# HelixPulse — Genomic Sequence Explorer

A responsive, static educational web application for exploring DNA sequence composition and a transparent decision-tree classification example. Built with HTML, CSS, and vanilla JavaScript; no build step or API key is required.

## Features

- DNA sequence input with live sanitization and validation (A, T, G, C only)
- Feature extraction: A/T/G/C counts, sequence length, and GC/AT content ratios
- Proportional base spectrum bar and vertical relative distribution chart
- Four assignment-provided training samples (S1–S4) with instant one-click loading
- Educational GC-content decision-rule demonstration for Group A / Group B (56.25% threshold)
- Interactive training set table with record filtering and CSV feature matrix export
- Responsive layout with dark and daylight laboratory appearance toggle

## Run locally

1. Download or clone this repository.
2. Open `index.html` in a modern web browser.

No package installation or server is needed.

## Deploy to Vercel

### Option 1: Import from GitHub

1. Create a GitHub repository and upload `index.html`, `style.css`, `app.js`, and `README.md`.
2. Sign in to Vercel and choose **Add New → Project**.
3. Import your GitHub repository.
4. Keep the Framework Preset as **Other**.
5. Leave Build Command and Output Directory empty (or use `.` as the output directory if prompted).
6. Click **Deploy**.

### Option 2: Vercel CLI

If you have Node.js and Vercel CLI installed, run `vercel` from this project folder and follow the prompts.

## Important Academic Note

The assignment asks students to run a Python / Google Colab classifier, report the model output and accuracy, and submit a PDF with screenshots and discussion. This website is an interactive educational companion/demo, not a replacement for that required Python implementation.

The browser demo uses a transparent one-split rule on GC content (threshold 56.25%) to illustrate classification on the four supplied examples. It is **not** an actual scikit-learn DecisionTreeClassifier, does not perform independent testing, and does not establish reliable predictive performance. With only four samples, training accuracy is not evidence of generalization. The unknown sequence's true group is not supplied, so prediction correctness cannot be confirmed.

This educational tool is not intended for medical, diagnostic, clinical, or research use.