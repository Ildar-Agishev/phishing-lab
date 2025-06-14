# Phishing Attack Investigation: My Hands-On Experience

## Introduction

Phishing remains one of the most common and dangerous cybersecurity threats today. As part of my learning journey, I decided to dive deeper into this topic by setting up my own lab environment and conducting a phishing investigation from start to finish. In this post, I’m sharing how I approached it, the tools I used, and what I learned along the way.

## What I Knew Before Getting Started

Before I began, I made sure I had a basic understanding of:
- How email systems work
- Common phishing techniques
- Tools used for analyzing emails

## Lab Environment & Tools I Used

To safely analyze phishing emails, I set up a local environment. Here's how I approached it:

### 1. Email Server Simulation (Optional)

You can use a simulated mail server to test and analyze phishing emails in a controlled environment without risking the real inbox.

**Tool:**
- **MailCatcher** — a simple SMTP server that captures emails for inspection.


### 2. Phishing Email Samples

To practice, I collected 4 phishing email samples from https://www.malware-traffic-analysis.net/2020/05/05/index.html

### 3. Email Analysis Tools

- **Thunderbird** — Mozilla’s email client that makes email inspection and management easy.

## Setting Up the Environment

### Installing Thunderbird

I downloaded Thunderbird from the [official site](https://www.thunderbird.net/) and connected it to my local email setup using MailCatcher.

### Configuring MailCatcher

```bash
gem install mailcatcher
mailcatcher
```

MailCatcher runs locally and is accessible via [http://127.0.0.1:1080](http://127.0.0.1:1080), which allows to view captured emails in a safe way.

### Importing Phishing Samples

I downloaded samples from PhishTank and OpenPhish, then loaded them into Thunderbird for analysis.

### Setting Up PhishTool

I created a free account at PhishTool and followed their integration guide to connect it to Thunderbird. This made analysis more structured and insightful.

## Practical Exercises

### Exercise 1: Identifying Phishing Emails

**Goal**: Learn how to spot phishing emails based on common red flags.

**What I did**:
- Opened email samples in Thunderbird
- Looked for suspicious elements like fake sender addresses, generic greetings, urgency tactics, and dodgy links

**Outcome**:
A list of phishing emails with annotations highlighting key indicators.

---

### Exercise 2: Email Header Analysis

**Goal**: Understand how to trace email origins through header inspection.

**Steps**:
- Opened full email headers
- Identified the sender’s IP, mail server hops, and inconsistencies in the metadata

**Outcome**:
A detailed breakdown of header information with notes on suspicious patterns.

---

### Exercise 3: Investigating Suspicious Links

**Goal**: Learn to safely investigate URLs without compromising security.

**Steps**:
- Extracted links from phishing emails
- Ran them through services like VirusTotal and PhishTool
- Assessed threat levels and activity

**Outcome**:
A report with findings for each link, including screenshots and risk assessments.

---

### Exercise 4: Compiling an Investigation Report

**Goal**: Document the entire phishing analysis process in a professional format.

**Report structure**:
- Executive summary
- Breakdown of phishing indicators
- Email header analysis
- Link investigation
- Recommendations for prevention

**Outcome**:
A comprehensive report that could be shared with a security team or used for educational purposes.

## Helpful Resources

- [PhishTool](https://phishtool.com)
- [VirusTotal](https://www.virustotal.com)
- [How to View Email Headers (Gmail)](https://support.google.com/mail/answer/22454?hl=en)

---

By going through this project hands-on, I gained practical experience in identifying, analyzing, and documenting phishing attacks. This was a great step in developing my cybersecurity skills, especially in email threat analysis and incident response.

Feel free to reach out or fork this project if you're exploring the same!
