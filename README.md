# Prahari AI — HERHACK 2026 MVP

A small, privacy-first phishing-awareness demo. It analyses pasted messages and URLs for common warning signs and explains its findings.

## Run it
**Fastest:** Open `index.html` in Chrome or Edge. No Node.js, npm, Python, server, or API key is required.

## Publish with GitHub Pages
1. Create a **public** GitHub repository named `Prahari-AI`.
2. Upload `index.html`, `README.md`, and the `tests/` folder.
3. In the repository, open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select branch `main`, folder `/ (root)`, then Save.
6. Wait for the Pages URL to appear. It will look like `https://YOUR-USERNAME.github.io/Prahari-AI/`.

## Demo
Open the page and click any sample on the right. Click **Analyse input**. Try all five samples, then test your own harmless examples.

## Important limitations
- This is a transparent rule-based educational prototype, not a trained AI model, antivirus, threat-intelligence service, or guarantee.
- The score is an illustrative indicator score, **not** a probability or measured accuracy.
- A low-risk result does not prove a message or site is safe. A high-risk result is a prompt to verify, not a definitive verdict.
- It does not visit, download, or execute links or files.
- Inputs are processed in the browser and are not sent to a server or saved.

## Safety
Use only the synthetic examples supplied in this project or messages you are authorised to analyse. Never test with real malware, exploit payloads, stolen credentials, OTPs, or private financial information. Do not click suspicious links. Verify organisations through contact details from their official app or website.

## Project structure
- `index.html` — complete browser-based demo (HTML, CSS, JavaScript)
- `tests/test-cases.md` — synthetic test cases and expected behaviour

## Future work
A backend API, carefully evaluated ML classifier, multilingual support, URL reputation feeds, accessibility improvements, and a documented false-positive/false-negative evaluation.
