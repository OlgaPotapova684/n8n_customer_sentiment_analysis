# Customer Sentiment Analysis Workflow (n8n)

## Overview
This n8n workflow automates the analysis of customer reviews from Google Sheets using **custom JavaScript sentiment analysis**. It classifies reviews as positive, negative, or neutral based on key words and updates the results back into Google Sheets.

## Features
- Fetches customer reviews from a Google Sheet.
- Iterates over reviews using batch processing.
- Analyzes sentiment using custom JavaScript rules:
  - Positive keywords: "отлич", "супер", "удоб", "рекомендую", "нрав", "люблю"
  - Negative keywords: "плохо", "долго", "ужас", "ненавижу", "не нрав", "проблем"
- Classifies each review as **positive**, **negative**, or **neutral**.
- Writes the sentiment result back into the Google Sheet.

## Workflow Steps
1. **Manual Trigger** – Starts the workflow manually.
2. **Get row(s) in sheet** – Retrieves reviews from Google Sheets.
3. **Loop Over Items** – Iterates over each review.
4. **Code in JavaScript** – Applies custom sentiment analysis rules to determine sentiment.
5. **Append row in sheet** – Updates the sentiment classification back into the Google Sheet.

## Technology Stack
- [n8n](https://n8n.io/) – Workflow automation.
- Google Sheets API – Reads and writes customer review data.
- JavaScript – Custom sentiment analysis rules.

## Usage
1. Clone this repository.
2. Import the workflow into your n8n instance.
3. Replace placeholders `<GDRIVE_ID>` and `<CREDENTIALS>` with your own Google Sheets document ID and credentials.
4. Click **Execute Workflow** to process reviews and classify sentiments.

---

> **Note:** All credentials and Google Sheet IDs have been removed from this workflow. Replace placeholders with your own credentials before running.
