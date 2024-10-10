# Security Charter

## Mission

The Keycloak Security Taskforce is committed to enhancing the security of the Keycloak project through continuous improvement of documentation, code, and processes. Our core responsibilities include:

* Proactive triage: rapidly addressing security vulnerabilities reported to Keycloak and ensuring they are resolved promptly and consistently.  
* Impact evaluation: assessing the security implications of new and existing features.  
* Process enhancement: regularly reviewing and refining security processes to ensure ongoing improvement within the codebase.

## Teams

### Keycloak Security Response Team

A dedicated subset of maintainers actively involved in triaging new issues and coordinating with Resolution Teams. The Response Team has full access to all CVEs reported to the project and can add or remove members from Resolution Teams as necessary.

Member Nomination Process

* New members can be nominated by existing maintainers and members of the Keycloak Security Response Team. Members of both teams have a vote in the approval process, and a 2/3 majority is required for approval.  
* All nominations must be sent to the Keycloak Security mailing list.  
* Members may step down at any time and may nominate a replacement when they do.

Responsibilities

* Remain active and responsive, participating in day-to-day activities.  
* Communicate any leave of absence.  
* Participate on rotating shifts on weekly basis  
* Members that have been inactive or not filling their responsibilities for more than three months without in advance notice will be removed by vote.

#### Scope

* Vulnerability triage: managing reports received via the Keycloak security mailing list.  
* Coordination: overseeing the response to reported vulnerabilities to ensure compliance with SLA deadlines.  
* Process improvement: maintaining and enhancing security measures, such as implementing linters, scanners, fuzzers, and patch managers. Ensuring security is proactively integrated throughout the project.

#### Rotating shifts

* Team members take turns being the primary point of contact on a weekly basis.  
* The designated person on the shift handles incoming security requests, coordinates responses to incidents, and manages day-to-day security tasks during their shift.   
* Other team members will continue to work on security response duties, supporting the person on the shift.  
* The Keycloak Security Office weekly meeting hours determine the end of the shift, and the next person on the shift is updated about the status.  
* Vacations and PTOs are communicated during the meeting so we can adjust the shift.

### Keycloak Security Resolution Team

Dynamic teams formed by individuals actively involved in triaging or resolving open CVEs. Members are added when they engage with a vulnerability and removed once their involvement concludes.

### Scope

* Resolution and testing: ensuring vulnerabilities are effectively fixed and thoroughly tested.  
* Collaboration:  working with the Response team to prioritize fixes above all other items in the team's backlog, regardless of their nature.  
* Release Coordination: collaborating closely with release coordinators and Quality Engineering (QE) teams to include patches in upcoming releases.

## Access

| Resource | Response Team | Resolution team |
| :---- | :---- | :---- |
| [Mailing list](https://groups.google.com/g/keycloak-security) | Full access | Added in CC to specific threads |
| [Private GitHub repository](https://github.com/keycloak/keycloak-private/) | Full access | Temporary access |
| [Security advisories and alerts](https://github.com/keycloak/keycloak/security) | Full access | No access |
| Slack channel (\#alerts-keycloak-cve) | Full access | Temporary access |

## Coordinating a Security Vulnerability Fix

* Identification: the Response Team identifies relevant engineers from affected areas and temporarily includes them in private communication channels (e.g., repositories, email threads), forming a temporary Resolution Team.  
* Efficiency: to prevent accidental disclosure, the Resolution Team remains as small as necessary.  
* Autonomy: the Resolution Team has the autonomy to involve additional parties such as release coordinators, QE, and documentation teams. Communication with the Response Team is advised when in doubt.  
* Access Revocation: post-release, access to sensitive communication channels is revoked to uphold the principle of least privilege.

## Process Overview

1. A new vulnerability is reported to the Keycloak security mailing list.  
2. The vulnerability report is triaged.
3. A CVE ID is assigned.  
4. The Response Team identifies the responsible group (e.g., Team A with members Noah and Emma).  
5. Team A submits the fix to the private repository and includes domain experts for review.  
6. Team A informs QE and releases coordinators about the forthcoming patch.  
7. The pull request is merged, and a new release is issued along with official advisories.

In the absence of CVEs to fix, all team members will have their access revoked to security sensitive channels except for the Keycloak Security Response Team. 

This charter outlines the approach the Keycloak project takes to manage and mitigate security vulnerabilities, ensuring the integrity and reliability of the project for all users.
