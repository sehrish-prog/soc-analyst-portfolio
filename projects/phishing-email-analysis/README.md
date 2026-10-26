# Phishing Email Analysis — Guided Exercise

## Scope
AI-assisted analysis of a fictional training email.
This is a text-only exercise, not a real incident.

## Evidence Reviewed
- Sender: helpdesk@company-security.example
- Reply-To: verify@external-mail.example
- Subject: URGENT: Your account will close in 30 minutes
- Message: Your mailbox access will be suspended.
  Verify your password immediately using this link:
  hxxps://account-check.example/login

## Findings
1. The suspension threat creates fear.
2. The deadline pressures the recipient to act quickly.
3. The password verification request suggests credential theft.
4. Different sender, Reply-To, and link domains warrant further investigation.

## Assessment
Suspected credential phishing based on the combined indicators.
Domain differences alone do not prove phishing.

## Recommended Response
- Do not submit credentials through the email link.
- Verify the request through a known IT support channel.
- Report the email to the security team.

## Limitations
No original headers or authentication results were available.
No website inspection or security tools were used.
The .example domains are fictional placeholders.

## Learning
Recognizing social engineering indicators and documenting
findings while clearly stating investigation limitations.
