# Project Workflow

## 1. Contact Source

The system reads contact information from a Google Sheet containing company names, recipient names, job titles, and email addresses.

## 2. Contact Approval

Contacts are maintained in a separate tracking worksheet. Only contacts explicitly marked as approved are eligible for outreach.

## 3. Campaign Preview

Before sending, users can review eligible contacts, campaign settings, and email content.

## 4. Controlled Email Sending

Approved emails are sent through the Gmail API. Users can configure:

- Daily sending cap
- Batch size
- Fixed interval between emails
- Cooldown between batches
- Permitted sending hours

## 5. Persistent Tracking

The tracking worksheet records contact-level information, including:

- Approval and send status
- Sending timestamp
- Gmail message ID
- Attempt count
- Errors and suppression status

## 6. Interruption Recovery

If execution is interrupted, the system uses its persistent tracking records to identify completed and unresolved sends.

Contacts in uncertain states are flagged for manual reconciliation rather than automatically retried.

## 7. Campaign Monitoring

Users can review sent, pending, suppressed, and unresolved contacts through the tracking worksheets.

## Workflow Principle

The system separates contact approval, campaign execution, and tracking so that email outreach remains controlled and traceable.
