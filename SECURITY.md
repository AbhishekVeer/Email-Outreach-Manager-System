# Security Policy

## Protecting Credentials

This project uses Google APIs to access Google Sheets and send emails.

- Never commit OAuth client secrets, refresh tokens, access tokens, or API credentials.
- Store credentials securely using Google Colab Secrets or an equivalent secrets manager.
- Do not hardcode credentials in notebook cells.
- Never share your authenticated notebook or credential files publicly.

## Protecting Contact Data

- Use fictional data when testing or demonstrating the project.
- Do not upload private contact lists or confidential campaign information to this public repository.
- Obtain appropriate consent and follow applicable privacy and email communication laws before contacting recipients.
- Respect opt-outs and maintain suppression records.

## Safe Execution

- Review the recipient list and email template before sending.
- Keep live sending disabled until the configuration has been checked.
- Use the preview functionality before enabling live sending.
- Follow Google's Gmail API policies and applicable sending limits.

## Reporting a Security Issue

If you identify a security vulnerability, avoid publishing credentials, personal information, or exploit details in a public issue. Contact the repository owner privately through GitHub.
