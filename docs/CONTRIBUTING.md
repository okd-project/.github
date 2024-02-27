Contributing to OKD
===

<!--- cSpell:ignore virt -->

OKD is built from many different open source projects - Fedora CoreOS, the CentOS Stream and UBI RPM ecosystems, cri-o, Kubernetes, and many different extensions to Kubernetes. The `openshift` organization on GitHub holds active development of components on top of Kubernetes and references projects built elsewhere. Generally, you'll want to find the component that interests you and review their README.md for the processes for contributing.

Community process and questions can be raised in our [community repo](https://github.com/openshift/community) and issues [opened in this repository](https://github.com/okd-project/okd/issues) (Bugzilla locations coming soon).

Our unified continuous integration system tests pull requests to the ecosystem and core images, then builds and promotes them after merge. To see the latest development releases of OKD visit [our continuous release page](https://amd64.origin.releases.ci.openshift.org/). These releases are built continuously and expire after a few days. Long lived versions are pinned and then listed on our [stable release page](https://github.com/okd-project/okd/releases).

All contributions are welcome - OKD uses the Apache 2 license and does not require any contributor agreement to submit patches.  Please open issues for any bugs or problems you encounter, ask questions in the [OKD discussion forum](https://github.com/okd-project/okd/discussions){: target=_blank}, or get involved in the [Kubernetes project](https://github.com/kubernetes/kubernetes) at the container runtime layer.

## Becoming a contributor

The easiest way to get involved in the community is to:

- watch [replays of previous working group meetings](https://www.youtube.com/playlist?list=PLaR6Rq6Z4Iqc3WjZB-rUTPru8RKyOCnBo)
- attend [one of the working group meetings](https://calendar.fedoraproject.org/list/okd/) (no invite needed, just use the link in the calendar to join the Zoom video conference).
- join the [OKD Working Group Google Group](https://groups.google.com/g/okd-wg)
- join the [Kubernetes Slack](https://slack.k8s.io/) channel [#okd-dev](https://kubernetes.slack.com/archives/C06FF6342RG)
- join the [Matrix room](https://matrix.to/#/#okd:fedoraproject.org)

The OKD project has a [charter](GOVERNANCE.md#okd-working-group-charter), setting out how the project is run.

## Working Groups

The project is managed by a bi-weekly working group video call:

The [main working group](GOVERNANCE.md) is where are the major project decisions are made, but when a specific work item needs to be completed a sub-group may be formed, so a focussed set of volunteers can work on a specific area.