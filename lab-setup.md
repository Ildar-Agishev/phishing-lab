# 🔍 Phishing Attack Investigation – A Hands-On Security Lab

**Phishing** remains one of the most common and dangerous threats in the cybersecurity landscape. As part of my professional growth, I developed a hands-on phishing investigation lab to simulate real-world incident analysis. This blog-style post walks through the project’s stages and insights gained during the process.

---

## 🧪 Why This Lab?

The goal of this project was to practice **realistic techniques for phishing detection and analysis**, including:

- Identifying phishing characteristics
- Analyzing email headers
- Investigating suspicious links
- Documenting findings professionally

This is not a theory-based exercise — it simulates the type of work one might do in a SOC or during an actual incident response.

---

## 📌 Project Stages

### 1. Environment Setup

The first step was to establish a **safe, isolated lab environment** using:

- **MailCatcher** – a lightweight SMTP server that captures test emails
- **Thunderbird** – a reliable email client with header inspection support

> MailCatcher was used optionally in this lab to verify email reception and test Thunderbird configuration. If you're generating phishing emails yourself, isolating the environment is **mandatory** to avoid system compromise.

**Goal:** Create a safe workspace to analyze malicious content without risk.

---

### 2. Collecting Phishing Samples

I imported real phishing email samples sourced from malware traffic analyses rosurce :

- [malware-traffic-analysis.net](https://www.malware-traffic-analysis.net/)


These messages were loaded into Thunderbird for inspection.

**Goal:** Work with actual phishing examples for realistic analysis.

---

### 3. Identifying Phishing Indicators

Each email was reviewed for common phishing signs:

- Fake or spoofed sender addresses  
- Generic greetings (“Dear user”)  
- Urgent language or threats  
- Obfuscated or shortened links

**Goal:** Build awareness of how phishing attempts are crafted.

---

### 4. Email Header Analysis

Using Thunderbird email client, I examined raw headers to trace:

- Email routing paths (Received headers)  
- Sender IP addresses  
- Domain mismatch and SPF/DKIM failures

**Goal:** Uncover technical clues that reveal spoofing or forged origins.

---

### 5. Link Investigation

URLs found in the emails were extracted and analyzed using:

- [VirusTotal](https://www.virustotal.com/)  

This tool helps determine whether a link points to a malicious or deceptive site, without visiting it directly.

**Goal:** Identify potentially harmful destinations safely.

---

### 6. Report Writing

All findings were compiled into a **structured incident report**, including:

- 📝 Executive summary  
- ⚠️ Observed phishing indicators  
- 🧠 Technical analysis results  
- ✅ Recommendations for prevention

> This report simulates how investigations are documented in real-world cybersecurity teams.





