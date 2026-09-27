<div align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,50:0f2e1d,100:00ff9c&height=140&section=header&text=Digital%20Forensics&fontSize=36&fontColor=00ff9c&fontAlignY=55" />
<br>
<img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&size=18&duration=2500&pause=800&color=00FF9C&center=true&vCenter=true&width=650&lines=Windows+Artifacts+for+SOC+Analysts;Evidence.+Timelines.+Attribution.;Notes+From+the+Field%2C+Not+the+Textbook" />
<br>

[![License: MIT](https://img.shields.io/badge/License-MIT-00FF9C.svg)](LICENSE)
![Status: Active](https://img.shields.io/badge/Status-Active-00FF9C)
![Focus: Windows Forensics](https://img.shields.io/badge/Focus-Windows%20Forensics-0f2e1d)
![Level: SOC Analyst](https://img.shields.io/badge/Level-SOC%20Analyst-16213e)

</div>

<br>

## Overview

This repository is a working reference on **digital forensics for SOC analysts**, with a specific focus on investigating malicious activity in **Windows-based environments**. It is written as a practical companion for analysts who already understand the basics of incident response and need a fast, reliable place to check what an artifact means, where it lives, and why it matters during an investigation.

This is not an exhaustive academic treatment of digital forensics. It is a working foundation — enough depth to confidently identify, preserve, and interpret the artifacts that show up in real Windows compromises, without wading through unrelated theory to get there.

<br>

## What's Inside

| File | Covers |
|---|---|
| [`01Introduction_to_Digital_Forensics.md`](./01_Introduction_to_Digital_Forensics.md) | Core concepts, the forensic process, evidence types, and why digital forensics matters to a SOC |
| [`02_Windows_Forensics_Overview.md`](./02_Windows_Forensics_Overview.md) | NTFS artifacts, Windows Event Logs, execution artifacts (Prefetch, Shimcache, Amcache, UserAssist), persistence mechanisms, browser forensics, and SRUM |

<br>

## Core Topics

- **Forensic Fundamentals** — identification, collection, examination, analysis, and presentation of digital evidence, plus chain-of-custody and evidence integrity.
- **NTFS Artifacts** — MFT entries, file slack, USN Journal, LNK files, shellbags, alternate data streams, and volume shadow copies.
- **Execution Evidence** — Prefetch, Shimcache, Amcache, UserAssist, and Jump Lists, mapped to their exact registry keys and file paths.
- **Persistence Mechanisms** — Run/RunOnce keys, WinLogon hijacks, scheduled tasks, and rogue services.
- **Browser & User Activity** — history, cache, downloads, autofill, and session data as indicators of user behavior.
- **SRUM Analysis** — resource usage tracking for application profiling, timeline reconstruction, and malware detection.

<br>

## How to Use This Repo

- **Read sequentially** if you're building foundational knowledge — start with the introduction, then move into the Windows-specific artifacts.
- **Jump straight to a topic** if you're mid-investigation — every file uses consistent headers, so Ctrl+F / Cmd+F gets you to the relevant artifact fast.
- **Clone locally** for offline reference during engagements where browser access is restricted:

```bash
git clone https://github.com/tousifahmed101-0xT/Introduction-to-Digital-Forensics.git
cd  Introduction-to-Digital-Forensics
```

<br>

## A Note on Scope

The artifact locations, registry keys, and file paths referenced throughout this repo reflect standard Windows behavior at the time of writing. Paths and behaviors can shift across Windows versions and builds, so always validate against the specific OS version in scope during a live investigation rather than relying on these notes alone.

<br>

## Contributing

Corrections and additions are welcome, provided they hold to the same standard as the rest of the repo:

1. Verify artifact locations and registry keys against a real system before submitting.
2. Keep explanations precise — this repo favors clarity over length.
3. Cite the Windows version(s) an artifact applies to, if it's version-specific.
4. Open an issue first for a new artifact category so scope stays focused.

<br>

## License

MIT — see [LICENSE](LICENSE) for details.

<br>

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,50:0f2e1d,100:00ff9c&height=100&section=footer" />
</div>

<div align="center">
<br>
Maintained by <a href="https://github.com/tousifahmed101-0xT">Tousif Ahmed</a>
</div>
