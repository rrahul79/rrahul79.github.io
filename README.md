# Rahul V — Data Engineering Portfolio

A responsive static portfolio with engineering case studies, a working browser-based ETL lab and a SQL notebook. Built with HTML, CSS and JavaScript. No backend, API keys, build step or paid services.

## Run locally

From this directory run `python3 -m http.server 8080 --directory dist`, then open http://localhost:8080.

## Publish with GitHub Pages

1. Create a GitHub repository, for example `data-engineering-portfolio`.
2. Upload **the contents of `dist`** (`index.html`, `style.css`, `app.js`) to the repository root. Also upload this README if desired.
3. In the repository open **Settings → Pages**.
4. Under Build and deployment select **Deploy from a branch**, choose **main** and **/(root)**, then Save.
5. When deployment completes, use the Pages URL shown by GitHub in your resume.

Relative asset links support both project repositories and username.github.io repositories. Do not upload the Sites `.openai` folder to your GitHub portfolio.

## Content and editing

- `dist/index.html`: biography, projects, skills, contact links and certifications.
- `dist/style.css`: colours, spacing, layout, mobile and print styles.
- `dist/app.js`: sample dataset, ETL demo, SQL notebook and expandable project notes.
- Google Fonts is optional; the site falls back to system fonts if unavailable.
- Contact uses a mailto link; there is no form backend or visitor tracking.
- Resume links download the supplied data-engineering CV as resume.pdf.
- Your GitHub profile and public repository links are included.

## Demo contract

Synthetic source: 6 base orders, optionally plus 1 duplicate and 2 invalid records. Validate required fields, valid ISO date, positive amount and allowed status. Keep the first valid record per order ID. Retain completed orders and sum daily revenue.

Expected output in both modes: 4 completed orders, revenue INR 5,600; daily totals INR 2,000 / 1,500 / 2,100. Dirty mode: 9 input rows and 3 quality exclusions. Clean mode: 6 input rows and 0 quality exclusions. Pending and cancelled rows are excluded separately after quality validation. Repeated runs replace output and do not accumulate values.

SQL examples use Snowflake syntax and are illustrative; they do not execute against a database. The browser lab demonstrates ETL concepts, not distributed AWS execution.

Professional project descriptions contain no client data, proprietary code or unverified numeric achievements. Review professional statements before making your GitHub repository public.

## Repository collection

Public GitHub snapshot reviewed 15 November 2026. All 16 public repositories are linked, including profile and archive entries. Filters group AI, Python/NLP, web applications and portfolio experiments. Repository descriptions distinguish available source, documentation-only projects and minimal contents. JobPilot AI remains in progress.
