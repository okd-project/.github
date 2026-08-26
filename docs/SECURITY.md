# Reporting a Security Vulnerability or Incident

Please do not report security vulnerabilities or security incidents via public channels (such as GitHub Issues, Pull Requests, or Discussions). To ensure coordinated disclosure, submit your findings via email to: `secalert@redhat.com`

## Submission Guidelines

To help us triage and resolve the issue efficiently, please include the following in your report:

- **Title**: A concise, descriptive summary of the issue.
- **Reporter Details**: Your name/handle and affiliation.
- **Technical Description**: Detailed information regarding the vulnerability.
- **Affected Versions**: The specific version(s) or range(s) of OKD tested.
- **Reproduction Steps**: A minimal, functional example to reproduce the issue.
- **Impact Assessment**: Potential exploit scenarios and perceived severity (optional).
- **Suggested Fix**: Any proposed patches or mitigations (optional).
- **Disclosure Status**: Whether this has been shared with other parties or published and your plan for future sharing (e.g., at a conference).

## Response Timeline

We aim to provide an initial acknowledgement of your report within 3 business days.

Our goal is to assess the report, coordinate fix and disclosure as quickly as possible. All confirmed security vulnerabilities and incidents will be addressed according to severity level and impact on the project.

## Contact Information

Direct all security questions and vulnerability reports to:

- **Email**: [secalert@redhat.com](mailto:secalert@redhat.com)

## Supported Versions

We regularly perform releases that contain fixes for relevant security vulnerabilities and important bugs. Prior releases might receive critical security fixes on a best-effort basis. However, we cannot guarantee that security fixes will get back-ported to unsupported versions.

- [OKD releases](https://amd64.origin.releases.ci.openshift.org/)
## Secure Development Practices

OKD uses OCP codebase, which follows established industry practices for secure development, including but not limited to:

- **Mandatory peer review**: All code changes require review and approval via the [OWNERS file (https://git.k8s.io/community/contributors/guide/owners.md) model enforced by Prow. PRs cannot merge without at least one `/lgtm` from a reviewer and one `/approve` from a listed approver.
- **CI-gated merges**: All pull requests must pass presubmit test jobs in [Prow](https://docs.prow.k8s.io/) before merging. CI job configuration is centralized in the [openshift/release](https://github.com/openshift/release) repository.
- **Immutable release payloads**: Each OKD release is a container image containing a manifest of pinned image digests (SHA256), not mutable tags. The Cluster Version Operator orchestrates upgrades exclusively from payload contents.
- **Image-based OS**: OKD runs on CentOS Stream CoreOS, an immutable, image-based operating system. OKD does not use RPM repositories at runtime.
- **Vendored dependencies**: Go modules with vendored dependencies provide reproducible builds. Changes to `go.mod`, `go.sum`, or `vendor/` directories are automatically labeled for dedicated review scrutiny.

## EU Cyber Resilience Act — Open Source Steward Statement

This project is stewarded by **Red Hat, Inc.**, an open source software steward as defined in Article 3(14) of the [EU Cyber Resilience Act (Regulation 2024/2847)](https://eur-lex.europa.eu/eli/reg/2024/2847/oj/eng).
Contact: [cra-steward@redhat.com](mailto:cra-steward@redhat.com)

For guidance on reporting actively exploited vulnerabilities and severe incidents under the CRA, see [Reporting Actively Exploited Vulnerabilities and Severe Incidents](https://github.com/RedHatProductSecurity/CRA/blob/main/Guidelines/eu-cra-incident-and-vulnerability-reporting-guidelines.md).

Refer to [Red Hat's security practices and vulnerability management policy](https://access.redhat.com/security/) for detailed information.
