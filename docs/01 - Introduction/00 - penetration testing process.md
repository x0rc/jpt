# Penetration Testing Process

![[Pasted image 20220628184429.png]]


## Pre-Engagement
The first step is to create all the necessary documents in the pre-engagement phase, discuss the assessment objectives, and clarify any questions.

## Information Gathering

Once the pre-engagement activities are complete, we investigate the company's existing website we have been assigned to assess. We identify the technologies in use and learn how the web application functions.

## Vulnerability Assessment

With this information, we can look for known vulnerabilities and investigate questionable features that may allow for unintended actions.

## Post-Exploitation

Once we have successfully exploited the target, we jump into information gathering and examine the webserver from the inside. If we find sensitive information during this stage, we try to escalate our privileges (depending on the system and configurations).

## Lateral Movement

If other servers and hosts in the internal network are in scope, we then try to move through the network and access other hosts and servers using the information we have gathered.

## Proof-of-Concept

We create a proof-of-concept that proves that these vulnerabilities exist and potentially even automate the individual steps that trigger these vulnerabilities.

## Post-Engagement

Finally, the documentation is completed and presented to our client as a formal report deliverable. Afterward, we may hold a report walkthrough meeting to clarify anything about our testing or results and provide any needed support to personnel tasked with remediating our findings.

## Signing documents
There are 7 documents that needs to be prepared for a peneration test. 

| Document | Timing for Creation |
| ----------- | ------ |
| `1. Non-Disclosure Agreement` (`NDA`) | `After` Initial Contact |
| `2. Scoping Questionnaire` | `Before` the Pre-Engagement Meeting |
| `3. Scoping Document` | `During` the Pre-Engagement Meeting |
| `4. Penetration Testing Proposal` (`Contract/Scope of Work` (`SoW`)) | `During` the Pre-engagement Meeting |
| `5. Rules of Engagement` (`RoE`) | `Before` the Kick-Off Meeting |
| `6. Contractors Agreement` (Physical Assessments) | `Before` the Kick-Off Meeting |
| `7. Reports` | `During` and `after` the conducted Penetration Test |