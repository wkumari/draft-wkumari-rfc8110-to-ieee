---
title: "Transferring Opportunistic Wireless Encryption to the IEEE 802.11 Working Group"
abbrev: "RFC8110-to-IEEE"
category: info

docname: draft-wkumari-rfc8110-to-ieee-latest
submissiontype: IETF  # also: "independent", "editorial", "IAB", or "IRTF"
number:
date:
consensus: true
v: 3
updates: 8110
# area: AREA
# workgroup: WG Working Group
keyword:
 - IEEE
 - OWE
 - Opportunistic Wireless Encryption
 - RFC8110
venue:
#  group: WG
#  type: Working Group
#  mail: WG@example.com
#  arch: https://example.com/WG
  github: "wkumari/draft-wkumari-rfc8110-to-ieee"
  latest: "https://wkumari.github.io/draft-wkumari-rfc8110-to-ieee/draft-wkumari-rfc8110-to-ieee.html"

author:
  -
    name: "Warren Kumari"
    ins: "W. Kumari"
    organization: "Google, LLC"
    email: "warren@kumari.net"
  -
    name: "Dan Harkins"
    ins: "D. Harkins"
    organization: "Hewlett-Packard Enterprise"
    email: daniel.harkins@hpe.com

normative:
  RFC8110:

informative:
  RFC7435:
  Wi-Fi_Enhanced_Open:
    target: "https://www.wi-fi.org/beacon/dan-harkins/wi-fi-certified-enhanced-open-transparent-wi-fi-protections-without-complexity"
    title: "Wi-Fi CERTIFIED Enhanced Open™: Transparent Wi-Fi® protections without complexity"
  IEEE_802.11:
    target: https://www.ieee802.org/11/
    title: "IEEE 802.11 Working Group"
  IEEE_LS:
    target: https://datatracker.ietf.org/liaison/1929/
    title: "Liaison Statement from IEEE 802.11 to the IETF - OWE (RFC8110) now in 802.11"


--- abstract

RFC 8110 describes Opportunistic Wireless Encryption (OWE), a mode that allows
unauthenticated clients to connect to a network using encrypted traffic. This
document transfers the ongoing maintenance and further development of the protocol to the IEEE 802.11 Working Group.

This document updates RFC 8110 by noting that future work on the protocol described in RFC 8110 will occur in the IEEE 802.11 Working Group.

--- middle

# Introduction

{{RFC8110}} describes Opportunistic Wireless Encryption (OWE), a mode of
opportunistic security {{RFC7435}} for IEEE Std 802.11 that provides encryption
of the wireless medium without authentication.

Since publication, {{RFC8110}} (also known as "{{Wi-Fi Enhanced Open}}") has been widely implemented and deployed.


{{IEEE_802.11}} has requested {{IEEE_LS}} that in order to allow for ongoing maintenance and further development of the protocol, and to ensure that the protocol remains in sync with IEEE 802.11 protocols, future work on the protocol described in {{RFC8110}} will now occur in {{IEEE_802.11}}. This document is a concurrence.

# Transfer of Maintenance

At the request of {{IEEE_802.11}}, in order to allow for ongoing maintenance
and further development of the  protocol, and to ensure that the protocol
remains in sync with IEEE 802.11 protocols, this document specifies that future
work on the protocol described in RFC8110 will now occur in {{IEEE_802.11}}.

The protocol defined in {{RFC8110}} will be duplicated in {{IEEE_802.11}}
such that that document alone will be enough to implement it and any
further maintenance or modification of the protocol will be performed
in IEEE under its policies and procedures.

# Security Considerations

This document simply notes that future work on the protocol described in
{{RFC8110}} will now occur in the IEEE. As such, it does not introduce any new
security considerations.


# IANA Considerations

This document has no IANA actions.


--- back

# Acknowledgments
{:numbered="false"}

The authors would like to thank the IEEE 802.11 working group for their work,
and for taking on the responsibility for future work on the protocol
described in {{RFC8110}}.

In addition, we would like to thank Stephen Farrell, who AD sponsored the
original work, as well as Clemens Schimpe, Dorothy Stanley, Paul Wouters, Éric
Vyncke, Mike Montemurro, and Peter Yee.

Apologies to anyone we forgot to acknowledge; {{RFC8110}} was written 7+ years ago and we have had many conversations with many people since then...

# Change Log
{:numbered="false"}

* From -02 to -03:
  * Updated "the IEEE protocols" to Peter Yee's "IEEE 802.11 protocols".
  * Somehow many of the references to RFC8110 were not entered as references.
  * Fixed "RFC8110" -> "RFC 8110" in the abstract.
  * Fixed Éric Vyncke's name.

* From -01 to -02:
  * The Updates header contained 'RFC', removed it to make idnits happy.

* From -00 to -01:
  * Fixed a nit ("This documents updates" -> "This document updates")
  * We have the liaison from the IEEE 802.11 WG; update to point at the liaison
    statement.
  * For some reason, pushing the -01 version to GitHub didn't trigger the
    build. Trying to post manually.
