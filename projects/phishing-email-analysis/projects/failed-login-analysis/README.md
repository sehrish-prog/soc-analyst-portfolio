# Failed Login Analysis — Guided Exercise

## Scope
AI-assisted review of five fictional login events.
This is a text-only training exercise; no SIEM was used.

## Sample Logs
```text
09:00:01  user=admin  source=192.0.2.25  result=FAILED
09:00:04  user=admin  source=192.0.2.25  result=FAILED
09:00:07  user=admin  source=192.0.2.25  result=FAILED
09:00:10  user=admin  source=192.0.2.25  result=FAILED
09:00:13  user=admin  source=192.0.2.25  result=SUCCESS
```

## Findings
- Account: admin
- Source IP: 192.0.2.25
- Four failed attempts followed by one successful login.
- Events occurred three seconds apart.
- Total time from first failure to success: 12 seconds.

## Assessment
Possible password guessing, requiring further investigation.
A legitimate user correcting a password is another explanation.
These logs alone do not confirm account compromise.

## Proposed Investigation Steps
1. Confirm whether the account owner recognizes the login.
2. Check whether the source matches an expected device or VPN.
3. Review MFA results and additional authentication logs.
4. Review activity after the successful login.
5. Escalate unexpected activity according to the response procedure.

## Limitations
The date, timezone, destination system, authentication method,
and post-login activity were not provided.
192.0.2.25 is a documentation address used for this exercise.
No real account or system was investigated.

## Learning
Identify login patterns, calculate time intervals, and separate
observed evidence from possible explanations.
