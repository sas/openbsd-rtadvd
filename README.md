patches for OpenBSD's rtadvd(8)
===============================

This repo contains a set of patches I made for OpenBSD's rtadvd(8) daemon.


## RFC 6106 patch

The first patch (located in patches/rtadvd-rfc6106.patch) brings support of
RDNSS and DNSSL to rtadvd(8). These options, added to the RA protocol by RFC
6106 allow ipv6 clients to get DNS configuration without using DHCP or DHCPv6.


## noifprefix patch

The second patch adds a flag to rtadvd.conf(5) to disable automatic prefix
gathering when no addr option is present for an interface.
