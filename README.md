# -Analyze-a-Phishing-Email-Sample
 Identify phishing characteristics in a suspicious email sample

Objective:
Analyze the provided phishing email sample and identify phishing characteristics (sender spoofing, header anomalies, suspicious links/phone, language issues, social-engineering cues). Produce a report suitable for upload to GitHub and submission

/
├─ README.md            ← this file
├─ evidence/
│  ├─ sample_email.txt   ← raw email body (sample)
│  └─ sample_headers.txt ← constructed/raw headers used for analysis
└─ report.pdf           ← optional PDF version of this report

From: Microsoft Team <

Windows Error Report

Windows User Alert

# Unusual sign-in activity

We detected something unusual to use an application to sign in to your Windows Computer. We have fc:njnd suspicious login attempt on your windows computer through an unknown source. When our security officers investigated. it was found out that someone from' foreign LP Address was trying to make a prohibited connection on your network which can corrupt your windows license key.

Sign-in details:

Country/region: Lagos, Nigeria

IP Address: 293.09.101.9

Date: 09/07/2016 02:16 AM (GMT)

If you're sure this was you. a malicious user might trying to access your network. Please review your recent activity and we'll help you take corrective action. Please contact Security Communication Center and report to us immediately. 1 •8008160380 or substitute you can also visit the Website: ht(ps;//wwwxmi«osoft.com/and fill out the consumer complaint form. Once you call. please provide your Reference no: AZ- 1190 in order for technicians to assist you better.

Our Microsoft certified technician will provide you the best resolution. You have received this mandatory email service announcement to update you about important changes to your Windows Device.

Return-Path: <noreply@micr0soft-support.com>
Received: from mail.fakeisp.ru (mail.fakeisp.ru [185.77.12.34])
        by mx.google.com with ESMTP id abc123xyz
        for <victim@example.com>;
        Tue, 7 Sep 2016 02:16:34 -0700 (PDT)
Received-SPF: fail (google.com: domain of noreply@micr0soft-support.com does not designate 185.77.12.34 as permitted sender)
Authentication-Results: mx.google.com;
       spf=fail (google.com: domain of noreply@micr0soft-support.com does not designate 185.77.12.34 as permitted sender) smtp.mailfrom=noreply@micr0soft-support.com;
       dkim=none (message not signed)
       dmarc=fail (p=REJECT) header.from=micr0soft-support.com
Message-ID: <201609070216@mail.fakeisp.ru>
From: "Microsoft Team" <noreply@micr0soft-support.com>
To: victim@example.com
Subject: Windows User Alert - Unusual sign-in activity
Date: Tue, 7 Sep 2016 02:16:00 +0000

Phishing indicators (findings)
Header-level indicators

From / Return-Path mismatch / typosquatting: micr0soft-support.com (uses a zero instead of an "o") — lookalike domain tactic.

Suspicious sending host / IP: Message appears to originate from mail.fakeisp.ru / 185.77.12.34 — not a Microsoft IP.

Authentication failures: spf=fail, dkim=none, dmarc=fail — strong signs of spoofing.

Message-ID domain mismatch: mail.fakeisp.ru vs. microsoft.com.

Body-level indicators

Brand impersonation: Claims to be from “Microsoft Team” / “Windows Error Report.”

Malformed / obfuscated URL: ht(ps;//wwwxmi«osoft.com/ — not a valid Microsoft URL; likely malicious.

Unsolicited phone number: 1 •8008160380 — attackers often use fake support numbers to social-engineer victims.

Invalid IP format: 293.09.101.9 — 293 is not a valid octet (0–255); indicates fabrication.

Old/irrelevant date: 09/07/2016 — inconsistent with an immediate security alert.

Poor grammar/typos/punctuation errors: multiple mistakes (e.g., fc:njnd, someone from' foreign LP Address) — legitimate vendor messages are professionally written.

Generic greeting / no personalization: no recipient name or account details.

Urgency / scare tactics: language designed to provoke immediate action.

Social-engineering cues

Fear-based messaging (license corruption) and a provided reference number (AZ- 1190) to feign legitimacy.

Push to call or visit the provided link/number for immediate remediation.
