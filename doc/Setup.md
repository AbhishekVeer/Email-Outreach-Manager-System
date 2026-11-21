# Setup Guide

This guide explains how to prepare the Email Outreach Manager System for a test run.

## 1. Prerequisites

You will need:

- A Google account
- Google Drive and Google Sheets access
- Google Colab
- Gmail API access
- Google Sheets API access

## 2. Prepare the Sample Workbook

1. Download `sample_outreach_workbook.xlsx` from the repository.
2. Upload it to Google Drive.
3. Open it using Google Sheets.
4. Copy the Google Sheets URL.

The workbook contains fictional contacts. Use it for testing rather than real recipient data.

## 3. Open the Notebook

1. Navigate to `notebooks/resumable_outreach_manager.ipynb`.
2. Open the notebook in Google Colab.
3. Save a copy to your Google Drive.

## 4. Configure the Notebook

Review the configuration section and update the spreadsheet URL and sender details using your own authorised account.

Keep live sending disabled while testing.

## 5. Configure Credentials

Use Google Colab Secrets to store the required credentials.

The notebook expects these secret names:

- `GMAIL_CLIENT_ID`
- `GMAIL_CLIENT_SECRET`
- `GMAIL_REFRESH_TOKEN`

Never paste credentials into publicly visible notebook cells or commit them to GitHub.

You must configure the required Google API access and OAuth authorisation for your own account.

## 6. Test Before Sending

1. Run the notebook setup and authentication cells.
2. Validate the Google Sheets connection.
3. Review the contact and tracking worksheets.
4. Run the campaign preview.
5. Verify the recipient list and email template.

Only enable live sending after reviewing the configuration and confirming that you have permission to contact the recipients.

## Important

This project is a demonstration of controlled email outreach automation. Actual sending depends on your Google account permissions, API configuration, applicable sending limits, and compliance with relevant email policies.
