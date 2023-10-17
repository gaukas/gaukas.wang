---
title: Selected Projects and Other Contributions
description: A list of selected projects of Gaukas Wang.
---
This page serves as an incomplete lists of the academic/personal projects I have been working on. Unless otherwise noted, I am the major or sole author of the listed projects. 

## TLS/QUIC Fingerprinting

### [clienthellod](https://github.com/gaukas/clienthellod)
A service that parses and resolves the ClientHello message sent by the client to the server. It is a part of the TLS fingerprintability research project which spans tlsfingerprint.io and quic.tlsfingerprint.io. It parses the ClientHello messages sent by TLS clients and QUIC Client Initial Packets sent by QUIC clients and display the parsed information in a human-readable format with high programmability.

See [tlsfingerprint.io](https://tlsfingerprint.io/) and [quic.tlsfingerprint.io](https://quic.tlsfingerprint.io/) for more details about the background and the motivation of this project.

### [uTLS](https://github.com/refraction-networking/utls) (maintainer)
Fork of the Go standard TLS library, providing low-level access to the ClientHello for mimicry purposes.

uTLS is one of the most popular middlewares used in many TLS-based censorship circumvention tools.

### [uQUIC](https://github.com/refraction-networking/uquic)
Fork of the quic-go QUIC library, providing low-level access to the Client Initial Packet for mimicry purposes.

### [TLSFingerprint.io](https://tlsfingerprint.io/) (maintainer)
A website that collects and displays TLS ClientHello fingerprints. It is a part of the TLS fingerprintability research project which spans tlsfingerprint.io and quic.tlsfingerprint.io.

### [QUIC.TLSFingerprint.io](https://quic.tlsfingerprint.io/) (maintainer)
A website that collects and displays QUIC Client Initial Packet fingerprints. It is a part of the TLS fingerprintability research project which spans tlsfingerprint.io and quic.tlsfingerprint.io.

## Building Better Transport 

### [W.A.T.E.R.](https://github.com/gaukas/water) - WebAssembly Transport Executables Runtime
A runtime environment for WebAssembly-based transport executables. It is a part of the [Refraction Networking](https://refraction.network/) project.

## Other Projects

### [socks5](https://github.com/gaukas/socks5)
This package implements the SOCKS5 protocol as described in RFC1928 in Go with no external dependency. Unlike a traditional SOCKS5 server, this implementation separates the SOCKS5 server from the actual proxy server, which allows it to be used with any custom transport and/or in other applications.

### disc†
A safe communication protocol based on a decentralized network and provides message delivery with guaranteed integrity and confidentiality.

### [passthru](https://github.com/gaukas/passthru)
(De-)multiplexing TCP connections based on DPI-based Application Data sniffing.

## CVE (Common Vulnerabilities and Exposures)

### [CVE-2021-36539](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2021-36539)

Unbound file access vulnerabilities in Canvas LMS from Instructure, Inc. allow an attacker to access arbitrary files in a course it enrolled as a student(unprivileged user). The file does not need to be unlocked or even published.

### [CVE-2021-28681](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2021-28681)

Man-in-the-Middle (MITM) vulnerability in Pion WebRTC library during/before DTLS handshake allows an attacker to intercept and modify the DTLS stream by switching the DTLS certificate fingerprint since it is not being verified properly on each side.

† These projects are not publicly viewable due to unsettled authorship/copyright/licensing issue. 