# Evalora AI — Answer Sheet Evaluation Demo

A GitHub-ready frontend demo for an AI-based answer sheet evaluation system. It presents the project as a usable product and demonstrates the scoring logic in the browser.

## Features

- Paste a reference answer and a student response
- Load a student response from a `.txt` file or answer-sheet image (`.png`, `.jpg`, `.webp`)
- Extract answer text from an image using browser-based OCR (Tesseract.js)
- Text preprocessing (tokenisation and stop-word removal)
- TF-style term vectors with cosine similarity scoring
- Concept-coverage check and a transparent audit trail
- Responsive, dependency-free interface suitable for GitHub Pages

## Run locally

Open `index.html` in a browser. No installation is required. The OCR library loads from a public CDN, so an internet connection is needed when extracting image text.

## Publish on GitHub Pages

Push this folder to a GitHub repository. In **Settings → Pages**, select **Deploy from a branch**, then choose your main branch and the root folder.

## Production architecture

This portfolio demo keeps evaluation in the browser. The full project described in the resume would use Django for authentication, submissions, persistent audit records, OCR extraction (for example, Tesseract), and a server-side NLP pipeline using scikit-learn's `TfidfVectorizer` and cosine similarity.

## Tech stack

Python · Django · OCR · NLP · TF-IDF · Cosine Similarity · JavaScript
