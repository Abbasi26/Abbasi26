# Hi, I'm Wasaf 👋

I build small, **read-only-by-default** tools for the unglamorous parts of IT operations: endpoint state, certificates, patch priorities, runbooks, logs and AI-assisted coding.

Every tool below is MIT-licensed, ships an **offline demo with fictional data** that runs in under a minute, sends no telemetry, and writes plain HTML / Markdown / JSON / CSV reports.

[**Website**](https://abbasi26.github.io/) · [**Writing**](https://abbasi26.github.io/posts/) · [**RSS**](https://abbasi26.github.io/index.xml)

## Endpoint management (Intune / Entra ID / ConfigMgr)

| Tool | What it does | Status |
|---|---|---|
| [**endpoint-quorum**](https://github.com/Abbasi26/endpoint-quorum) · PowerShell | Finds devices that Intune, Entra ID and Defender for Endpoint disagree about. Read-only, `Invoke-Quorum -Demo` runs offline. | [![release](https://img.shields.io/github/v/release/Abbasi26/endpoint-quorum?label=release)](https://github.com/Abbasi26/endpoint-quorum/releases/latest) [![CI](https://github.com/Abbasi26/endpoint-quorum/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/Abbasi26/endpoint-quorum/actions/workflows/ci.yml) [![license](https://img.shields.io/github/license/Abbasi26/endpoint-quorum)](https://github.com/Abbasi26/endpoint-quorum/blob/main/LICENSE) |
| [**secure-app-factory**](https://github.com/Abbasi26/secure-app-factory) · PowerShell | Pinned, reproducible Win32 packaging for Intune: SHA-256 + signer pin, PSADT 4.1, `.intunewin`, CycloneDX SBOM, provenance. | [![release](https://img.shields.io/github/v/release/Abbasi26/secure-app-factory?label=release)](https://github.com/Abbasi26/secure-app-factory/releases/latest) [![CI](https://github.com/Abbasi26/secure-app-factory/actions/workflows/package.yml/badge.svg?branch=main)](https://github.com/Abbasi26/secure-app-factory/actions/workflows/package.yml) [![license](https://img.shields.io/github/license/Abbasi26/secure-app-factory)](https://github.com/Abbasi26/secure-app-factory/blob/main/LICENSE) |
| [**logsieve**](https://github.com/Abbasi26/logsieve) · Python | Puts ConfigMgr, Intune and Windows logs on one timeline, explains known error codes, and pseudonymises identifiers before sharing. | [![release](https://img.shields.io/github/v/release/Abbasi26/logsieve?label=release)](https://github.com/Abbasi26/logsieve/releases/latest) [![CI](https://github.com/Abbasi26/logsieve/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/Abbasi26/logsieve/actions/workflows/test.yml) [![license](https://img.shields.io/github/license/Abbasi26/logsieve)](https://github.com/Abbasi26/logsieve/blob/main/LICENSE) |

## Security & compliance

| Tool | What it does | Status |
|---|---|---|
| [**grundschutz-check**](https://github.com/Abbasi26/grundschutz-check) · PowerShell | Read-only Windows 11 checks against BSI IT-Grundschutz and Grundschutz++, with a cited evidence report. | [![release](https://img.shields.io/github/v/release/Abbasi26/grundschutz-check?label=release)](https://github.com/Abbasi26/grundschutz-check/releases/latest) [![CI](https://github.com/Abbasi26/grundschutz-check/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/Abbasi26/grundschutz-check/actions/workflows/test.yml) [![license](https://img.shields.io/github/license/Abbasi26/grundschutz-check)](https://github.com/Abbasi26/grundschutz-check/blob/main/LICENSE) |
| [**certclock**](https://github.com/Abbasi26/certclock) · Python | Agentless certificate and CA expiry radar: TLS endpoints, files and internal CAs on one timeline, plus a CI gate. | [![release](https://img.shields.io/github/v/release/Abbasi26/certclock?label=release)](https://github.com/Abbasi26/certclock/releases/latest) [![CI](https://github.com/Abbasi26/certclock/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/Abbasi26/certclock/actions/workflows/ci.yml) [![license](https://img.shields.io/github/license/Abbasi26/certclock)](https://github.com/Abbasi26/certclock/blob/main/LICENSE) |
| [**patchorder**](https://github.com/Abbasi26/patchorder) · Python | Which CVEs hit the versions you actually run, ranked with CISA KEV, EPSS and exposure. No scanning. | [![release](https://img.shields.io/github/v/release/Abbasi26/patchorder?label=release)](https://github.com/Abbasi26/patchorder/releases/latest) [![CI](https://github.com/Abbasi26/patchorder/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/Abbasi26/patchorder/actions/workflows/ci.yml) [![license](https://img.shields.io/github/license/Abbasi26/patchorder)](https://github.com/Abbasi26/patchorder/blob/main/LICENSE) |

## Operations & developer tooling

| Tool | What it does | Status |
|---|---|---|
| [**runbook-rehearsal**](https://github.com/Abbasi26/runbook-rehearsal) · Python | Dry-runs runbooks and flags stale reviews, dead contacts, 404s, missing files and broken scripts, with a freshness score. | [![release](https://img.shields.io/github/v/release/Abbasi26/runbook-rehearsal?label=release)](https://github.com/Abbasi26/runbook-rehearsal/releases/latest) [![CI](https://github.com/Abbasi26/runbook-rehearsal/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/Abbasi26/runbook-rehearsal/actions/workflows/ci.yml) [![license](https://img.shields.io/github/license/Abbasi26/runbook-rehearsal)](https://github.com/Abbasi26/runbook-rehearsal/blob/main/LICENSE) |
| [**specfreeze**](https://github.com/Abbasi26/specfreeze) · Python | Ask design questions first, freeze the interface contract, reject LLM-generated code that drifts from it. | [![release](https://img.shields.io/github/v/release/Abbasi26/specfreeze?label=release)](https://github.com/Abbasi26/specfreeze/releases/latest) [![CI](https://github.com/Abbasi26/specfreeze/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/Abbasi26/specfreeze/actions/workflows/ci.yml) [![license](https://img.shields.io/github/license/Abbasi26/specfreeze)](https://github.com/Abbasi26/specfreeze/blob/main/LICENSE) |

## Writing

One write-up per tool: the problem it solves, a demo you can run offline, and what it deliberately doesnt do. Theyre at [abbasi26.github.io/posts](https://abbasi26.github.io/posts/), and the [RSS feed](https://abbasi26.github.io/index.xml) has the full text.

- [certclock: one timeline for every certificate](https://abbasi26.github.io/posts/certclock-one-timeline-for-every-certificate/)
- [endpoint-quorum: when Intune, Entra ID and Defender disagree](https://abbasi26.github.io/posts/endpoint-quorum-when-intune-entra-and-defender-disagree/)
- [grundschutz-check: Windows 11 against BSI IT-Grundschutz](https://abbasi26.github.io/posts/grundschutz-check-windows-11-against-bsi-grundschutz/)
- [logsieve: one timeline for ConfigMgr, Intune and Windows logs](https://abbasi26.github.io/posts/logsieve-one-timeline-for-configmgr-intune-and-windows-logs/)
- [patchorder: which CVEs hit the versions you run](https://abbasi26.github.io/posts/patchorder-which-cves-hit-the-versions-you-run/)
- [runbook-rehearsal: dry-run your runbooks](https://abbasi26.github.io/posts/runbook-rehearsal-dry-run-your-runbooks/)
- [secure-app-factory: pinned Win32 packaging for Intune](https://abbasi26.github.io/posts/secure-app-factory-pinned-win32-packaging-for-intune/)
- [specfreeze: freeze the interface before the model writes code](https://abbasi26.github.io/posts/specfreeze-freeze-the-interface-before-the-model-writes-code/)

## Principles

- **Read-only first.** Anything that changes a system or sends data needs an explicit switch.
- **Evidence over claims.** Reports cite their sources and mark what is unverified.
- **Privacy by default.** Identifiers are pseudonymised or fingerprinted where reports might be shared.
- **Try before you trust.** Each repo has a one-command offline demo.

## Contributing

Issues, ideas and pull requests are welcome. Every repo has a `ROADMAP.md` with good first issues and issue forms.
