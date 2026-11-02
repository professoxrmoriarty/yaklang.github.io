<div align="center">
  <img
    src="https://raw.githubusercontent.com/yaklang/.github/main/profile/assets/yak-logo.png"
    alt="YAK"
    width="280"
  />

  <br/>

  <strong>Security Capability Convergence · AI-Native Cybersecurity Technology Stack</strong>

  <br/><br/>

  <a href="https://github.com/professoxrmoriarty/yaklang"><img alt="Yaklang Stars" src="https://img.shields.io/github/stars/professoxrmoriarty/yaklang?style=social"/></a>
  <a href="https://github.com/professoxrmoriarty/yakit"><img alt="Yakit Stars" src="https://img.shields.io/github/stars/professoxrmoriarty/yakit?style=social"/></a>
  <a href="https://github.com/professoxrmoriarty/yaklang/releases"><img alt="Yaklang Release" src="https://img.shields.io/github/release/professoxrmoriarty/yaklang.svg"/></a>
  <a href="https://github.com/professoxrmoriarty/yaklang/releases"><img alt="Yaklang Downloads" src="https://img.shields.io/github/downloads/professoxrmoriarty/yaklang/total.svg"/></a>
  <a href="https://github.com/professoxrmoriarty/yaklang/blob/main/LICENSE.md"><img alt="License" src="https://img.shields.io/badge/license-AGPL%20v3-%23ff7d23.svg"/></a>
  <a href="https://yaklang.com"><img alt="Site" src="https://img.shields.io/badge/site-yaklang.com-%233399dd.svg"/></a>
</div>

---

## What is Yak Project?

**Yak Project is a widely-used open-source cybersecurity infrastructure.**

It is not a single tool, but a **complete technology ecosystem centered around the "CDSL-YAK Domain-Specific Programming Language", extending outwards to encompass a GUI platform, static analysis engine, security AI agent, Java toolchain, vulnerability range, and AI benchmark.** From the underlying virtual machine `YakVM`, Static Single Assignment `YAK SSA`, and vulnerability modeling language `SyntaxFlow`, to the top-level graphical tools used daily by security practitioners, Yak Project has engineered "security capability convergence" into a reusable foundation.

> "**Security Convergence is Inevitable**" — Yak's starting point is not to build another "Swiss Army Knife", but to build a foundational infrastructure that allows **security capabilities to be combined, reused, and distributed like building blocks.**
>
> "**Do the Hard and Right Things**" — Team Slogan.

**Key Metrics** (Continuously Updating):

| Dimension | Data |
| --- | --- |
| Core Language Repo Commits | 14,000+ times (as of 2026-07) |
| Yakit Desktop Client Commits | 8,400+ times |
| Historical Release Versions | 600+ tags |
| Community Contributors | 50+ people |
| Academic Guidance | School of Cyberspace Security, UESTC |
| Tech Achievement Evaluation | [2024 Sci-Tech Achievement Appraisal organized by China Institute of Communications (CIC)](https://rivers.chaitin.cn/blog/cqj629h0lnedo7thptf0) |
| Industry Tech Progress | [Selected as Top 10 Sci-Tech Progresses in Info-Communications 2023 by CIC](https://www.china-cic.cn/Detail/24/60/6085) |
| Industry Sci-Tech Award | [Won 1st Prize of CIC Sci-Tech Award in 2025](https://www.china-cic.cn/Detail/24/6900/6900) |

---

## CDSL-YAK: A Domain-Specific Programming Language Born for Cybersecurity

<p align="center">
  <strong>CDSL-YAK · Cybersecurity Domain Specific Language</strong><br/>
  <em>"Probably the most advanced domain-specific programming language (DSL) in the security field"</em>
</p>

**CDSL (Cybersecurity Domain Specific Language)** is the core concept proposed and practiced by the Yaklang team: Instead of repeatedly "reinventing the wheel of security tools" with general-purpose languages, it is better to directly tailor a **Turing-complete, strongly-typed + dynamically-typed programming language that supports both bytecode compilation and interpreted execution** specifically for security scenarios.

Yaklang is the first complete implementation of the CDSL concept, containing an entire set of self-developed compiler infrastructure:

| Compiler Component | Role |
| --- | --- |
| **CDSL Yaklang** | The Cybersecurity Domain-Specific Language body (Syntax / Type System / Runtime) |
| **YakVM** | Virtual Machine for the CDSL (Stack-based bytecode execution) |
| **YAK SSA** | Static analysis-friendly Static Single Assignment intermediate representation |
| **SyntaxFlow** | Syntax pattern matching DSL — Vulnerability feature code description language |
| **LSP / DSP Server** | Language Server Protocol + Debug Adapter Protocol Server (IDE-level development experience) |

**Why is CDSL more suitable for security than general-purpose languages?**

- ✅ **Concise**: Use the least amount of code to describe high-frequency security scenarios like port scanning, traffic hijacking, and fuzzing.
- ✅ **Easy to Use**: Script is capability, single binary, out-of-the-box, cross-compiled across macOS / Linux / Windows.
- ✅ **Flexible**: Supports hot-reloading and embedded execution; can be called as the "capability foundation" of other security products.
- ✅ **Maintainable**: Syntax defined by context-free grammar, IDE-friendly, facilitating long-term engineering.
- ✅ **Reliable**: Strong typing + SSA intermediate representation makes program analysis "inherently friendly".

> Technology Comparison: `Golang ≈ Yaklang ≥ JVM Based Lang >> Python`
>
> Yak's Goal: To become the **"Matlab"** of the security field, giving "hacker programming" its own domain mother tongue.

**CDSL Textbook Officially Published**: *CDSL-YAK Cybersecurity Domain-Specific Programming Language — From Introduction to Practice*

---

## Product Matrix

The Yak Project product matrix is centered around CDSL-YAK, covering five layers from bottom to top: Language, Platform, Engine, Agent, and Toolchains. Each external product is detailed below; open-source ecosystem projects are summarized at the end of the document.

### Yakit: Intelligent Interactive Penetration Testing Platform

Yakit is the core desktop platform of the Yak Project for security practitioners. Its core purpose is to allow security engineers to complete the full penetration testing chain—"Observing Traffic -> Modifying Packets -> Fuzzing -> Writing Scripts -> Installing Plugins"—within a single workbench, eliminating the need to constantly switch context between BurpSuite, terminals, editors, and script repositories. It solves three long-standing pain points in solo operations and team collaboration: **fragmented tools** leading to repeated context loss, **difficulty in accumulating capabilities** preventing experience reuse, and **excessive repetitive labor** causing similar operations to be rewritten every time. To this end, Yakit integrates capabilities such as MITM interactive hijacking, Web Fuzzer visual fuzzing, passive scanning, port scanning, web crawling, reverse connections, WebShell management, and AI Agents into an open-source, free, cross-platform client, with a built-in Yaklang runtime, allowing security actions to switch from "clicking buttons" to "writing code" at any time.

The underlying support for this complete capability is the **architectural advantage of Yak CDSL**. With CDSL-YAK as its core, Yakit integrates the runtime, debugging capabilities, and security engineering workflows of a language tailored for cybersecurity into the same graphical workbench. Because the core is a Turing-complete domain language rather than a fixed set of features, Yakit achieves "Script is Capability": Any corner case not covered by the GUI can be temporarily solved or solidified into a plugin using a piece of Yaklang script; any team's private methodology can be accumulated into reusable, distributable assets. This also makes Yakit the graphical best practice of Yaklang security capabilities—Graphical means efficiency, plugin-based means ecosystem, script-based means infinite extension.

| Item | Details |
| --- | --- |
| Positioning | Interactive Application Security Testing ALL-IN-ONE platform built on Electron + Yaklang gRPC engine |
| Open Source | First released on 2021-10-12, completely open-source and free |
| Repository | [github.com/professoxrmoriarty/yakit](https://github.com/professoxrmoriarty/yakit) |

#### Core Features

**1. Fluent MITM Hijacking, Packet Replay, and Fuzzing Workflow**

Yakit's MITM module is the core of interactive penetration, providing both manual hijacking/modification and automatic passive observation modes, combined with historical traffic tracing and visual Web Fuzzer to form a complete workflow: After hijacking a packet, you can view, edit, replay, batch process, and fuzz in the same interface. The workflow is smooth and efficient, requiring no context switching between multiple tools. Its unique fuzzing system allows Yakit to describe injection points via Fuzztag syntax; a single line of annotation can generate variants in batches and observe server behavior, making fuzzing visual and composable.

**2. Powerful Plugin Ecosystem and Community Support**

Yakit has a plugin system that runs through the entire penetration process. The plugin store has accumulated thousands of plugins covering various security scenarios, from general scanning and protocol processing to specialized detection, ready to use upon installation. Users can run and debug plugins locally, distribute and share them via the plugin store, and publish their own plugins to feed back into the community after review. An active user ecosystem has formed around the plugins and products; GitHub Issues handle bug feedback and capability co-construction, while community discussions and user mutual aid help practitioners quickly get started and accumulate methodologies.

**3. Powered by CDSL-Yak Engine, Hot-Reloading Solves Edge Cases**

Yakit incorporates the CDSL-Yak language engine and runtime, adopting hot-reloading technology: Users can dynamically load and execute Yaklang scripts at any stage of penetration, rewriting traffic and behavior in real-time without restarting the platform. This allows edge cases not covered by the GUI—traffic modification, signature repair, auth token recalculation, encryption/decryption preprocessing, custom protocol parsing—to be temporarily solved or solidified into plugins via scripting. Script is capability, hot-reloading is real-time effect; this is the fundamental difference between Yakit and fixed-feature tools.

**4. Completely Rewritten Core Libraries, Optimized for SM Algorithms, Extremely Compatible**

Yakit and the underlying Yaklang engine have completely rewritten core libraries, specifically optimized for key scenarios in practical cybersecurity, especially strengthening built-in support for Chinese cryptographic algorithms (SM2 / SM3 / SM4, etc.), codec chains, and protocol adaptations, meeting the encryption communication testing requirements in compliant environments. Meanwhile, Yakit is highly compatible, working consistently across macOS / Windows / Linux, and adapting to domestic OS like UOS and Kylin, fitting various deployment forms from solo operations to team collaboration and enterprise intranets.

### Yaklang: The Domain-Specific Programming Language for Cybersecurity

Yaklang is the core and starting point of the Yak Project, a domain-specific programming language designed exclusively for cybersecurity. Packaged as a single binary runtime, it encapsulates security capabilities such as port scanning, service scanning, MITM hijacking, HTTP fuzzing, encoding/decoding, reverse connections, and protocol parsing into built-in functions that can be called directly by scripts. Security practitioners can accomplish tasks that previously required assembling multiple tools with minimal code. In the Yak ecosystem, Yakit is the graphical platform, IRify is the code analysis system, and their driving core engine is Yaklang.

| Item | Details |
| --- | --- |
| Positioning | Cybersecurity Domain Specific Language (CDSL), a Turing-complete, strongly & dynamically typed language supporting both bytecode compilation and interpretation. |
| Repository | [github.com/professoxrmoriarty/yaklang](https://github.com/professoxrmoriarty/yaklang) |
| License | AGPL-3.0 |
| Form | Single binary, run scripts with `yak script.yak`, execute expressions with `yak -c 'expr'`, cross-compiled for macOS / Linux / Windows |
| Documentation | [/docs/intro](https://yaklang.com/docs/intro) |

#### What Problem It Solves

There has been a long-standing fragmentation in security R&D: The **development of security platforms** (using Golang/Java for engineering) and the **development of security capabilities** (writing PoCs, scanners, detection logics) are scattered across different languages and projects. To scan ports, a security engineer has to install nmap or call a Python library; to fuzz, they have to manually assemble HTTP variants; to write a PoC, they have to rewrite HTTP requests and codec logics every time. Everyone implements different solutions and fingerprint library standards, reinventing wheels, scattering security capabilities, making them un-reusable.

Yaklang's goal is to eliminate this fragmentation and assume the responsibility of "**Security Capability Convergence**". The official positioning is clear: "Our goal is to provide a 'one-stop' security capability foundation"—PoCs, scanners, scanning modules, and vulnerability scanning algorithms can all be built with it. As a DSL for the security domain, Yaklang has built-in massive security domain functions, making security capabilities directly part of the language itself, without relying on assembling external tools.

#### Language Features

**1. Script is Capability, Out-of-the-Box**

Yaklang scripts do not require a `main()` function or compilation steps; they run as soon as they are written. Distributed as a single binary, out-of-the-box, and can be cross-compiled across macOS / Linux / Windows. Low-level capabilities like SYN scanning only require libpcap (npcap on Windows) to be installed on the system. The language supports modern scripting features like `var` / `=` / `:=` variable declarations, f-string interpolation, `defer` / `recover()` exception handling, and `go func()` concurrency with WaitGroup synchronization. The syntax style is very friendly to developers with Go / Python experience.

**2. Built-in Massive Security Domain Function Library**

This is the core value of Yaklang as a DSL. The language has a built-in standard library covering the entire penetration process, eliminating the need for security engineers to search for and maintain third-party wheels:

- **Scanning**: `synscan` (SYN Port Scan), `servicescan` (Service Scan), `finscan`, `subdomain`, `spacengine` (Cyberspace Mapping Engines)
- **Traffic**: `mitm` (Man-in-the-Middle), `http` / `httpool` (HTTP requests and batching), `fuzz` (Fuzzing), `poc` (PoC packet sending)
- **Encoding/Decoding**: `codec` (Base64 / Hex / URL / SM2 / SM3 / SM4 encoding/decoding and cryptography)
- **Target Identification**: `fp` (Fingerprinting), `crawler` / `crawlerx` (Crawling), `brute` (Brute-forcing)
- **Infrastructure**: `dnslog` / `dns`, `csrf`, `pcapx` (PCAP parsing), `ja3`, `nuclei` (Nuclei template scanning compatibility)

A script of less than 30 lines can complete port scanning and service identification; a few lines of code can initiate an HTTP request and parse the response.

**3. Coexistence of Dynamic and Strong Typing, Dual-Mode Execution**

Yaklang is a dynamically typed language where variable types are inferred from assigned values, requiring no explicit declaration; at the static analysis level, it is supported by strong typing and SSA intermediate representation, making program analysis "inherently friendly". Scripts can be compiled into bytecode for stack execution via YakVM, or interpreted, balancing execution efficiency and development flexibility.

**4. Hot-Reloading and Embedded Execution**

Yaklang supports hot-reloading and embedded execution: Scripts can be dynamically loaded and executed at any stage of penetration (e.g., Yakit MITM hot-reloading packet modification), and can also be embedded as a security capability foundation to be called by other security products. Yaklang possesses the dual identity of an independent programming language and an orchestratable security capability runtime.

#### Architecture: The Five Compiler Components

Yaklang is a complete compiler infrastructure, consisting of five components from bottom to top:

| Compiler Component | Role |
| --- | --- |
| **CDSL Yaklang** | The Cybersecurity Domain-Specific Language body (Syntax / Type System / Runtime) |
| **YakVM** | Virtual Machine for the CDSL (Stack-based bytecode execution) |
| **YAK SSA** | Static analysis-friendly Static Single Assignment intermediate representation |
| **SyntaxFlow** | Syntax pattern matching DSL — Vulnerability feature code description language |
| **LSP / DSP Server** | Language Server Protocol + Debug Adapter Protocol Server (IDE-level development experience) |

Among them, YAK SSA and SyntaxFlow are the technical foundations for code security analysis (IRify). The LSP / DSP Server allows Yaklang to gain IDE-level development experiences like auto-completion, jump to definition, parameter hints, and syntax checking in the built-in Yak Runner of Yakit and the VSCode extension. This infrastructure supports Yaklang in becoming "the Matlab of the security field, giving hacker programming its own domain mother tongue".

#### Installation

```bash
# macOS / Linux One-Click Install
bash <(curl -sS -L https://github.com/professoxrmoriarty/yaklang/blob/english-edition/scripts/install-latest-yak.sh)

# Windows
powershell (new-object System.Net.WebClient).DownloadFile('https://github.com/professoxrmoriarty/yaklang/releases/download/v2026.10.31-engine-en/yak_windows_amd64.exe','yak_windows_amd64.exe') && yak_windows_amd64.exe install && del /f yak_windows_amd64.exe

# Verify Installation
yak version
