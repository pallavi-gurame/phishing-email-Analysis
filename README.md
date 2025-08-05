# phishing-email-Analysis
Analysis of a phishing email sample using Gmail header and MxToolbox to detect spoofing and phishing indicators.

Objective
To analyze a suspicious email sample and identify phishing characteristics using Gmail's "Show Original" view and email header analysis.

 Tools Used
- Gmail – Show Original feature
- MXToolbox Email Header Analyzer
- Screenshot tool (Snipping Tool / Lightshot)


 Steps Performed
1. Opened the phishing email in Gmail.
2. Selected Show Original to view full email headers.
3. Copied the header section and analyzed it in MXToolbox.
4. Checked SPF, DKIM, and DMARC results.
5. Examined the email body for suspicious elements.
6. Saved screenshots of:
   - Original view in Gmail
   - MXToolbox results
   - Email body

 Phishing Indicators Found

SPF/DKIM/DMARC failures - The sending IP (203.0.113.50) is not authorized to send for `yourbank-support.com`.
Domain mismatch  - "From" address claims to be from `secure-update@yourbank-support.com` but was sent from a Gmail server.
Reply-To mismatch - Reply-To points to `securehelpdesk@gmail.com`, not the bank’s official domain.
Urgent tone in subject  - "Your Bank Account Will Be Suspended!" designed to create panic.
Suspicious link -  Hovering over the "Verify Now" button shows `http://bank-security-update-login.com` instead of the bank’s official website.
Generic greeting  -  "Dear Customer" instead of the recipient’s real name.



 Screenshots in This Repository
screenshots/original_view.png` – Gmail Show Original
screenshots/mxtoolbox_result.png` – Header analysis
screenshots/email_body.png` – Suspicious content

Conclusion
The analyzed email is confirmed to be a phishing attempt using:
- Domain spoofing
- Social engineering with urgency
- Malicious link targeting credential theft

