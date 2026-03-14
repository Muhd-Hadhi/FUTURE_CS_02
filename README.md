# FUTURE_CS_02
Future Intern Cybersecurity Task 2 : Phishing Email Detection & Awareness System
This repository contains a professional cybersecurity project focused on identifying, analyzing, and documenting real-world phishing threats. The assessment utilizes technical email header analysis and social engineering evaluation to classify various attack vectors and provide actionable prevention strategies.

Project Overview
Prepared By: Muhammed Hadhi K P 
Date: March 5, 2026 
Project ID: 002 

Objective: To analyze phishing indicators, examine sender authenticity, and strengthen organizational cybersecurity posture through employee awareness.

Methodology & Tools :
The analysis was performed using industry-standard diagnostic tools to examine the technical "digital fingerprints" of suspicious emails:
1.Google Admin Toolbox (Messageheader): Traced email paths and identified authentication results such as SPF, DKIM, and DMARC.
2.MXToolbox: Conducted deep header inspection and domain verification to identify spoofed domains and verify sender authenticity.
3.Browser Developer Tools: Safely inspected suspicious destination URLs and misleading links without interacting with malicious content.

WHOIS Analysis: Investigated the registration and reputation of suspicious relay domains (e.g., granigo.art).

Phishing Case Studies
The report details three distinct phishing attack vectors classified as high-risk:

1. Banking Fraud (Bradesco Livelo)
Attack Type: Reward/Point Expiry Scam.
Key Indicator: Infrastructure Trace. The email originated from DigitalOcean cloud infrastructure rather than legitimate banking servers.
Technical Failure: Failed SPF/DMARC checks and lacked a DKIM signature.

2. Loan Scam (Account Takeover)
Attack Type: Business Email Compromise (BEC) via Hijacked Account.
Key Indicator: Geographic Anomaly. An email from a Thai domain (.or.th) was sent via an African IP address.
Tactics: Used an off-platform pivot by directing victims to a private Gmail account to bypass corporate monitoring.

3. Health Scam (Brand Impersonation)
Attack Type: Brand Hijacking of a major e-commerce retailer (OTTO).
Key Indicator: Critical Spam Rating. Received an SCL Score of 9 (the highest possible "spammy" rating).
Tactics: Employed URL shorteners (t.co) to mask malicious redirection to scam sites.

Prevention & Best Practices :
The project concludes with a framework for building a "Human Firewall":

The "Do's" :
Verify Headers: Always check the "Display Name" against the actual sender address.
Hover Before Clicking: Inspect the actual destination URL for suspicious redirects.
Enable MFA: Implement Multi-Factor Authentication as a critical second layer of defense.

The "Don't s" :
Avoid "Urgency": Do not react to threatening language like "Expiring Today".
Skip "Unsubscribe" Links: In scam emails, clicking unsubscribe often confirms your email address is active to the attacker.
Restrict Attachments: Never download unsolicited files ending in .zip, .exe, or unexpected .pdf formats.

Conclusion: While an email might look perfect on the surface, technical failures like SPF SoftFails and DMARC mismatches provide the necessary evidence to identify a scam.
