# Client Reporting Automation

An automated monthly advertising reporting workflow built for digital marketing agencies using Make.com.

## Project Overview

This project automates the process of collecting advertising campaign data, calculating performance metrics, generating AI-powered insights, creating a client-ready PDF report, and recording report details.

## Problem Statement

Marketing agencies often spend time manually collecting campaign data, calculating KPIs, preparing performance reports, and emailing clients.

This workflow reduces repetitive reporting work through automation.

## Technology Stack

| Tool | Purpose |
|---|---|
| Make.com | Workflow orchestration |
| Google Sheets | Campaign data and KPI calculations |
| Gemini 2.5 Flash | AI campaign analysis |
| Google Docs | Report generation |
| Gmail | PDF email delivery |
| Airtable | Reporting records |

## Workflow Architecture

1. Retrieve Meta Ads and Google Ads campaign data from Google Sheets.
2. Aggregate campaign records.
3. Convert campaign data into JSON.
4. Generate campaign analysis using Gemini.
5. Retrieve calculated KPIs.
6. Generate a Google Docs report using a template.
7. Export the report as a PDF.
8. Send the PDF through Gmail.
9. Store report details and status in Airtable.

## Key Performance Metrics

- Total Ad Spend
- Impressions
- Clicks
- Leads
- Revenue
- Average CPC
- Average CPL
- Click-through Rate (CTR)
- Return on Ad Spend (ROAS)

## Error Handling

- Incomplete execution storage enabled.
- Automatic retry configured for Gemini HTTP requests.
- Automatic retry configured for Gmail delivery.
- Three retry attempts with five-minute intervals.

## Testing

The workflow has been tested using sample campaign data.

Verified outputs include:
- AI-generated campaign analysis
- Google Docs report with performance charts
- PDF export
- Gmail delivery with PDF attachment
- Airtable reporting record

## Project Status

Core workflow implemented and successfully tested.

## Repository Structure

```text
taw-make-client-reporting/
├── README.md
└── docs/
    └── project-overview.md
```

## Important Note

This project currently uses Gemini for AI analysis. Campaign data is supplied through Google Sheets test data; live advertising API integrations should not be assumed.

