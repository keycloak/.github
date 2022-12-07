# Security Policy

The Keycloak team takes security very seriously, and aim to resolve issues as quickly as possible. Building secure
software is a continuous process, and can always be improved. As such we welcome reports on potential security 
vulnerabilities, as well as suggestions around hardening the software and our process.

## Reporting a suspected vulnerability

It is important that suspected vulnerabilities be disclosed responsibly, and are not publicly disclosed until after they have been analyzed and a fix is available.

To report a security vulnerability, please create a [new GitHub advisory](https://github.com/keycloak-poc/keycloak/security/advisories/new.), or if you don't have a GitHub account, you can email the Keycloak team at [keycloak-security@googlegroups.com.](mailto:keycloak-security@googlegroups.com.) Please make sure to include the steps to reproduce the vulnerability, the affected version, and any additional files necessary.

When creating an advisory, you should have access to the temporary private fork, so we can collaborate on a fix without publicly disclosing the issue.

Do not open a public issue, send a pull request, or disclose any information about the suspected vulnerability publicly. If you discover any security vulnerabilities, please notify us immediately through [keycloak-security@googlegroups.com](mailto:keycloak-security@googlegroups.com).

## Public CVEs

For publicly known CVEs from third-party dependencies, we use [Trivy](https://github.com/aquasecurity/trivy) and [Snyk](https://snyk.io/). Trivy is a vulnerability scanning tool that checks container images, and Snyk keeps track of our project's dependencies.

We review the reports coming from Trivy and Snyk daily, below you can find the list of issues:

-   [Open Issues](https://github.com/keycloak/keycloak/issues?q=is%3Aissue+sort%3Aupdated-desc+label%3Akind%2Fcve+is%3Aopen)
-   [New fixes](https://github.com/keycloak/keycloak/pulls?q=is%3Apr+is%3Aopen+sort%3Aupdated-desc+label%3Akind%2Fcve)
-   [Closed issues](https://github.com/keycloak/keycloak/issues?q=is%3Aissue+sort%3Aupdated-desc+is%3Aclosed+label%3Akind%2Fcve)

Although we appreciate receiving reports from the community, it is not necessary to send scanner reports for public known CVEs to the keycloak-security mailing list. Instead, please create [a new GitHub issue](https://github.com/keycloak/keycloak/issues/new?assignees=&labels=kind%2Fbug%2Cstatus%2Ftriage&template=bug.yml) on GitHub.

## Supported Versions

Depending on the severity of a vulnerability the issue may be fixed in the current `major.minor` release of Keycloak, or
for lower severity vulnerabilities or hardening in the following `major.minor` release. Refer to 
`https://www.keycloak.org/downloads` to find the latest release.

If you are unable to regularly upgrade Keycloak we encourage you to consider 
[Red Hat Single Sign-On](https://access.redhat.com/products/red-hat-single-sign-on), which offers 
[long term support](https://access.redhat.com/support/policy/updates/jboss_notes#p_sso) of specific versions of Keycloak.
