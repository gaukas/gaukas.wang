---
title: Selected Projects
description: A list of selected projects that I am actively working on, have worked on, will be working on, and have completed.
---
This page lists some of my academic/personal projects that I recently have been working on.

## On-going

### [uTLS](https://github.com/refraction-networking/utls)
Fork of the Go standard TLS library, providing low-level access to the ClientHello for mimicry purposes.

uTLS is one of the most popular middlewares used in many TLS-based censorship circumvention tools.

### [clienthellod](https://github.com/gaukas/clienthellod)
A service that parses and resolves the ClientHello message sent by the client to the server. It is a part of the TLS fingerprintability research project which spans tlsfingerprint.io and quic.tlsfingerprint.io. It parses the ClientHello messages sent by TLS clients and QUIC Client Initial Packets sent by QUIC clients and display the parsed information in a human-readable format with high programmability.

See [tlsfingerprint.io](https://tlsfingerprint.io/) and [quic.tlsfingerprint.io](https://quic.tlsfingerprint.io/) for more details about the project.

## Archived/Completed

### [socks5](https://github.com/gaukas/socks5)
This package implements the SOCKS5 protocol as described in RFC1928 in Go with no external dependency. Unlike a traditional SOCKS5 server, this implementation separates the SOCKS5 server from the actual proxy server, which allows it to be used with any custom transport and/or in other applications.

### disc†
A safe communication protocol based on a decentralized network and provides message delivery with guaranteed integrity and confidentiality.

### [passthru](https://github.com/gaukas/passthru)
(De-)multiplexing TCP connections based on DPI-based Application Data sniffing.

## CVEs

### [CVE-2021-36539](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2021-36539)

Unbound file access vulnerabilities in Canvas LMS from Instructure, Inc. allow an attacker to access arbitrary files in a course it enrolled as a student(unprivileged user). The file does not need to be unlocked or even published.

### [CVE-2021-28681](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2021-28681)

Man-in-the-Middle (MITM) vulnerability in Pion WebRTC library during/before DTLS handshake allows an attacker to intercept and modify the DTLS stream by switching the DTLS certificate fingerprint since it is not being verified properly on each side.

† These projects are not publicly viewable due to unresolved authorship/copyright/license conflicts. 