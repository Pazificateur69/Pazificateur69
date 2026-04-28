<!-- ─────────────────────────────────────────────────────────────────────
     Pazent's GitHub profile README
     Drop this file at the root of github.com/Pazificateur69/Pazificateur69
     as `README.md` — it will render on your public profile page.
     ───────────────────────────────────────────────────────────────────── -->

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0a0d12,50:3fd0d4,100:c8a96b&height=240&section=header&text=Pazent&fontSize=80&fontColor=f6f9fc&animation=fadeIn&fontAlignY=38&desc=Quantum-resistant%20systems%20engineer&descAlignY=58&descSize=18" alt="header banner" />

<br />

<a href="https://curs3d.fr"><img src="https://img.shields.io/badge/curs3d.fr-3fd0d4?style=for-the-badge&logo=rust&logoColor=white" alt="curs3d.fr" /></a>
<a href="https://explorer.curs3d.fr"><img src="https://img.shields.io/badge/Live%20Explorer-0a0d12?style=for-the-badge&logo=ethereum&logoColor=3fd0d4" alt="explorer" /></a>
<a href="https://api.curs3d.fr/api/status"><img src="https://img.shields.io/badge/Testnet%20Live-c8a96b?style=for-the-badge&logo=hyper&logoColor=white" alt="testnet" /></a>
<a href="mailto:agencenetstrategy@gmail.com"><img src="https://img.shields.io/badge/Contact-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="email" /></a>

<br /><br />

<a href="https://github.com/Pazificateur69">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=22&duration=3500&pause=900&color=3FD0D4&center=true&vCenter=true&width=720&lines=Building+a+post-quantum+Layer+1+from+scratch+in+Rust;Dilithium+L5+%E2%80%A2+BFT+PoS+%E2%80%A2+WASM+VM+%E2%80%A2+Light+clients;Solo+dev+%E2%80%A2+Open+source+(MIT)+%E2%80%A2+Live+testnet" alt="rotating tagline" />
</a>

</div>

---

## 🜲 Featured project — CURS3D

> **A quantum-resistant Layer 1 blockchain, built from zero in Rust.**
> No fork, no copy-paste — every component (consensus, crypto, networking, storage, VM, API) implemented from scratch with NIST-standardized post-quantum primitives.

<table>
  <tr>
    <td valign="top" width="50%">

**Why it matters**

NIST published FIPS 204 (CRYSTALS-Dilithium) in August 2024. CNSA 2.0 (US) mandates post-quantum migration by 2030. eIDAS 2.0 (EU) will require it for the European digital wallet.

Every existing chain — Bitcoin, Ethereum, Solana — is built on ECDSA, which is broken by Shor's algorithm. CURS3D is a working reference implementation of what the migration looks like at L1.

**What's running today**

- 4 BFT validators on Oracle Cloud ARM (Marseille, EU)
- ~31,400 lines of Rust • 145 tests • 0 clippy warnings
- HTTP REST API + Ethereum-compatible JSON-RPC + WebSocket events
- Rust SDK with 5 example contracts (counter, ERC-20, multisig, NFT, vesting)
- Public block explorer + bilingual website (EN/FR)

    </td>
    <td valign="top" width="50%">

**Stack**

```
Crypto      CRYSTALS-Dilithium L5  (FIPS 204)
            SHA-3 Keccak-256       (FIPS 202)
Consensus   BFT PoS, 2/3 finality, slashing
VM          Wasmer 5 + Cranelift, fuel metering
Network     libp2p 0.54 + Gossipsub
Storage     sled, Sparse Merkle Trie
Wallet      AES-256-GCM + Argon2id
API         hyper 1.x + tokio + tungstenite
```

**Try it now**

```bash
# Status of the live testnet
curl -s https://api.curs3d.fr/api/status | jq

# Ethereum-compatible RPC (Metamask, ethers.js)
curl -s -X POST https://api.curs3d.fr/eth \
  -H 'content-type: application/json' \
  -d '{"jsonrpc":"2.0","id":1,"method":"eth_blockNumber"}'
```

[**→ Read the whitepaper**](https://curs3d.fr/whitepaper.html) &nbsp;•&nbsp; [**→ Run a validator**](https://curs3d.fr/run-validator.html) &nbsp;•&nbsp; [**→ Source code**](https://github.com/Pazificateur69/curs3d)

    </td>
  </tr>
</table>

---

## ⛁ Tech stack

<div align="center">

<img src="https://skillicons.dev/icons?i=rust,wasm,docker,linux,nginx,bash,nodejs,ts,react,tailwind,postgres,redis,git,github,vscode&perline=15" alt="tech stack" />

<br /><br />

<a href="#"><img src="https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white" /></a>
<a href="#"><img src="https://img.shields.io/badge/WebAssembly-654FF0?style=flat-square&logo=webassembly&logoColor=white" /></a>
<a href="#"><img src="https://img.shields.io/badge/libp2p-3FD0D4?style=flat-square" /></a>
<a href="#"><img src="https://img.shields.io/badge/Wasmer-4946DD?style=flat-square&logo=webassembly&logoColor=white" /></a>
<a href="#"><img src="https://img.shields.io/badge/Tokio-DAD2D8?style=flat-square&logo=rust&logoColor=black" /></a>
<a href="#"><img src="https://img.shields.io/badge/sled-FF5B00?style=flat-square" /></a>
<a href="#"><img src="https://img.shields.io/badge/Dilithium%20L5-0F1729?style=flat-square&logoColor=white" /></a>
<a href="#"><img src="https://img.shields.io/badge/SHA--3-2B2D42?style=flat-square" /></a>

</div>

---

## ✦ GitHub at a glance

<div align="center">

<a href="https://github.com/Pazificateur69">
  <img height="180em" src="https://github-readme-stats.vercel.app/api?username=Pazificateur69&show_icons=true&theme=midnight-purple&hide_border=true&bg_color=0a0d12&title_color=3fd0d4&text_color=d8e2ec&icon_color=c8a96b&include_all_commits=true&count_private=true" alt="GitHub stats" />
  <img height="180em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Pazificateur69&layout=compact&theme=midnight-purple&hide_border=true&bg_color=0a0d12&title_color=3fd0d4&text_color=d8e2ec&langs_count=8" alt="Top languages" />
</a>

<br /><br />

<a href="https://git.io/streak-stats">
  <img src="https://streak-stats.demolab.com?user=Pazificateur69&theme=midnight-purple&hide_border=true&background=0a0d12&stroke=3fd0d4&ring=c8a96b&fire=c8a96b&currStreakLabel=3fd0d4&currStreakNum=f6f9fc&sideNums=f6f9fc&dates=a4b3c3&sideLabels=a4b3c3" alt="GitHub Streak" />
</a>

<br /><br />

<a href="https://github.com/Pazificateur69">
  <img src="https://github-profile-trophy.vercel.app/?username=Pazificateur69&theme=onedark&no-frame=true&no-bg=true&column=7&margin-w=10" alt="trophies" />
</a>

</div>

---

## 🜂 Activity

<div align="center">

<img src="https://github-readme-activity-graph.vercel.app/graph?username=Pazificateur69&bg_color=0a0d12&color=3fd0d4&line=c8a96b&point=f6f9fc&hide_border=true&area=true&custom_title=Contribution%20Activity" alt="activity graph" />

</div>

---

## 𓅪 The snake

<div align="center">

<img src="https://raw.githubusercontent.com/Pazificateur69/Pazificateur69/output/github-snake-dark.svg" alt="snake animation" />

</div>

---

## 🜨 What I'm focused on right now

```rust
struct CurrentlyFocusedOn {
    primary:   "CURS3D testnet stability + external audit prep",
    research:  "Post-quantum migration paths for legacy chains",
    learning:  ["Formal verification (TLA+, Tamarin)",
                "MPC and threshold-Dilithium",
                "BFT under network partition"],
    open_to:   "Grant collaborations, freelance Rust/security",
    location:  "France 🇫🇷  •  remote-first",
}
```

---

<div align="center">

**Building things meant to last —** **building post-quantum is building for a 50-year horizon.**

<sub><sup>⚙ Profile auto-built with GitHub Actions • snake animation regenerated every 6h • last touched today</sup></sub>

<br />

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:c8a96b,50:3fd0d4,100:0a0d12&height=120&section=footer&reversal=true" alt="footer" />

</div>
