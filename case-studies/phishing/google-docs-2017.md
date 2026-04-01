# Google Docs Phishing Worm (2017)

## Source
https://krebsonsecurity.com/2017/05/massive-google-docs-phishing-worm/

---

## Overview
In 2017, a large-scale phishing attack spread rapidly by impersonating a legitimate Google Docs sharing request. Victims received emails that appeared to come from trusted contacts, prompting them to click a link to view a document.

Instead of opening a document, the link asked users to grant permissions to a malicious Google app. Once access was granted, the attacker gained access to the user’s email account and contact list, allowing the phishing email to automatically spread to others.

---

## Techniques Used

- Social Engineering  
  Emails appeared to come from known contacts and leveraged trust to increase click rates  

- OAuth Abuse  
  Victims granted app permissions instead of entering credentials, bypassing traditional detection  

- Self-Propagation  
  Access to contacts enabled automatic spreading across networks  

---

## Impact

- Spread to thousands of users within hours  
- Affected Gmail users globally  
- Demonstrated a new phishing technique using trusted platforms  

---

## Detection and Response

- Google disabled the malicious app  
- Revoked permissions and warned users  
- Encouraged review of third-party app access  

---

## Key Lessons

- Phishing is evolving beyond password theft  
- Trust-based attacks are highly effective  
- Third-party app permissions are a major attack surface  

---

## Relevance to AI and Modern Phishing

- AI can increase the scale and realism of phishing attacks  
- Messages can be highly personalized  
- Detection requires more advanced, behavior-based methods  

---

## My Insight

This case highlights that effective phishing attacks exploit trust and platform features rather than technical vulnerabilities. As attacks become more advanced, especially with AI, detection must evolve beyond rule-based systems.
