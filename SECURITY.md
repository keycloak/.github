# Coordinated Vulnerability Disclosure

*This policy is based on the [CISA vulnerability disclosure policy template](https://www.cisa.gov/vulnerability-disclosure-policy-template)*

## Introduction

The Keycloak team believes that everyone, everywhere, is entitled to the access and quality information needed to mitigate security and privacy risks. We strive to protect communities of users, contributors, and partners from digital security threats. We believe an [open approach to vulnerability management](https://www.redhat.com/en/blog/red-hats-open-approach-vulnerability-management) is the best way to achieve this.

This policy supports our open approach and is intended to give security researchers clear guidelines for submitting and coordinating discovered vulnerabilities with us. In complying with this policy, you authorize CNCF to work with you to understand and resolve the issue quickly. For more details about our processes, please read the [security charter](SECURITY_CHARTER.md).

## Guidelines

* Research shared with any Keycloak representatives/individual will be reported to and managed by the Keycloak Security Response Team in order to be officially protected and coordinated.  
* Access and visibility to research and all CVE related data will follow the principle of least privilege by all vendors involved.  
* Establish and set a reasonable amount of time to resolve the issue before a vulnerability is disclosed publicly; agree and coordinate on public disclosure dates when possible.   
* Public disclosure should be prioritized on the need to keep company, government, and individual data confidential and the general public safe.  
* All vendors will honor disclosure/embargo requests in good faith as long as all guidelines are met.
* NDA signatures are not required.
* Vendors involved in coordinated disclosure will remain actively involved.

Violation of these guidelines may result in the individual, or vendor, being added to a denied coordination list.

## Scope

This policy applies to all Keycloak components and projects.  Research disclosed to the project will be limited to Response Team members; however, we will assist in coordinating the disclosure of research with upstream open-source communities as needed and requested.

## Reporting a suspected vulnerability

Suspected vulnerabilities should be disclosed responsibly and not made public until after analysis and a fix are available. We will acknowledge your report within 7 business days and work with you to confirm the vulnerability's existence and impact. Our goal is to maintain open dialogue during the assessment and remediation process.

To report a security vulnerability in the Keycloak codebase, send an email to [keycloak-security@googlegroups.com](mailto:keycloak-security@googlegroups.com). Please test against the **latest version** of Keycloak, include the affected version in your report, provide detailed instructions on how to reproduce the issue with a [minimal and reproducible example](https://stackoverflow.com/help/minimal-reproducible-example), and include your contact information for acknowledgements. If you are reporting known CVEs related to third-party libraries used in Keycloak, please [create a new GitHub issue](https://github.com/keycloak/keycloak/issues/new/choose).

If you would like to collaborate on a fix for the security vulnerability, please include your GitHub username in the email, and we will provide you access to a temporary private fork where we can work together.

If you discover any publicly disclosed security vulnerabilities, please notify us immediately through [keycloak-security@googlegroups.com](mailto:keycloak-security@googlegroups.com).

## Security Scanners

Reports from automated security scanners will **not** be accepted. These tools often report false positives, and can be disruptive to the project maintainers as it takes a long time to analyse these reports. If you believe you have found a security vulnerability using a security scanner, it is your responsiblity to provide a clear example of the vulnerability and how it could be exploited specifically for Keycloak as outlined above.

## Supported Versions

Depending on the severity of a vulnerability the issue may be fixed in the current `major.minor` release of Keycloak, or
for lower severity vulnerabilities or hardening in the following `major.minor` release. Refer to 
`https://www.keycloak.org/downloads` to find the latest release.

If you are unable to regularly upgrade Keycloak we encourage you to consider 
[Red Hat build of Keycloak](https://access.redhat.com/products/red-hat-build-of-keycloak/), which offers 
[long term support](https://access.redhat.com/support/policy/updates/jboss_notes#p_rhbk) of specific versions of Keycloak.
