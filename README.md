# Email-Outreach-Manager-System
A Python-based email outreach automation system using Google Colab, Google Sheets and Gmail API, featuring persistent tracking, batch controls and interruption recovery.

# Email Outreach Manager System

A Python-based email outreach automation system built with Google Colab, Google Sheets, and the Gmail API.

The project helps users manage structured email campaigns with contact-level tracking, controlled sending, persistent campaign records, and recovery mechanisms for interrupted execution.

## What does it do?

- **Contact management:** Reads contact information from Google Sheets.
- **Approval-based outreach:** Separates approved contacts from those awaiting approval.
- **Email automation:** Sends personalised emails through the Gmail API.
- **Campaign tracking:** Records send status, timestamps, message IDs, and attempt counts.
- **Duplicate-send prevention:** Excludes contacts already marked as successfully sent.
- **Interruption recovery:** Flags uncertain sending states for manual reconciliation instead of automatically retrying.
- **Batch controls:** Supports configurable daily limits, batch sizes, sending intervals, and cooldown periods.

## Technology Stack

- Python
- Google Colab
- Google Sheets
- Google Sheets API
- Gmail API
- OAuth 2.0
- Google Sheets as the campaign tracking database

## Project Outcomes

The system is designed to make outreach workflows more structured, traceable, and recoverable.

Its key outcomes include:

- Reduced risk of accidentally sending the same campaign email multiple times.
- Persistent records of approvals, sending activity, and campaign status.
- Better visibility into sent, pending, suppressed, and uncertain contacts.
- Recovery safeguards when a notebook session is interrupted.
- Configurable campaign controls rather than an uncontrolled bulk-send process.

In a working campaign workflow, the tracking mechanism retained contact-level send records across execution sessions. These are observed workflow outcomes, not guarantees of inbox delivery or campaign performance.

## Repository Structure

The repository will contain:

- `notebooks/` — Google Colab-compatible outreach automation notebook.
- `sample_outreach_workbook.xlsx` — Dummy workbook with fictional contacts and tracking sheets.
- `docs/` — Workflow and setup documentation.
- `requirements.txt` — Python dependencies.
- `.gitignore` — Excludes credentials and private campaign data.
- `SECURITY.md` — Security guidance.

## Getting Started

1. Download the sample workbook.
2. Upload it to Google Drive and open it with Google Sheets.
3. Open the notebook in Google Colab.
4. Configure the Google Sheets URL and sender details.
5. Set up Gmail API OAuth credentials using Colab Secrets.
6. Review the contact approval and campaign settings.
7. Run the preview before enabling live sending.

Detailed instructions will be provided in the project documentation.

## Security

- Never upload Gmail credentials, OAuth tokens, or private contact lists.
- Store credentials in Google Colab Secrets.
- Use the sample workbook for testing.
- Review recipients and message content before enabling live sending.
- Follow Google's applicable API policies and email-sending requirements.

## Important Limitations

- A successful Gmail API response indicates that Gmail accepted the send request; it does not guarantee inbox delivery.
- The Gmail send-only permission does not automatically detect replies.
- Google account limits and sending policies apply.
- Google Colab sessions can disconnect, so this is not an unattended email scheduler.

## Sample Data

The sample workbook uses fictional names and reserved `.test` email addresses. These addresses are non-deliverable and are intended only for demonstration and testing.

## License

MIT License.
