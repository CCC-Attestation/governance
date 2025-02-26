# CCC Attestation Projects

This repo contains governance and other documents related to attestation
projects within the [Confidential Computing
Consortium](https://github.com/confidential-computing).


## Observation on the need for common standards

Attestation features found in current offerings in the Confidential Computing
space meaningfully improve security of confidential applications by offering
computing parties a way to verify specific properties of each other’s
workloads, lessening the need for blind trust that must be placed on the other
party. However, these solutions do not yet offer a standard way for customers
to declare, configure and authenticate attestation claims of a peer workload
that might be running in a peer TEE (e.g., Intel SGX, AMD SEV, Arm TrustZone,
etc. or other protected environment), and they may offer limited
framework-independent and platform-independent ways to accomplish Attestation
interoperability goals. Additionally, they do not have built-in support for web
services and application frameworks popular among the user community.

Therefore, it is of significant interest to the Confidential Computing
Consortium to explore how harmonisation and de-fragmentation can be achieved
(i.e., by producing interoperable implementations based on real-world use
cases).

# Scoping

This work focuses on the *interoperability* between different types of
Confidential environments, as well as between Confidential and non-Confidential
environments, and more specifically how existing authentication, authorization,
and identification flows can be enhanced with Attestation, and on new flows
created to leverage Attestation.

# Governance

* [Project Governance](governance.md)
* [Project Technical Charter](TECHNICAL_CHARTER.md)

# Community, discussions, and how to contribute

Most of our discussions take place on the [CCC
Slack](https://confidentialcomputing.slack.com/) in the
[#attestation](https://confidentialcomputing.slack.com/archives/C01QZ3K1APM)
channel.

Individual sub-projects are likely to have their own Slack channels as well.
We'll jot down a list here.

We will have [periodic meetings](https://confidentialcomputing.io/get-involved/calendar/) on [Zoom](https://zoom.us/j/99639347425?pwd=VGhEamJrVVhwaFZmMjFJTExoRlVFUT09), and will be
captured in [Google docs](https://docs.google.com/document/d/1NkiS78knPhDO0vA9ElS-bQOHNu783gGPdmTEbbOoOOU).

