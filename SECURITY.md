# Security Policy

The Keycloak team takes security very seriously, and aim to resolve issues as quickly as possible. Building secure
software is a continuous process, and can always be improved. As such we welcome reports on potential security 
vulnerabilities, as well as suggestions around hardening the software and our process.

## Reporting a suspected vulnerability

It is important that suspected vulnerabilities are disclosed in a responsible way, and are not publicly disclosed until after they have been analysed and a fix is available.

To report a security vulnerability in the Keycloak codebase, send an email to keycloak-security@googlegroups.com. Please include the version affected, provide detailed instructions on how to reproduce the issue, and include your contact information for acknowledgements. If you are reporting known CVEs related to third-party libraries used in Keycloak, [please create a new GitHub issue](https://github.com/keycloak/keycloak/issues/new/choose).

If you would like to work with us on a fix for the security vulnerability, please include your GitHub username in the above email, and we will provide you access to a temporary private fork where we can collaborate on a fix without it being disclosed publicly.

Do not open a public issue, send a pull request, or disclose any information about the suspected vulnerability publicly. If you discover any publicly disclosed security vulnerabilities, please notify us immediately through keycloak-security@googlegroups.com.

## Supported Versions

Depending on the severity of a vulnerability the issue may be fixed in the current `major.minor` release of Keycloak, or
for lower severity vulnerabilities or hardening in the following `major.minor` release. Refer to 
`https://www.keycloak.org/downloads` to find the latest release.

If you are unable to regularly upgrade Keycloak we encourage you to consider 
[Red Hat Build of Keycloak](https://access.redhat.com/products/red-hat-build-of-keycloak/), which offers 
[long term support](https://access.redhat.com/support/policy/updates/jboss_notes#p_rhbk) of specific versions of Keycloak.
