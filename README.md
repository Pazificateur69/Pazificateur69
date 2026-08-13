<!-- ─────────────────────────────────────────────────────────────────────
     Alessandro Gagliardi — GitHub profile README
     Lives at github.com/Pazificateur69/Pazificateur69/README.md
     ───────────────────────────────────────────────────────────────────── -->

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0a0d12,50:3fd0d4,100:c8a96b&height=240&section=header&text=Pazent&fontSize=80&fontColor=f6f9fc&animation=fadeIn&fontAlignY=38&desc=Cybersecurity%20%C2%B7%20DevSecOps%20Engineer&descAlignY=58&descSize=18" alt="header banner" />

<br />

<a href="mailto:agencenetstrategy@gmail.com"><img src="https://img.shields.io/badge/Contact-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="email" /></a>
<a href="https://github.com/Pazificateur69/gauntlet"><img src="https://img.shields.io/badge/Container%20security-0a0d12?style=for-the-badge&logo=docker&logoColor=3fd0d4" alt="container security" /></a>
<a href="https://github.com/Pazificateur69/aedsc-action"><img src="https://img.shields.io/badge/Shift--left%20CI-3fd0d4?style=for-the-badge&logo=githubactions&logoColor=white" alt="secure ci" /></a>
<a href="https://github.com/pazent/exploitspec"><img src="https://img.shields.io/badge/Exploit%20regression-c8a96b?style=for-the-badge&logo=githubactions&logoColor=white" alt="ExploitSpec" /></a>
<a href="https://curs3d.fr"><img src="https://img.shields.io/badge/Post--quantum%20L1-c8a96b?style=for-the-badge&logo=rust&logoColor=white" alt="curs3d" /></a>

<br /><br />

<a href="https://github.com/Pazificateur69">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=22&duration=3500&pause=900&color=3FD0D4&center=true&vCenter=true&width=780&lines=Security+engineer+%E2%80%94+I+break+it%2C+then+I+make+it+hold;Secure+CI%2FCD+%E2%80%A2+Container+hardening+%E2%80%A2+Linux+infrastructure;Offensive+background%2C+defensive+job+%E2%80%94+both+sides+of+the+wire" alt="rotating tagline" />
</a>

</div>

---

## ⛨ Who I am

Cybersecurity & DevSecOps engineer based in Lyon, France. I hold the French **RNCP *Administrateur d'Infrastructures Sécurisées*** title (Guardia Cybersecurity School, 2026), and I currently own application and production-server security for a web agency's entire client estate — the whole loop, from finding the vulnerability to watching the fix ship.

My work sits on both sides of the wire: I audit and exploit (OWASP Top 10, bug bounty, red-team tooling), then I build the controls that make the same class of bug impossible next time (pipeline gates, hardened images, network segmentation).

<table>
<tr>
<td valign="top" width="33%">

### ⚙ Secure CI/CD

Security as a pipeline property, not a good intention.

- **SAST** — Semgrep, SonarQube-class gating
- **SCA & images** — Trivy
- **Secrets** — Gitleaks, pre-push and in-CI
- **DAST** — OWASP ZAP
- **Supply chain** — CycloneDX SBOM + Cosign signing
- **Runtime** — distroless, non-root, read-only rootfs

*A committed secret doesn't reach production. It breaks the build.*

</td>
<td valign="top" width="33%">

### ⌖ Offensive security

You cannot defend an attack path you've never walked.

- Web / network / system pentesting
- **Bug bounty** — 2 high-severity findings accepted at a telecom operator (YesWeHack)
- White-box audits: OWASP / CWE / CVSS scoring, prioritised remediation roadmaps
- IDOR, privilege escalation, exposed secrets, file inclusion
- Red-team tooling — see `T3MP3ST`, `NightOwl`

</td>
<td valign="top" width="33%">

### ⛯ Infrastructure hardening

Linux, containers, and the blast radius around them.

- Host hardening — SSH key-only, `nftables`, kernel CVE patching, Lynis scoring
- **WAF** — ModSecurity + OWASP CRS in blocking mode
- **IDS/IPS** — CrowdSec, Fail2ban, Suricata, Wazuh
- **Containers** — `seccomp`, `cgroups`, capability dropping, user namespaces, gVisor
- **Kubernetes** — deny-all NetworkPolicies, `runAsNonRoot`, namespace isolation
- **IaC** — Terraform, Ansible, bastion / jump-host topologies

</td>
</tr>
</table>

---

## ✦ Selected work

Each of these exists to prove one thing. That thing is in the right-hand column.

| Project | What it is | What it demonstrates |
|---|---|---|
| **[ExploitSpec](https://github.com/pazent/exploitspec)** | Turns proven exploits into permanent regression tests — import a sanitized cURL, express the invariant in YAML, run locally or in GitHub Actions. | Bridges offensive findings and defensive CI: **RED → GREEN → STABLE**. Local-first, no account, no telemetry, Apache-2.0. |
| **[gauntlet](https://github.com/Pazificateur69/gauntlet)** | Secure remote-code-execution & online-judge platform. Treats every submission as hostile. | Container escape defence — `seccomp`, `cgroups`, dropped capabilities, user namespaces, optional gVisor. Full [`THREAT_MODEL.md`](https://github.com/Pazificateur69/gauntlet/blob/main/THREAT_MODEL.md). K8s manifests with **deny-all-by-default NetworkPolicy**, non-root pods, read-only rootfs. |
| **[aedsc-action](https://github.com/Pazificateur69/aedsc-action)** | GitHub Action running Slither + Aderyn on every pull request. | Shift-left security in practice — automated scanning wired into the review loop, with results where developers actually read them. |
| **[T3MP3ST](https://github.com/Pazificateur69/T3MP3ST)** | Autonomous red-teaming platform — a multi-agent offensive-security meta-harness. | Offensive automation and attack-chain orchestration. |
| **[mldsa-kit](https://github.com/Pazificateur69/mldsa-kit)** | FIPS-204 ML-DSA-87 post-quantum signing for Rust, with an encrypted keystore. | Applied cryptography — Argon2id + AES-256-GCM key protection, byte-for-byte browser↔native interop, stable toolchain. |
| **[pricestream](https://github.com/Pazificateur69/pricestream)** | Real-time crypto pricing & liquidity service — Django, Kafka, Celery, WebSockets. | Distributed systems and observability — Prometheus metrics, deep health probes, Kubernetes manifests, CI. |
| **[NightOwl](https://github.com/Pazificateur69/NightOwl)** | 57-module open-source pentesting framework. | Breadth across the offensive toolchain. |

<p align="center">
  <a href="https://github.com/pazent/exploitspec"><img src="https://raw.githubusercontent.com/pazent/exploitspec/v0.1.0/docs/demo.svg" width="900" alt="ExploitSpec RED GREEN STABLE demo" /></a>
  <br />
  <a href="https://github.com/pazent/exploitspec/actions/workflows/ci.yml"><img src="https://github.com/pazent/exploitspec/actions/workflows/ci.yml/badge.svg?branch=main" alt="CI" /></a>
  <a href="https://github.com/pazent/exploitspec/releases/tag/v0.1.0"><img src="https://img.shields.io/github/v/release/pazent/exploitspec?style=flat-square&color=3fd0d4" alt="release" /></a>
  <a href="https://github.com/pazent/exploitspec/blob/main/LICENSE"><img src="https://img.shields.io/github/license/pazent/exploitspec?style=flat-square&color=c8a96b" alt="license" /></a>
</p>

<details>
<summary><b>More — infrastructure, backend, Web3</b></summary>

<br />

| Project | Stack |
|---|---|
| [market-data-collector](https://github.com/Pazificateur69/market-data-collector) | Async Python → Kafka. `asyncio`, `aiokafka`, `mypy --strict`, multi-stage Dockerfile |
| [pricing-grpc-service](https://github.com/Pazificateur69/pricing-grpc-service) | Async gRPC, unary + server-streaming, strict typing, CI |
| [zenith](https://github.com/Pazificateur69/zenith) | Solidity contracts for a rollup system |
| [concierge](https://github.com/Pazificateur69/concierge) | Unified hotel-facing touchscreen platform (TypeScript) |

</details>

---

## ⛊ In production

What I do outside GitHub — application and infrastructure security for a web agency's client estate.

<table>
<tr>
<td valign="top" width="50%">

**Built the DevSecOps pipeline**

Went from manual, occasional review to automated gating on every push: Semgrep (SAST), Trivy (dependencies + images), Gitleaks (secrets), OWASP ZAP (DAST) — with a CycloneDX SBOM and Cosign signature on what ships, and base images rebuilt distroless and non-root.

**Audited the estate, then got it fixed**

White-box audit of a production SaaS (Angular / Laravel): **45 vulnerabilities** scored OWASP / CWE / CVSS, including a **CVSS 9.9 privilege escalation** and IDOR across 11 controllers. Then three internal applications — 31 findings on a Next.js CRM, and **52 of 53 findings actually remediated** on an accounting application.

*Finding bugs is the easy half. Getting them closed is the job.*

</td>
<td valign="top" width="50%">

**Hardened the production servers**

Defence in depth on the estate's production host: SSH key-only, ModSecurity + OWASP CRS switched to blocking, CrowdSec and Fail2ban (~15 000 IPs banned), **7 Docker ports pulled off the public internet**, 9 kernel CVEs patched. **Lynis score 67 → 77.**

**Handled a real intrusion attempt**

A file-inclusion attempt targeting `/.env` — contained, then an anti-dotfile rule deployed across every hosted domain.

**Then re-verified it two months later.** The controls still held. Hardening that isn't re-checked is hardening that quietly rotted.

</td>
</tr>
</table>

---

## ⛁ Tech stack

<div align="center">

<img src="https://skillicons.dev/icons?i=linux,docker,kubernetes,bash,python,rust,nginx,postgres,redis,ts,nodejs,git,github,terraform,ansible&perline=15" alt="tech stack" />

<br /><br />

<img src="https://img.shields.io/badge/Semgrep-1B2B34?style=flat-square&logoColor=white" />
<img src="https://img.shields.io/badge/Trivy-1904DA?style=flat-square&logo=aqua&logoColor=white" />
<img src="https://img.shields.io/badge/Gitleaks-2B2D42?style=flat-square" />
<img src="https://img.shields.io/badge/OWASP%20ZAP-000000?style=flat-square&logo=owasp&logoColor=white" />
<img src="https://img.shields.io/badge/CycloneDX%20SBOM-3fd0d4?style=flat-square&logoColor=black" />
<img src="https://img.shields.io/badge/Cosign-0F1729?style=flat-square&logoColor=white" />
<img src="https://img.shields.io/badge/ModSecurity%20%2B%20CRS-c8a96b?style=flat-square&logoColor=black" />
<img src="https://img.shields.io/badge/CrowdSec-FF5B00?style=flat-square" />
<img src="https://img.shields.io/badge/Suricata-EE3124?style=flat-square&logo=suricata&logoColor=white" />
<img src="https://img.shields.io/badge/Wazuh-3F80EA?style=flat-square" />
<img src="https://img.shields.io/badge/Burp%20Suite-FF6633?style=flat-square&logo=burpsuite&logoColor=white" />
<img src="https://img.shields.io/badge/Nmap-4682B4?style=flat-square" />
<img src="https://img.shields.io/badge/Metasploit-2596CD?style=flat-square&logo=metasploit&logoColor=white" />
<img src="https://img.shields.io/badge/Proxmox-E57000?style=flat-square&logo=proxmox&logoColor=white" />
<img src="https://img.shields.io/badge/OPNsense-D94F00?style=flat-square&logo=opnsense&logoColor=white" />
<img src="https://img.shields.io/badge/WireGuard-88171A?style=flat-square&logo=wireguard&logoColor=white" />

</div>

---

## ⟠ Web3, on the side

Same discipline, different threat model — and the reason I went deep on applied cryptography.

> ### CURS3D — a quantum-resistant Layer 1, written from scratch in Rust
>
> No fork, no copy-paste. Consensus, crypto, networking, storage, VM and API all implemented from zero on NIST-standardised post-quantum primitives — because every chain in production today signs with ECDSA, which Shor's algorithm breaks.
>
> **ML-DSA-87 / CRYSTALS-Dilithium L5** (FIPS 204) · SHA-3 Keccak-256 · BFT PoS with slashing · Wasmer 5 + Cranelift WASM VM with fuel metering · libp2p + Gossipsub · AES-256-GCM + Argon2id wallet
>
> Live public developer testnet, 5 validators across 4 providers, MetaMask-compatible JSON-RPC alongside native post-quantum transactions. Not audited, not production, no monetary value — deliberately.
>
> [**→ curs3d.fr**](https://curs3d.fr) &nbsp;•&nbsp; [**→ whitepaper**](https://curs3d.fr/whitepaper.html) &nbsp;•&nbsp; [**→ source**](https://github.com/Pazificateur69/curs3d) &nbsp;•&nbsp; [**→ live status**](https://api.curs3d.fr/api/status)

Also: [`mldsa-kit`](https://github.com/Pazificateur69/mldsa-kit) (post-quantum signing library), [`zenith`](https://github.com/Pazificateur69/zenith) (rollup contracts), [`aedsc-action`](https://github.com/Pazificateur69/aedsc-action) (Solidity security scanning in CI).

---

## ✧ GitHub at a glance

<div align="center">

<img src="https://github-readme-activity-graph.vercel.app/graph?username=Pazificateur69&bg_color=0a0d12&color=3fd0d4&line=c8a96b&point=f6f9fc&hide_border=true&area=true&custom_title=Contribution%20Activity" alt="activity graph" />

</div>

---

## ⛬ Currently

```yaml
role:      Application & infrastructure security — agency client estate
focus:
  - Kubernetes security: RBAC, NetworkPolicies, admission control
  - Supply-chain integrity: SBOM, signing, provenance
  - Detection engineering on production Linux hosts
learning:  [ CKA, threat modelling at design time, eBPF observability ]
open_to:   DevSecOps / security engineering roles — Lyon, France
languages: FR native · EN C1 · IT B2
```

---

<div align="center">

**Security that isn't automated is security that happens when someone remembers.**

<br />

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:c8a96b,50:3fd0d4,100:0a0d12&height=120&section=footer&reversal=true" alt="footer" />

</div>
