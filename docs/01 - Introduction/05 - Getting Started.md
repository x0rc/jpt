# Getting started

- [Information security](https://en.wikipedia.org/wiki/Information_security) (infosec) is a vast field. The field has grown and evolved greatly in the last few years. It offers many specializations, including but not limited to:
	-   Network and infrastructure security
	-   Application security
	-   Security testing
	-   Systems auditing
	-   Business continuity planning
	-   Digital forensics
	-   Incident detection and response
	
	Data can be electronic or physical and tangible (e.g., design blueprints) or intangible (knowledge). A common phrase that will come up many times in our infosec career is protecting the "confidentiality, integrity, and availability of data," or the `CIA triad`.

- Risk Managment Process

| Step | Explanation |
| ---- | --- |
| `Identifying the Risk` | Identifying risks the business is exposed to, such as legal, environmental, market, regulatory, and other types of risks.|
| `Analyze the Risk` | Analyzing the risks to determine their impact and probability. The risks should be mapped to the organization's various policies, procedures, and business processes.|
| `Evaluate the Risk` | Evaluating, ranking, and prioritizing risks. Then, the organization must decide to accept (unavoidable), avoid (change plans), control (mitigate), or transfer risk (insure).|
| `Dealing with Risk` | Eliminating or containing the risks as best as possible. This is handled by interfacing directly with the stakeholders for the system or process that the risk is associated with. |
| `Monitoring Risk` | All risks must be constantly monitored. Risks should be constantly monitored for any situational changes that could change their impact score, `i.e., from low to medium or high impact`.|

- Red Team vs. Blue Team
In infosec, we usually hear the terms `red team` and `blue team`. In the simplest terms, the `red team` plays the attackers' role, while the `blue team` plays the defenders' part.

- Stay organized
	- Note taking tools:
		- [Cherrytree](https://www.giuspen.com/cherrytree)
		- [Visual Studio Code](https://code.visualstudio.com)
		- [Evernote](https://evernote.com)
		- [Sublime Text](https://www.sublimetext.com)
		- [GitBook](https://www.gitbook.com)
		- [Notion](https://www.notion.so)
		- [Notepad++](https://notepad-plus-plus.org/downloads)

- Common terms

| **Shell Type** | **Description** |
| --- | --- |
| `Reverse shell` | Initiates a connection back to a "listener" on our attack box. |
| `Bind shell` | "Binds" to a specific port on the target host and waits for a connection from our attack box. |
| `Web shell` | Runs operating system commands via the web browser, typically not interactive or semi-interactive. It can also be used to run single commands (i.e., leveraging a file upload vulnerability and uploading a `PHP` script to run a single command.|

[Reverse Shell - Payload All The Things](https://github.com/swisskyrepo/PayloadsAllTheThings/blob/master/Methodology%20and%20Resources/Reverse%20Shell%20Cheatsheet.md)

[Bind Shell Payload All The Things](https://github.com/swisskyrepo/PayloadsAllTheThings/blob/master/Methodology%20and%20Resources/Bind%20Shell%20Cheatsheet.md)

[Ports](https://web.mit.edu/rhel-doc/4/RH-DOCS/rhel-sg-en-4/ch-ports.html)
[Ports](https://packetlife.net/media/library/23/common-ports.pdf)
[Top 1000](https://nullsec.us/top-1-000-tcp-and-udp-ports-nmap-default/)

[OWASP Top 10](https://owasp.org/www-project-top-ten/). This is a standardized list of the top 10 web application vulnerabilities maintained by the Open Web Application Security Project (OWASP).This list is considered the top 10 most dangerous vulnerabilities and is not an exhaustive list of all possible web application vulnerabilities. Web application security assessment methodologies are often based around the OWASP top 10 as a starting point for the top categories of flaws that an assessor should be checking for. The current OWASP Top 10 list is:

| Number | Category | Description |
| --- | --- | --- |
| 1. | [Broken Access Control](https://owasp.org/Top10/A01_2021-Broken_Access_Control/) | Restrictions are not appropriately implemented to prevent users from accessing other users accounts, viewing sensitive data, accessing unauthorized functionality, modifying data, etc. |
| 2. | [Cryptographic Failures](https://owasp.org/Top10/A02_2021-Cryptographic_Failures/) | Failures related to cryptography which often leads to sensitive data exposure or system compromise. |
| 3. | [Injection](https://owasp.org/Top10/A03_2021-Injection/) | User-supplied data is not validated, filtered, or sanitized by the application. Some examples of injections are SQL injection, command injection, LDAP injection, etc.|
| 4. | [Insecure Design](https://owasp.org/Top10/A04_2021-Insecure_Design/) | These issues happen when the application is not designed with security in mind.|
| 5. | [Security Misconfiguration](https://owasp.org/Top10/A05_2021-Security_Misconfiguration/) | Missing appropriate security hardening across any part of the application stack, insecure default configurations, open cloud storage, verbose error messages which disclose too much information. |
| 6. | [Vulnerable and Outdated Components](https://owasp.org/Top10/A06_2021-Vulnerable_and_Outdated_Components/) | Using components (both client-side and server-side) that are vulnerable, unsupported, or out of date. |
| 7. | [Identification and Authentication Failures](https://owasp.org/Top10/A07_2021-Identification_and_Authentication_Failures/) | Authentication-related attacks that target user's identity, authentication, and session management. |
| 8. | [Software and Data Integrity Failures](https://owasp.org/Top10/A08_2021-Software_and_Data_Integrity_Failures/) | Software and data integrity failures relate to code and infrastructure that does not protect against integrity violations. An example of this is where an application relies upon plugins, libraries, or modules from untrusted sources, repositories, and content delivery networks (CDNs). |
| 9. | [Security Logging and Monitoring Failures](https://owasp.org/Top10/A09_2021-Security_Logging_and_Monitoring_Failures/) | This category is to help detect, escalate, and respond to active breaches. Without logging and monitoring, breaches cannot be detected.. |
| 10. | [Server-Side Request Forgery](https://owasp.org/Top10/A10_2021-Server-Side_Request_Forgery_%28SSRF%29/) | SSRF flaws occur whenever a web application is fetching a remote resource without validating the user-supplied URL. It allows an attacker to coerce the application to send a crafted request to an unexpected destination, even when protected by a firewall, VPN, or another type of network access control list (ACL).|

- Web Enumeration
	- [GoBuster](https://github.com/OJ/gobuster)
	- [ffuf](https://github.com/ffuf/ffuf) 
	- [HTTP status codes](https://en.wikipedia.org/wiki/List_of_HTTP_status_codes). 
	- [SecLists](https://github.com/danielmiessler/SecLists)
	- `Whatweb` is a handy tool and contains much functionality to automate web application enumeration across a network.
	- `robots.txt`
	- Source Code (`CTRL +U`)

- Public Exploits
	- [Exploit DB](https://www.exploit-db.com)
	- [Rapid7 DB](https://www.rapid7.com/db/)
	- [Vulnerability Lab](https://www.vulnerability-lab.com)
	- [searchsploit](https://github.com/offensive-security/exploitdb)


---

<details>
  <summary>T001</summary>
  
  ```
	 Target: 10.129.62.97

	1. Perform an Nmap scan of the target. What is the version of the service that is running on port 8080?
		- Apache Tomcat

	2. Perform an Nmap scan of the target and identify the non-default port that the telnet service running on.
		- 2323

	3. List the SMB shares available on the target host. Connect to the available share as the bob user. Once connected, access the folder called 'flag' and submit the contents of the flag.txt file.
		- dceece590f3284c3866305eb2473d099
  ```

</details>


<details>
  <summary>S001</summary>
  
  ```bash
	┌──(x0r㉿kreatur-der-nacht)-[~]
	└─$ nmap -sC -sV -p- 10.129.160.49 -oN 1.txt
	Starting Nmap 7.92 ( https://nmap.org ) at 2022-06-28 21:38 CEST
	...
	...
	┌──(x0r㉿kreatur-der-nacht)-[~]
	└─$ cat 1.txt | grep 8080
	8080/tcp open  http        Apache Tomcat

	┌──(x0r㉿kreatur-der-nacht)-[~]
	└─$ cat 1.txt | grep telnet
	2323/tcp open  telnet      Linux telnetd

	┌──(x0r㉿kreatur-der-nacht)-[~]
	└─$  smbclient -U bob \\\\10.129.62.104\\users
	Password for [WORKGROUP\bob]:
	Try "help" to get a list of possible commands.
	smb: \> ls
	  .                                   D        0  Fri Feb 26 00:06:52 2021
	  ..                                  D        0  Thu Feb 25 21:05:31 2021
	  flag                                D        0  Fri Feb 26 00:09:26 2021
	  bob                                 D        0  Thu Feb 25 22:42:23 2021

			4062912 blocks of size 1024. 944784 blocks available
	smb: \> cd flag
	smb: \flag\> ls
	  .                                   D        0  Fri Feb 26 00:09:26 2021
	  ..                                  D        0  Fri Feb 26 00:06:52 2021
	  flag.txt                            N       33  Fri Feb 26 00:09:26 2021

			4062912 blocks of size 1024. 944784 blocks available
	smb: \flag\> get flag.txt
	getting file \flag\flag.txt of size 33 as flag.txt (0.2 KiloBytes/sec) (average 0.2 KiloBytes/sec)
	smb: \flag\> exit

	┌──(x0r㉿kreatur-der-nacht)-[~]
	└─$ cat flag.txt           
	dceece590f3284c3866305eb2473d099
    }
  ```
</details>

---


<details>
  <summary>T002</summary>
  
  ```
	 Target: 206.189.25.173:32360

	1. Try running some of the web enumeration techniques you learned in this section on the server above, and use the info you get to get the flag.
		- HTB{w3b_3num3r4710n_r3v34l5_53cr375}

  ```

</details>

<details>
  <summary>S002</summary>
  
  ```
	navigate to /robots.txt
	![[Pasted image 20220628234958.png]]
	inspect the source code of the admin page
	![[Pasted image 20220628235049.png]]
	log in
	![[Pasted image 20220628235157.png]]
  ```

</details>