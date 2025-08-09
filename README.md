<h1>Cloud and Web Security   </h1>

<h2>Description</h2>
As a Security Consultant brought in to investigate a severe breach at an online banking website, I was tasked with identifying the reason for a web server attack that resulted in unauthorized access to: 

• Critical transaction logs, and 

• Customer account details 

Following the initial triage, it was clear that attackers had been successful in gaining administrative control of the web server by exploiting two systemic issues 

1. Outdated software running on the production environment, notably Drupal 7.5 (CVE-2018-7600), vulnerable to Drupalgeddon2 remote code execution exploit (Drupal Security Team, 2018; NIST, 2018). 

2. Misconfigured server components, including open directories and weak authentication controls lacking brute-force protection and input sanitization measures, as outlined in OWASP guidelines (OWASP Foundation, 2017) 

This is my report, threat model and risk analysis using STRIDE, and my implementation test that recreated the two most severe vulnerabilities — all conducted on a controlled TryHackMe environment emulated on the compromised system's setup. These simulations confirmed that inadequate patching and configuration hygiene permitted administrative control of the web server. The report outlines the risk footprint, provides mitigation strategies utilizing the NIST Cybersecurity Framework, and discusses the ethical and legal implications of such a breach within the financial sector.
<br />


<h2>Tools used in Investigation</h2>

- nmap (Nmap.org)
- searchsploit (Offensive Security)
- 44449.rb (Exploit-DB Drupalgeddon2)

<h2>Platform and Environments Used </h2>

- <b>Ubuntu Linux</b>
- <b>TryHackMe</b>

<img width="1099" height="839" alt="image" src="https://github.com/user-attachments/assets/70b603bf-33dc-4fd2-9484-fca2fecb9da1" />
<img width="1107" height="837" alt="image" src="https://github.com/user-attachments/assets/9dedd894-3e61-4216-adfc-6cd7bc6f948c" />
<img width="1104" height="832" alt="image" src="https://github.com/user-attachments/assets/192a1cc8-242a-435e-9697-ea4bdbafb6f5" />
<img width="1107" height="847" alt="image" src="https://github.com/user-attachments/assets/4880c208-4b19-4273-9972-809c390bde69" />
<img width="1107" height="842" alt="image" src="https://github.com/user-attachments/assets/52e14017-453e-4ae0-bced-b3061c326d2d" />
<img width="1105" height="841" alt="image" src="https://github.com/user-attachments/assets/a8dd452d-4395-4ace-a29b-e62f8383d2b1" />
<img width="1114" height="844" alt="image" src="https://github.com/user-attachments/assets/8435b8cf-a440-4936-b535-7b3f33a4bf88" />


