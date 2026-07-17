---
unit: FIT1047
type: MOC
tags: [Monash/CS_DS, CS/Systems]
---
# 📘 FIT1047: Introduction to Computer Systems, Networks and Security

> [!INFO] Map of Content
> Index for **FIT1047 (Malaysia campus)**. Hand-execution unit: number conversions, logic circuits, MARIE assembly traces are the assessed skills — every applied note carries a write-from-blank element. No code toolkit ⟹ no Tier 3C cheatsheet; the conversion procedures ARE the toolkit.

## 📊 Assessment Map (from Week 1 workshop — verify remainder against unit guide)
- **Assignment 1 (15%)** ➔ Foundations: Binary Number System (W1) + Boolean Logic Circuit (W2).
- **Assignment 2 (25%)** ➔ Programming Interview: Assembly Programming (W3–4), Computer Architecture (W3–4), Motherboard & Boot (W5), OS (W5).
- **Remaining weight** ➔ networks + security half (LO5–7) and final assessment *(⚠ split not stated in W1 deck)*.
- **LO1 (W1–2):** number representations + Boolean algebra → logic circuits · **LO2:** hardware/software architectures · **LO3:** MARIE assembly · **LO4:** OS functions.

## 🧰 Unit Cheatsheet (pinned — SWOTVAC single re-read)

- 📌 [[FIT1047 Unit Cheatsheet]] — whole-unit exam crib — systems → networks → security in one re-read

## 📅 Knowledge Index

### Week 1 — Data Representation (Foundations of Computing)
- [[Computer Fundamentals (Bits, Bytes, Words)]] -> Parent Framework: [[FIT1047_MOC]]
- [[Number Systems (Binary and Hexadecimal)]] -> Parent Framework: [[Computer Fundamentals (Bits, Bytes, Words)]]
- [[Signed Integer Representation (Two's Complement)]] -> Parent Framework: [[Number Systems (Binary and Hexadecimal)]]
- [[Floating Point Numbers (IEEE 754)]] -> Parent Framework: [[Number Systems (Binary and Hexadecimal)]]
- [[Text Encoding (ASCII and Unicode)]] -> Parent Framework: [[Computer Fundamentals (Bits, Bytes, Words)]]
- [[Transistors and Logic Gates]] -> Parent Framework: [[Computer Fundamentals (Bits, Bytes, Words)]]

### Week 2 — Boolean Logic & Circuits
- [[Boolean Algebra Laws]] -> Parent Framework: [[Logical Connectives]] *(Smart Merged: FIT1058 logic + FIT1047 circuit notation, precedence, why-simplify)*
- [[Sum-of-Products (Functions to Circuits)]] -> Parent Framework: [[Boolean Algebra Laws]]
- [[Karnaugh Maps]] -> Parent Framework: [[Sum-of-Products (Functions to Circuits)]]
- [[Transistors and Logic Gates]] -> Parent Framework: [[Computer Fundamentals (Bits, Bytes, Words)]] *(extended in Week 2: NAND + universal gates)*

### Week 3 — Circuits with Memory, Architecture & MARIE
- [[Combinational Circuits (Adders, Decoders, MUX, ALU)]] -> Parent Framework: [[Transistors and Logic Gates]]
- [[Sequential Circuits (Latches, Flip-Flops, Registers)]] -> Parent Framework: [[Combinational Circuits (Adders, Decoders, MUX, ALU)]]
- [[Von Neumann Architecture and Programs]] -> Parent Framework: [[Computer Fundamentals (Bits, Bytes, Words)]]
- [[Fetch-Decode-Execute and RTL (Control)]] -> Parent Framework: [[Von Neumann Architecture and Programs]]
- [[MARIE Assembly (Instruction Set and Patterns)]] -> Parent Framework: [[Von Neumann Architecture and Programs]]

### Week 4 — Indirect Addressing, Subroutines & Memory
- [[MARIE Assembly (Instruction Set and Patterns)]] -> Parent Framework: [[Von Neumann Architecture and Programs]] *(extended in Week 4: LoadI/StoreI/AddI/JnS/JumpI + Adr/HEX directives)*
- [[MARIE Patterns (Indirect Addressing, Arrays, Subroutines)]] -> Parent Framework: [[MARIE Assembly (Instruction Set and Patterns)]]
- [[Memory and the Memory Hierarchy]] -> Parent Framework: [[Von Neumann Architecture and Programs]]

### Week 5 — Motherboard, I/O, Boot & Operating Systems (A2 material complete)
- [[Motherboard and IO Interfaces]] -> Parent Framework: [[Von Neumann Architecture and Programs]]
- [[CPU-IO Communication (Memory-Mapped, Polling, Interrupts, DMA)]] -> Parent Framework: [[Motherboard and IO Interfaces]]
- [[The Boot Process]] -> Parent Framework: [[Motherboard and IO Interfaces]]
- [[Operating Systems and Multi-Processing]] -> Parent Framework: [[Von Neumann Architecture and Programs]]
- [[Virtual Memory (MMU and Paging)]] -> Parent Framework: [[Operating Systems and Multi-Processing]]

### Week 6 — Networks I: Layers & Application Protocols (LO5–6 begin)
- [[Computer Networks (Components and Types)]] -> Parent Framework: [[FIT1047_MOC]]
- [[Internet Model (Layers, Protocols, Encapsulation)]] -> Parent Framework: [[Computer Networks (Components and Types)]]
- [[Application Architectures (Client-Server Tiers)]] -> Parent Framework: [[Computer Networks (Components and Types)]]
- [[World Wide Web (HTTP and HTML)]] -> Parent Framework: [[Internet Model (Layers, Protocols, Encapsulation)]]
- [[Electronic Mail (SMTP, POP, IMAP, MIME)]] -> Parent Framework: [[Internet Model (Layers, Protocols, Encapsulation)]]

### Week 7 — Networks II: The Four Lower Layers & Addressing
- [[Physical and Data Link Layers (Signals, Ethernet, CSMA-CD)]] -> Parent Framework: [[Internet Model (Layers, Protocols, Encapsulation)]]
- [[Network Addresses (URL, Port, IP, MAC)]] -> Parent Framework: [[Internet Model (Layers, Protocols, Encapsulation)]]
- [[Address Resolution (DNS and ARP)]] -> Parent Framework: [[Network Addresses (URL, Port, IP, MAC)]]
- [[Network Layer (Routing and Routing Tables)]] -> Parent Framework: [[Internet Model (Layers, Protocols, Encapsulation)]]
- [[Transport Layer (TCP and UDP)]] -> Parent Framework: [[Internet Model (Layers, Protocols, Encapsulation)]]

### Week 8 — Networks III: Switched Ethernet, WiFi & Organisational Networks
- [[Switched Ethernet (Switches, Forwarding, LAN Design)]] -> Parent Framework: [[Physical and Data Link Layers (Signals, Ethernet, CSMA-CD)]]
- [[WiFi (802.11, CSMA-CA, Topologies)]] -> Parent Framework: [[Physical and Data Link Layers (Signals, Ethernet, CSMA-CD)]]
- [[WiFi Security (WEP, WPA2)]] -> Parent Framework: [[WiFi (802.11, CSMA-CA, Topologies)]] *(seeds the security half)*
- [[LAN, Backbone, MAN, WAN (Organisational Networks)]] -> Parent Framework: [[Computer Networks (Components and Types)]]

### Week 9 — The Internet: Structure, Access, Delivery & Society
- [[Internet Structure and Governance]] -> Parent Framework: [[Computer Networks (Components and Types)]]  *(AS, BGP, IXP, peering/transit, governance)*
- [[Internet Access Technologies]] -> Parent Framework: [[Internet Structure and Governance]]
- [[CDNs, Load Balancing and Caching]] -> Parent Framework: [[Internet Structure and Governance]]
- [[Internet of Things (IoT)]] -> Parent Framework: [[Internet Structure and Governance]]
- [[Net Neutrality and Internet Policy]] -> Parent Framework: [[Internet Structure and Governance]]
- *(Week 7 recap in the workshop — line-coding/modulation — is already covered by [[Physical and Data Link Layers (Signals, Ethernet, CSMA-CD)]]; interior routing (RIP/OSPF) by [[Network Layer (Routing and Routing Tables)]].)*

### Week 10 — Security I: Cryptography & Secure-Channel Protocols (LO7)
- [[Information Security and Cryptography]] -> Parent Framework: [[FIT1047_MOC]]  *(hub: security goals + three algorithm families)*
- [[Symmetric Cryptography]] -> Parent Framework: [[Information Security and Cryptography]]
- [[Public Key Cryptography]] -> Parent Framework: [[Information Security and Cryptography]]
- [[Cryptographic Hash Functions]] -> Parent Framework: [[Information Security and Cryptography]]
- [[Key Establishment and Diffie-Hellman]] -> Parent Framework: [[Information Security and Cryptography]]
- [[Authentication, Certificates and PKI]] -> Parent Framework: [[Information Security and Cryptography]]
- [[Secure Channels - TLS and VPNs]] -> Parent Framework: [[Information Security and Cryptography]]
- *(Cross-links to FIT1058 number theory: [[Diffie-Hellman Key Agreement]], [[Cryptosystem]], [[One-Way Function]], [[Modular Exponentiation]], [[Euler Totient Function]], [[Prime Number]], [[Primitive Root]] — the maths behind RSA/DH lives there, not duplicated here.)*

### Week 11 — Security II: Authentication, Access Control & Network Defence (LO7)
- [[User Authentication and Passwords]] -> Parent Framework: [[Information Security and Cryptography]]
- [[Multi-Factor Authentication and Biometrics]] -> Parent Framework: [[User Authentication and Passwords]]
- [[Access Control]] -> Parent Framework: [[Information Security and Cryptography]]
- [[Firewalls and Packet Filtering]] -> Parent Framework: [[Information Security and Cryptography]]
- [[IDS, IPS and Next-Generation Firewalls]] -> Parent Framework: [[Firewalls and Packet Filtering]]
- *(Cross-links: salted-hash storage → [[Cryptographic Hash Functions]]; login in kernel mode → [[Operating Systems and Multi-Processing]]; NGF TLS-proxy breaks end-to-end → [[Secure Channels - TLS and VPNs]].)*

### Week 12 — Security III: Threats, Vulnerabilities, Risk & Privacy (LO7)
- [[Malware and Attack Types]] -> Parent Framework: [[Information Security and Cryptography]]
- [[Software Vulnerabilities (Injection, XSS, Buffer Overflow)]] -> Parent Framework: [[Information Security and Cryptography]]
- [[Cybersecurity Case Studies]] -> Parent Framework: [[Information Security and Cryptography]]
- [[Cybersecurity Risk Management]] -> Parent Framework: [[Information Security and Cryptography]]
- [[Privacy and Data Protection (FIT1047)]] -> Parent Framework: [[Information Security and Cryptography]]
- *(Cross-links: botnet/DDoS → [[Internet of Things (IoT)]]; buffer overflow return address → [[MARIE Patterns (Indirect Addressing, Arrays, Subroutines)]]; SQL injection → [[SQL SELECT and WHERE]]; privacy → [[Privacy, Confidentiality, and Security]], [[Personal Data and Privacy in Database Design]].)*

## 🧭 Suggested Reading Order
1. [[Computer Fundamentals (Bits, Bytes, Words)]] — why digital computers reduce everything to bits; bit → byte → word; CPU/RAM/I/O; stored programs.
2. [[Number Systems (Binary and Hexadecimal)]] — positional notation, binary↔decimal↔hex conversion drills, binary addition. **The A1 hand skill.**
3. [[Signed Integer Representation (Two's Complement)]] — sign-magnitude → 1's → 2's complement; negation recipe; overflow detection rules.
4. [[Floating Point Numbers (IEEE 754)]] — binary scientific notation, significand/exponent/sign, normalisation, rounding hazards.
5. [[Text Encoding (ASCII and Unicode)]] — ASCII 7-bit, extended sets, Unicode codepoints, UTF-8/UTF-16.
6. [[Transistors and Logic Gates]] — switches → transistors → NOT/OR/AND gates; the bridge into Week 2 Boolean algebra.

7. [[Boolean Algebra Laws]] — circuit notation ($XY$, $X{+}Y$, $\overline{X}$), precedence, the laws, and why simpler expressions mean cheaper/faster circuits.
8. [[Sum-of-Products (Functions to Circuits)]] — truth table → minterm products → OR → mechanical circuit construction.
9. [[Karnaugh Maps]] — Gray-code grid, the seven grouping rules, read-off; **the A1 simplification skill** (raw 5-term SOP → $Y + X\overline{Z}$).
10. [[Transistors and Logic Gates]] §Universality — NAND alone builds everything.

11. [[Combinational Circuits (Adders, Decoders, MUX, ALU)]] — half/full adders, ripple-carry, decoder vs MUX, the parallel-ops-plus-MUX ALU.
12. [[Sequential Circuits (Latches, Flip-Flops, Registers)]] — feedback = memory; SR latch table (forbidden $11$), D flip-flop, MARIE's PC/IR/MAR/MBR/AC.
13. [[Von Neumann Architecture and Programs]] — CPU+memory+I/O, stored programs, machine code → ISA → assembly → compiler/interpreter.
14. [[Fetch-Decode-Execute and RTL (Control)]] — the clock, RTL steps, the 7-cycle `Add X` trace. **The A2 trace skill.**
15. [[MARIE Assembly (Instruction Set and Patterns)]] — machine model, the 9-instruction W3 ISA, hand-assembly, SkipCond+Jump idioms. **The A2 writing skill.**

16. [[MARIE Patterns (Indirect Addressing, Arrays, Subroutines)]] — pointer walks, counter vs sentinel loops, JnS/JumpI calling convention. **The A2 core.**
17. [[Memory and the Memory Hierarchy]] — byte/word addressability, the 8 KiB MARIE calculation, cache behaviour, the speed/size table.

18. [[Motherboard and IO Interfaces]] — the physical board, interface trade-offs.
19. [[CPU-IO Communication (Memory-Mapped, Polling, Interrupts, DMA)]] — WHERE (mapped vs ports) and WHEN (poll/interrupt/DMA) the CPU talks to devices.
20. [[The Boot Process]] — the 12-step ROM→POST→boot-sector→kernel→GUI chain; BIOS vs UEFI. **A2 topic.**
21. [[Operating Systems and Multi-Processing]] — kernel's three managements, timesharing, Running/Ready/Blocked trace, user/kernel mode, system calls. **A2 topic + LO4.**
22. [[Virtual Memory (MMU and Paging)]] — per-process address spaces, MMU translation, page faults, swapping.

23. [[Computer Networks (Components and Types)]] — client/server/switch/router, LAN→WAN ladder, the bits-vs-bytes transfer-time drill.
24. [[Internet Model (Layers, Protocols, Encapsulation)]] — the five layers + PDU table; protocol (horizontal) vs interface (vertical). **The networks-half framework.**
25. [[Application Architectures (Client-Server Tiers)]] — four functions, six splits, one matrix.
26. [[World Wide Web (HTTP and HTML)]] — raw HTTP session anatomy, methods, one-page-many-requests.
27. [[Electronic Mail (SMTP, POP, IMAP, MIME)]] — the verbatim SMTP dialogue, push-vs-pull, envelope-vs-header, MIME.

28. [[Physical and Data Link Layers (Signals, Ethernet, CSMA-CD)]] — encodings/modulation, Ethernet, CSMA/CD's three parts, hub's physical-star-logical-bus trap.
29. [[Network Addresses (URL, Port, IP, MAC)]] — the one-address-per-layer table, /26 subnet arithmetic, IPv6 hierarchy, client/server port convention.
30. [[Address Resolution (DNS and ARP)]] — name→IP (iterative vs recursive) and IP→MAC (broadcast); the two-resolution page-load trace.
31. [[Network Layer (Routing and Routing Tables)]] — per-hop table lookup, default gateway, distance vector (RIP) vs link state (OSPF).
32. [[Transport Layer (TCP and UDP)]] — seq/ack arithmetic, 3-way open, 4-way close, the numbered lecture session, TCP vs UDP.

33. [[Switched Ethernet (Switches, Forwarding, LAN Design)]] — forwarding-table learning, flood-when-unknown, store-and-forward, switch vs router, bottleneck fixes.
34. [[WiFi (802.11, CSMA-CA, Topologies)]] — CSMA/CA + hidden node, the 1/6/11 channel puzzle, BSS→ESS, never-server-on-WiFi.
35. [[WiFi Security (WEP, WPA2)]] — open-WiFi capture, WEP's static-key flaw, WPA2 PSK vs Enterprise.
36. [[LAN, Backbone, MAN, WAN (Organisational Networks)]] — access/distribution/core, dedicated vs packet-switched vs VPN.

37. [[Internet Structure and Governance]] — the network-of-networks: Autonomous Systems + border routers + **BGP** (exterior) vs interior routing, IXPs, **peering vs transit**, Tier 1/2/3, RIR/APNIC, and the many governance bodies (ISOC/IETF, ICANN, ITU) — no single owner.
38. [[Internet Access Technologies]] — the last mile: ISP authenticate→assign-IP→give router/DNS; dial-up, **ADSL** (asymmetric, DSLAM, VDSL/FTTN), **NBN** (GPON, FTTP/FTTN/wireless/satellite, RSP/wholesale), and **4G/5G** mobile data.
39. [[CDNs, Load Balancing and Caching]] — why the Internet still works at scale: DNS/hardware **load balancing**, HTTP **content caching** (GET + `Expires`), and **CDNs** (points of presence near users, peering at IXPs).
40. [[Internet of Things (IoT)]] — device-to-device at billions-scale; enablers (cheap chips, IPv6, low-power wireless); the security problem ("S in IoT") and the **Mirai/Dyn** DDoS.
41. [[Net Neutrality and Internet Policy]] — treat-all-traffic-equally vs legitimate exceptions; apps vs open standards; platform vs public utility (natural monopoly); online law-enforcement challenges.

42. [[Information Security and Cryptography]] — the security-goal framework (confidentiality/integrity/authenticity/non-repudiation) and the three algorithm families; **match goal to mechanism** is the exam spine.
43. [[Symmetric Cryptography]] — shared key, S-boxes + permutations → AES/Rijndael, block chaining + CBC-MAC (WPA2), and the three disadvantages (key distribution, $O(n^2)$ scaling, no non-repudiation).
44. [[Public Key Cryptography]] — asymmetric key pairs; encryption / signatures / key-establishment; RSA operations + key generation; recommended AES vs RSA key lengths.
45. [[Cryptographic Hash Functions]] — one-way fixed-length digests, ideal properties (pre-image/avalanche/collision), MD5→SHA-256, and the **MAC-not-bare-hash** integrity rule.
46. [[Key Establishment and Diffie-Hellman]] — agree a secret over open comms; paint analogy + the $g{=}5, n{=}47 \to 15$ worked exchange; discrete-log security; the authentication gap.
47. [[Authentication, Certificates and PKI]] — closing the DH man-in-the-middle gap: CA-signed certificates, their contents, revocation (CRL/OCSP), and "a certificate ≠ a safe server".
48. [[Secure Channels - TLS and VPNs]] — TLS security layer (HTTPS, handshake/record/alert, SSL→TLS 1.3, DH-based key) and VPN tunnels (logical relocation, IPSec/OpenVPN/WireGuard, endpoint-only security).

49. [[User Authentication and Passwords]] — the three factor types (know/have/are), password problems, and safe storage (cleartext ❌ → hash → rainbow tables → **salted hash** ✅).
50. [[Multi-Factor Authentication and Biometrics]] — biometrics/hardware-token/authenticator-app trade-offs, MFA (combine factors), transaction authentication (TANs, SMS-TAN + SIM swap).
51. [[Access Control]] — access rights, ACL scaling wall ($1000{\times}200{=}2$M), ticket/token control (Kerberos/AD), SSO's single point of failure, privilege escalation + circumvention.
52. [[Firewalls and Packet Filtering]] — the filter-not-block barrier, packet-filtering fields (IP/port/protocol/state), inside-out-allow default, and the stateless/app-layer/internal-attacker limits.
53. [[IDS, IPS and Next-Generation Firewalls]] — IDS (detect/alert/log) vs IPS (+block), signature vs anomaly detection, and NGFs (app-aware, but TLS-proxy breaks end-to-end security).

54. [[Malware and Attack Types]] — phishing/ransomware/social-engineering/botnets/DoS, the virus-vs-worm-vs-trojan taxonomy, and why "careful people are safe" and anti-virus are both false comfort.
55. [[Software Vulnerabilities (Injection, XSS, Buffer Overflow)]] — the four classic weaknesses and their shared root cause (unchecked input + excess privilege); the `;rm -rf /` command-injection demo.
56. [[Cybersecurity Case Studies]] — F5 BIG-IP, Stuxnet, the Turkey pipeline, Bangladesh Bank SWIFT; the exposure-and-defaults lesson ("the main weapon was a keyboard").
57. [[Cybersecurity Risk Management]] — perfect security is impossible → manage residual risk with the NIST RMF control families; the NICE framework's 52 roles.
58. [[Privacy and Data Protection (FIT1047)]] — big-data profiling, "you are the product", PETs vs compliance-theatre cookie banners, and how data minimisation serves both privacy and security.

## 🎯 Learning Outcomes

After Week 1 you should be able to: explain why computers are digital, stored-program machines built from CPU/RAM/I/O and why all data reduces to bits (bytes, words); convert numbers between decimal, binary and hexadecimal in every direction and add binary numbers by hand; represent signed integers in sign-and-magnitude, 1's and 2's complement, negate via flip-and-add-one, state the 2's-complement range and detect overflow from sign patterns; explain binary scientific notation ($s \times 2^e$), normalise a value into significand + exponent, and reason about floating-point rounding error (why $0.1$ is inexact and why money needs integers); encode/decode text via ASCII (hex ↔ characters) and explain Unicode codepoints, UTF-8's 1–4-byte ASCII-compatible scheme vs UTF-16; and trace the hardware story from electronic switch → vacuum tube → transistor → gate (NOT/OR/AND truth behaviour) → integrated circuit, including Moore's law.

After Week 2 you should be able to: evaluate Boolean expressions and build truth tables (operator precedence NOT > AND > OR, circuit notation $XY$, $X{+}Y$, $\overline{X}$); state and apply the Boolean algebra laws (identity, null, idempotent, inverse, absorption, commutative, associative, distributive, De Morgan) to prove equivalence and simplify expressions, explaining why simplification matters for hardware cost; extract a sum-of-products expression from any truth table and convert it mechanically into a gate circuit; minimise a function with a Karnaugh map — Gray-code layout, maximal power-of-2 rectangular groups with overlap and wrap-around, read-off of the minimal SOP; and explain gate universality — NOT+AND or NOT+OR suffice, and NAND (or NOR) alone is functionally complete.

After Week 3 you should be able to: build and explain adders (half: XOR+AND; full: +carry-in; ripple-carry chains), decoders (1-of-$2^n$), multiplexers, and the ALU's compute-all-then-MUX-select design; explain how feedback turns combinational logic into memory — SR latch behaviour incl. the forbidden state, D flip-flops, registers and register files, and MARIE's five key registers; describe the Von Neumann architecture and the stored-program concept, distinguishing machine code, ISA, assembly (1-to-1 mnemonics), compilers and interpreters; hand-trace the fetch-decode-execute cycle in RTL, knowing fetch's fixed four steps, the variable decode steps, and per-step control signals; and hand-assemble and write small MARIE programs with the Week 3 instruction set (Load/Store/Add/Subt/Input/Output/Halt/SkipCond/Jump), using SkipCond+Jump to build conditionals and loops.

After Week 4 you should be able to: explain direct vs indirect addressing ($M[X]$ vs $M[M[X]]$) and why variable-length data is impossible without it; write MARIE loops over arrays using pointer initialisation (`Adr`), the 3-instruction pointer increment, and both termination styles (length counter with `SkipCond 400`, zero-sentinel with `SkipCond 800`); implement and call subroutines with `JnS`/`JumpI`, reserving the `HEX 0` return slot and passing arguments through labelled memory (and explain why recursion breaks); compute addressable capacity from address width and addressability (MARIE: $2^{12}$ words × 2 B = 8 KiB) and explain RAM's MUX-based row/column/byte decoding; and describe the memory hierarchy — cache purpose, transparency, prefetching and misses, swapping as the reverse of caching, and the register→cache→RAM→disk→network speed/size trade-offs.

After Week 5 you should be able to: identify motherboard components and explain why multiple I/O interface standards coexist (convenience/speed/cost/compatibility trade-offs); explain device registers and contrast memory-mapped I/O (Load/Store on mapped addresses; costs address space, bug-exposed) with port-mapped I/O (separate port space + dedicated instructions); compare polling, interrupt-driven I/O (checked before each fetch; handlers + context switches via shadow registers; IRQs → APIC) and DMA (direct device↔RAM transfer sharing the bus); recount the 12-step boot sequence from power-good through POST, boot sector, kernel load to GUI, and contrast BIOS with UEFI (disk limits, CPU modes, GUI, network, secure boot); explain the OS as abstraction/virtualisation, the kernel's process/memory/I-O management, timesharing with the Running/Ready/Blocked state cycle, user vs kernel mode, system calls and timer-driven preemption; and explain virtual memory's dual purpose — MMU-enforced per-process isolation on every access, and page-fault-driven swapping that provides more virtual memory than physical RAM.

After Week 6 you should be able to: define clients, servers, switches and routers and classify networks by reach (LAN, BN, MAN, WAN, Internet as network-of-networks); compute transfer times from data sizes and rates with correct byte→bit conversion; explain the five-layer Internet model with each layer's job and PDU (Message/Segment/Packet/Frame/Bit), distinguishing protocols (peer-to-peer, horizontal) from interfaces (adjacent layers, vertical) and knowing how high switches (Data Link) and routers (Network) climb; describe encapsulation down and up the stack; compare application architectures (server-based, client-based, client-server, thin client, multi-tier, P2P) via the four functions; read and label a raw HTTP request-response session (request line, headers, status, body; GET/HEAD/POST) and explain why one page triggers many cycles; and trace an email's three hops (SMTP push twice, POP/IMAP pull), read an SMTP dialogue, contrast POP (download+delete) with IMAP (server-side, multi-client), and explain MIME's base64 bridge for attachments.

After Week 7 you should be able to: explain how NICs implement the bottom two layers; distinguish digital encodings (unipolar, NRZ, NRZI, Manchester's self-clocking mid-bit transition) from analog modulation (frequency/amplitude/phase shift keying, and why combining AM+PM multiplies the data rate); describe Ethernet's evolution and recite CSMA/CD's carrier-sense, multiple-access and collision-detection (jam + random backoff) parts, including hub topology and shared-Ethernet's problems; state the address used at each layer (URL, port, IP, MAC) with the client-random/server-fixed port convention; do IPv4 subnet arithmetic with masks (/26) and explain IPv6's 128-bit hierarchical allocation; trace both resolutions — DNS's hierarchical name→IP lookup (iterative vs recursive with ISP caching) and ARP's broadcast IP→MAC discovery; explain per-hop routing-table forwarding with default gateways, static vs dynamic routing, and distance-vector (RIP, ≤15 hops) vs link-state (OSPF) algorithms; and detail TCP's connection lifecycle — sequence/acknowledgement byte counting, ARQ retransmission, 3-way open and full-duplex-forced 4-way close — against UDP's compact connectionless trade-off.

After Week 8 you should be able to: explain how a switch learns its forwarding table from sender MACs, floods unknowns, buffers with store-and-forward, and thereby delivers full-duplex collision-free Ethernet; contrast switches with hubs and routers; apply LAN design levers (standard upgrades, segmentation) to bottlenecks; explain WiFi's 802.11 family, 2.4 vs 5 GHz channels (only 1/6/11 orthogonal at 2.4 GHz), CSMA/CA with the hidden-node rationale and stop-and-wait ARQ, BSS/ESS topologies with roaming, attenuation-aware AP planning, and why servers never belong on WiFi; rank WiFi security modes (open — including captive portals, WEP's crackable static key, WPA2's per-packet AES keys in PSK vs Enterprise 802.1X modes); and describe organisational networking at every scale — owned LANs and fibre backbones in access/distribution/core layers, and the leased WAN triangle of dedicated circuits (guaranteed), carrier packet-switched services (shared) and encrypted VPN tunnels over the Internet (cheap, no guarantees).

After Week 9 you should be able to: describe the Internet as a **network of networks** of **Autonomous Systems** interconnected by **border routers** running **BGP**, distinguishing interior routing (RIP/OSPF/EIGRP, admin's choice) from exterior (BGP only), and explain **IXPs**, **peering vs transit**, the Tier 1/2/3 hierarchy, RIR/APNIC ASN allocation, and why no single body governs the Internet (ISOC/IETF, ICANN, ITU…); explain how an end user joins the Internet (ISP authenticates → assigns IP → supplies router/DNS) and compare access technologies — dial-up (modulate/demodulate, 54 kbit/s), **ADSL** (asymmetric, full-copper-bandwidth 4 kHz sub-bands, filter at home vs **DSLAM** at exchange, VDSL/FTTN), **NBN** (GPON fibre backbone, FTTP/FTTN/curb/fixed-wireless/satellite, RSP/wholesale/PoI) and **4G/5G** (cells, frequency↔range trade-off, latency/IoT aims); explain why huge services stay fast despite HTTP/TCP-IP/BGP not scaling — **load balancing** (DNS multi-IP, hardware LB), **content caching** (transparent cache engine, cacheable GET + `Expires`), and **CDNs** (points of presence near users, peering free at IXPs); describe the **IoT** (device-to-device, enabling cheap chips + IPv6 + low-power wireless) and its security weakness (default credentials → the **Mirai/Dyn** DDoS); and discuss the societal questions — **net neutrality** (equal treatment vs legitimate exceptions like spam/attack blocking and emergency prioritisation), apps vs open standards, platform vs **public utility / natural monopoly** regulation, and the difficulty of online law enforcement.

After Week 10 you should be able to: frame information security by its **goals** — confidentiality, integrity, authenticity, non-repudiation — and match each to the right primitive (encryption ⇒ confidentiality; keyed **MAC**/hash ⇒ integrity; signature + certificate ⇒ authenticity; public-key signature ⇒ non-repudiation), listing crypto/firewalls/MFA as the countermeasure toolkit; explain **symmetric cryptography** (a shared key, substitution **S-boxes** + **permutations** repeated over rounds → **AES/Rijndael**, block chaining with an IV and **CBC-MAC** as used by WPA2) and its three structural weaknesses — key distribution, $\frac{n(n-1)}{2}=O(n^2)$ key scaling, and no non-repudiation; explain **public-key (asymmetric) cryptography** — a key pair from a hard problem, used for encryption (encrypt with the public key), **digital signatures** (sign with the private key) and key establishment, the **RSA** operations $\text{cipher}=m^{e}\bmod n$ / $m=\text{cipher}^{d}\bmod n$ and its key generation ($p,q,n,\Phi(n),e,d$), and current key-length guidance (AES 128/256, RSA 2048/3072); state the properties of **cryptographic hash functions** (one-way, avalanche, collision-resistant), rank MD5/SHA-1/SHA-256, and explain why a bare hash cannot protect integrity in transit whereas a **keyed MAC** can; walk through **Diffie–Hellman key exchange** (public $g,n$, private $a,b$, shared $g^{ab}\bmod n$; the $g{=}5,n{=}47\to15$ example) and justify its security via the **discrete logarithm**, while recognising its lack of authentication; explain how **certificates** close that gap — a **certification authority** signs a public key with identity information, the certificate's contents (owner/validity/subject/issuer), revocation via **CRL** and **OCSP/OCSP stapling**, and the caveat that a certificate proves identity, not that a server is safe; and describe the two applied secure-channel protocols — **TLS** (a security layer between TCP and the application giving HTTPS, its handshake/record/alert sub-protocols, SSL→**TLS 1.3**, DH-established symmetric key, usually server-only authentication) and **VPNs** (an encrypted tunnel that logically relocates a device into a remote network via IPSec/OpenVPN/WireGuard, secure **only between tunnel endpoints**).

After Week 11 you should be able to: authenticate a **user** to a system — the three factor types (**something you know / have / are**), why passwords still dominate yet fail (reuse, weak choices, phishing/malware, bad storage, weak resets), and how to store credentials safely (**never cleartext**; a plain hash is beaten by **rainbow tables**; use a **per-user salted hash**), noting login is checked in the OS **kernel mode**; strengthen authentication with **multi-factor authentication** by combining factor types, weighing **biometrics** (usable but not secret, unrevocable, spoofable), **hardware tokens** (secure but costly/recoverable), and **authenticator apps** (weak if on the same device), plus **transaction authentication** (TANs, SMS-TAN and its **SIM-swap** weakness, barcode TAN generators); explain **access control** as deciding who may do what to which resources once authenticated, why **ACLs don't scale** ($1000$ staff × $200$ apps ≈ 2 million entries), how **ticket/token systems** (**Kerberos**, **Active Directory**) and **single sign-on** make it manageable at the cost of a single point of failure, and how access control is circumvented (software flaws, physical attacks, race conditions, USB, social engineering) and hardened (encryption, backups, updates, reduced complexity, Trusted Computing); describe **firewalls** as barriers that **filter (not block)** traffic between a more-secure inside and less-secure outside, how **packet filtering** works (source/destination IP, protocol, ports, connection state if stateful; inside→out usually allowed, outside→in blocked unless permitted) and its limits (stateless, no application context, blind to encrypted tunnels, useless against internal attackers); and explain **IDS vs IPS** (detect/alert/log vs actively block), **signature vs anomaly** detection (fast/known vs slower/novel), and **next-generation firewalls** (application-aware but whose TLS proxying **breaks end-to-end security** and becomes a single point of attack).

After Week 12 you should be able to: classify the common **attack and malware types** — **phishing** (fake login + lure), **ransomware** (encrypt-for-BitCoin; restore from backup, don't pay), **social engineering**, **botnets** (bots → command-and-control → **DDoS**), **denial of service**, and the **virus vs worm vs trojan** distinction (host-attached vs standalone-self-propagating vs hidden-in-legit-software), while debunking "only careless people get malware" (malvertising spreads with no interaction) and the false comfort of anti-virus (known-malware only, a prime target, blind to new malware); explain the four classic **software vulnerabilities** — **buffer overflow** (overwrite the return address; canary/ASLR defences), **command injection** (`;rm -rf /` executed with the host's privileges), **cross-site scripting** (attacker script runs with the trusted domain's rights; stored XSS steals session tokens), and **SQL injection** ("Bobby Tables") — and identify their shared root cause (**unchecked input + excessive privilege**) and defences (sanitisation, parameterised queries/output encoding, least privilege), noting CWE/OWASP as references; recount real **case studies** — the **F5 BIG-IP** management-plane RCE, **Stuxnet** jumping an air gap via USB to destroy centrifuges, the 2008 **Turkey pipeline** ("the main weapon was a keyboard"), and the **Bangladesh Bank** SWIFT theft — drawing the lesson that **exposure plus insecure defaults** is the core risk and patching doesn't clean an already-compromised device; frame **cybersecurity risk management** as accepting that perfect security is impossible and instead managing **residual risk** with the right controls (**NIST RMF** families spanning technical, physical and human domains; the **NICE** framework's 52 professional roles); and discuss **privacy** in the big-data age — cross-linked profiling, "**you are the product**", **privacy-enhancing technologies** (group/ring signatures) that exist but are underused, cookie pop-ups built for **compliance not traceability**, practical self-defence (cookie/script controls, Signal, awareness), and how **data minimisation** improves **both** privacy and cybersecurity (smaller attack surface, less data to misuse).
