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

```

### IRify: Modern Code Security Analysis System Centered on SSA and AI

IRify is the modern analysis system for code security of the Yak Project. Its core consists of **two engines**: One is a **static analysis engine centered on Static Single Assignment (SSA) with the self-developed vulnerability description language SyntaxFlow as the query language**; the other is an **artificial intelligence engine structured around LLMs and Agent loops**. The two engines are independent and self-contained, capable of completing code security analysis on their own; at the same time, they empower each other and are deeply integrated. AI directly analyzes or verifies the static analysis results in SSA form, and plays a key role in the generation and maintenance of SyntaxFlow rules.

The SSA engine and AI engine are independent and self-contained; yet they are deeply integrated: AI directly analyzes or verifies the static analysis results in SSA form, and plays a key role in the generation and maintenance of SyntaxFlow rules.

The division of labor is clear: The SSA engine ensures results are reproducible, verifiable, and engineerable; the AI engine brings semantic understanding, planning/reasoning, and scaled coverage. The intersection of the two—AI directly analyzing/verifying SSA static results and AI generating/maintaining SyntaxFlow rules—is exactly what distinguishes IRify from any single-paradigm product.

As an independent product, IRify's official website is [ssa.to](https://ssa.to).

| Item | Details |
| --- | --- |
| Positioning | Modern code security analysis system centered on SSA and AI; the SSA engine and AI engine are independent yet deeply integrated. |
| Release Form | Online [ssa.to](https://ssa.to) · Yakit IRify Release (Community / Enterprise) |
| Supported Languages | Java / SpringBoot series, Golang, PHP, JavaScript / EcmaScript, Python, C; built based on standard eBNF g4 grammar files. |
| Site / Source | [ssa.to](https://ssa.to) · [professoxrmoriarty/yaklang/tree/main/common/yak/ssa](https://www.google.com/search?q=https://github.com/professoxrmoriarty/yaklang/tree/main/common/yak/ssa) · [professoxrmoriarty/yaklang/tree/main/common/syntaxflow](https://www.google.com/search?q=https://github.com/professoxrmoriarty/yaklang/tree/main/common/syntaxflow) · [SyntaxFlow Tutorial](https://www.google.com/search?q=https://github.com/professoxrmoriarty/syntaxflow) |

#### Core Features

**1. SSA Engine: Static Analysis with Static Single Assignment as Core and SyntaxFlow as Query Language**

The SSA engine is the reproducible foundation of IRify, adopting a two-stage architecture: The first step compiles multi-language source code into a unified Static-Single-Assignment (SSA) intermediate representation (IR) and saves it to a program database (supporting lazy loading and storing); the second step uses the self-developed SyntaxFlow to perform query-based scanning on the IR products. This "decoupled compilation and analysis" design allows the IR of large projects to be compiled once and reused multiple times, and compilation and analysis can be executed separately on different machines, avoiding re-parsing source code for every scan.

SSA intermediate representation is naturally friendly to program analysis: It achieves bi-directional data flow analysis via Φ (Phi) nodes, supports cross-package, cross-file global analysis and path-sensitive analysis, and can perform context-sensitive interprocedural analysis for closures. Combined with deep correlation analysis (data flow + control flow), the SSA engine can trace a complete path of data from an external input (source) to a dangerous function (sink), far exceeding the precision of isolated function name matching.

What makes this architecture "directly usable by security engineers" is **SyntaxFlow**, positioned as an "Advanced Declarative Pattern Query Language", which is essentially a **Vulnerability Description Language (VDL)—a domain language specifically used to describe vulnerability forms and align rules with auditing intuition**. Unlike CodeQL or Datalog, SyntaxFlow does not require importing various tables and libraries to describe operational characteristics. Its logic is closer to the human thought process in code auditing: Directly declare "what kind of code pattern constitutes a vulnerability", and the engine takes care of taint tracking and data flow querying on the IR.

A SyntaxFlow rule consists of three parts: Rule description (`desc`, including `title`, `type`, `level`, `risk`, `cve`, etc.), Rule content (query expression), and Rule output (`check` / `alert`). Rules are chained using operators like `#->`, `-->`, `#>` to define Use-Def Chains, use `#{include}` / `#{exclude}` / `#{until}` for filtering, and capture nodes with `as $var`. This syntax makes the rule the vulnerability model itself: readable, testable, and version-controllable. Relying on this determinism, the SSA engine independently undertakes the entire analysis process from rule to result, producing stable, reproducible, and traceable outputs without any model inference in the pipeline.

**2. AI Engine: Code Security Analysis Structured by LLMs and Agent Loops**

The AI engine is the semantic reasoning layer of IRify, capable of working independently of the SSA engine. Structured around ReAct Agent loops, it registers independent code security audit loop types within the Yaklang AI ecosystem. On the desktop, it is accessed through two Focus Modes: `code_security_audit` (Whole-project code security audit) and `ai_skill_audit` (AI Skill-driven analysis). A complete AI audit follows a four-stage process: Project exploration, scan planning & dual-stage auditing serialized by category, step-by-step verification & evidence recording, and report generation & fallback, ultimately exporting MD / PDF reports.

As an independent engine, the AI engine performs semantic understanding and security analysis directly on source code: identifying business logic flaws without preset rules, explaining code intent, and restoring attack paths across functions, covering semantic risks that are hard to describe with pure pattern matching. Such semantic risks are exactly the areas difficult to reach by the SSA engine's deterministic analysis driven by "Rule is Vulnerability Model", thus forming a complementary relationship between the two engines.

The AI engine also provides a complete chain from results to evidence: Audit conclusions can point to specific code locations and contexts, and gain stable capability boundaries through SyntaxFlow syntax, approx. 40 NativeCalls, and Source/Source→Sink templates injected by `irify-sast-skill` (MCP tool `yak mcp -t ssa`), featuring a fallback mechanism of "self-healing and retrying upon query syntax errors".

**3. Deep Integration of Dual Engines: AI Analyzes and Verifies SSA Static Results, Driving Rule Generation & Maintenance**

IRify's differentiator lies in the deep integration of the two engines: AI is tightly coupled with the SSA system across three pathways: direct analysis, verification, and rule engineering.

* **AI directly analyzes static analysis results in SSA form**: Using the IR produced by the SSA compiler and identified risk products as inputs, the AI audit directly analyzes and judges the static analysis results—confirming if it constitutes a real exploitable path, converging false positives, and supplementing semantic risk descriptions. The stable SSA product provides a reproducible factual foundation for AI, making AI's semantic judgments more accurate and stable.
* **AI verifies SSA static analysis results**: For candidate vulnerabilities produced by the SSA engine based on SyntaxFlow rules, AI steps in as a verifier, judging whether they are genuinely established and their exploitation difficulty based on context, outputting verification conclusions with evidence. This chain of "Rule Coarse Filtering + AI Verification" is the key to improving true positive rates and suppressing false positives.
* **AI drives SyntaxFlow rule generation and maintenance**: The Focus Mode `write_syntaxflow_rule` performs retrieval on built-in rule example knowledge bases (`syntaxflow-aikb` text search + `syntaxflow-aikb-rag` vector search). Combined with single-file editing toolchains and SyntaxFlow compilation validation, it iteratively writes valid `.sf` files. The AI beautifier shortcut (`sf_rule_completion` Forge) in the top right of the editor reformats an `.sf` text according to unified standards. The production and long-term maintenance of rules thus upgrade from "manual trial and error" to "AI drafting + syntax self-check + manual gatekeeping".

This route—"SSA engine provides reproducible static analysis and rule foundations, AI engine provides semantic understanding and verification reasoning, and the two couple deeply on both analysis and rule sides"—makes IRify possess the stability and engineerability of traditional SAST, as well as the semantic coverage and scaling capabilities of the AI era.

**4. Rule Debugging System and Scanning Stability Guarantee**

IRify provides a complete toolchain from writing and debugging to result verification, ensuring rules are engineerable.

* **Rule Editor**: `RuleEditorBox` based on Monaco, incorporating SyntaxFlow language specification (`SyntaxFlowMonacoSpec`), and capable of reverse-looking up the original `.sf` rule that triggered a specific result via `result_id` on the audit results page, making "Result ↔ Rule" bi-directionally traceable.
* **Rule Debugger**: Debugging sessions (`apiSyntaxFlowScan`) driven by `useRuleDebug`, supporting `pause` / `resume` / `stop` / `reset`, outputting matched node cards and logs step-by-step, facilitating authors to confirm match boundaries and false positive sources.
* **Rule Management**: An independent "Rule Management" page distinguishes local rules and online rules, supporting rule grouping, batch import/export, and selecting rule sets by group during code scanning. Default rule templates link directly to the [SyntaxFlow Guide](https://ssa.to/syntaxflow-guide/intro).
* **Traceable Results**: Every audited vulnerability (`SSARisk`) carries severity, code locations (`CodeSourceUrl` / `CodeRange` / `CodeFragment`), affiliated functions and variables, matched rules (`FromRule`), CVE / Risk Types, and remediation suggestions. The detail pane displays an interactive data flow graph; clicking nodes jumps to the source code and displays the SSA IR code side-by-side. The full path from "Dangerous Function to Vulnerability Point" is traceable and expandable.
* **Scanning Stability**: Scanning tasks possess a complete lifecycle API (`StartScan` / `ResumeScan` / `GetScanStatus`), supporting resumable scanning and status querying. On the rule side, stable SSA scanning products support unstable AI auditing, aiming for "multiple audits of the same project to yield highly consistent outputs". Report generation (MD / PDF) makes results accumulable and reviewable.

The volume of built-in rules also supports this stability: The yaklang engine embeds **364 `.sf` rules** via `go:embed`, among which 363 are distributed across Java (154, incl. Spring), Golang (103), PHP (42), Python (26), JavaScript/EcmaScript (21), and C (17) language directories, plus 1 general rule. These rules span 130 language-specific CWE directories, covering 67 unique CWE IDs, and carry IRify-exclusive exclusion policies (`rules_irify_exclude.go`).

---

## Memfit AI: Desktop AI Agent for Security Engineers

Memfit AI is the desktop AI Agent developed by the Yak Project for the cybersecurity domain, mainly addressing the practical problems of security engineers in information organization, traffic analysis, vulnerability research, code auditing, automated execution, and report writing. The product prioritizes adaptation for cybersecurity workflows while providing general Agent capabilities such as file processing, knowledge retrieval, task planning, tool invocation, and result delivery, which can also be used for research, analysis, and daily automated tasks.

The core code of Memfit AI is located at [professoxrmoriarty/yaklang/tree/main/common/ai/aid](https://www.google.com/search?q=https://github.com/professoxrmoriarty/yaklang/tree/main/common/ai/aid). The desktop client is developed from the same infrastructure as Yakit, with the AI engine and tool system reusing the Yaklang language ecosystem. Existing capabilities of Yaklang such as HTTP, MITM, fuzzing, port and fingerprint identification, codec, vulnerability verification, and code auditing can be directly provided to the Agent. YakScript, Yakit Plugins, and MCP services can also be integrated per task to handle security scenarios difficult for general Agents to cover.

| Dimension | Memfit AI |
| --- | --- |
| Product Positioning | A vertical desktop AI Agent aimed at the full workflow of security engineers, while possessing general task capabilities. |
| Workflow | Goal -> Plan / Task Graph -> Tool Invocation -> Manual Review -> Deliverable |
| Context Inputs | Structured resources like local files, directories, images, knowledge bases, HTTP Flows, Web Fuzzer requests, etc. |
| Accumulable Assets | Knowledge Bases, Long-Term Memory, AI Skills (Forge), Tools, Focus Modes |
| Core Code | [professoxrmoriarty/yaklang/tree/main/common/ai/aid](https://www.google.com/search?q=https://github.com/professoxrmoriarty/yaklang/tree/main/common/ai/aid) |
| Extension Capabilities | Yaklang / YakScript Tools, Yakit Plugins, Security Analysis Capabilities, and MCP Services |
| Risk Control | File operation permissions, Manual / AI / Fully-auto review modes, Tool risk thresholds, Traceable task processes |

### Core Features

#### 1. Complete Workflow Oriented to Security Engineers

Memfit AI can process security data like HTTP Flows, Web Fuzzer requests, code projects, vulnerability evidence, and scan results, as well as ordinary files and directories. Security engineers can complete data reading, analysis and judgment, tool verification, and report output in the same task, reducing context switching between chat tools, terminals, scripts, and documents. The product also retains general Agent capabilities, making it usable for research and automation tasks outside of security work.

#### 2. Reusing Yaklang and Yakit Ecosystems

Memfit AI's AI engine, tool system, and security capabilities share code and runtime with Yaklang. Yaklang built-in libraries, YakScript scripts, and Yakit plugins can be used as Agent tools, so existing security capabilities do not need redevelopment. For scenarios like dynamic signatures, auth token recalculation, private protocols, special encoding, and traffic rewriting, processing logic can be supplemented via Yaklang scripts.

#### 3. Supports Complex Task Execution and Process Control

Memfit AI breaks down goals into plans and specific tasks, calling tools, reading resources, and generating results according to dependencies. Plans, tool parameters, execution results, and deliverables are recorded in a unified timeline, allowing users to view the task process and intervene when necessary. Tool invocation supports manual confirmation, AI judgment, and automatic execution, with configurable file permissions, risk thresholds, and disabled tools.

#### 4. Work Materials and Methods Can Be Reused

Knowledge Bases are used to manage verifiable materials; Long-Term Memory saves stable preferences, project constraints, and work experience; AI Skills (Forge) define task flows and output requirements. Tools, skills, knowledge, and memory can be combined per task and continue to be used in subsequent sessions. Model services are independent of these work assets; changing models will not affect already saved materials and processes.

> **Security Prompt**: Capabilities like port probing, HTTP testing, and vulnerability verification should only be used within clearly authorized scopes; official demos uniformly use local services, sanitized traffic, or dedicated test environments.

---

## Open Source Projects

Besides Yaklang, Yakit, IRify, and Memfit AI, the Yak Project also maintains a group of open-source projects geared towards security R&D, AI Agents, code analysis, and engineering delivery. These projects include installable Agent Skills, training & retrieval materials, benchmarking tools, independent modules within the Yaklang repository, command-line programs, and cross-platform infrastructure. Independent projects link to their repository roots; projects located in the Yaklang monorepo link directly to their source directories. The following content is organized according to the "Project Introduction, Core Value, Link Address" required by the official website's gallery cards.

### Agent Skills and Knowledge Assets

| Project | Introduction | Core Value | Project Link |
| --- | --- | --- | --- |
| **Yak Skills** | Yaklang programming, Yakit usage, and hot-reloading knowledge bases geared for AI Agents, with each topic accompanied by runnable `.yak` examples and verification tools. | Enables Agents to write, debug, and verify Yaklang scripts, and handle practical scenarios like MITM, Web Fuzzer, and global hot-reloading. | [GitHub](https://www.google.com/search?q=https://github.com/professoxrmoriarty/yak-skills) · [Online Browse](https://skills.yaklang.io) |
| **HackSkills** | Attack and defense skill base geared for AI Agents, covering Web, API, Auth, Privilege Escalation, Reverse Engineering, Crypto, and AI Security. | Organizes security knowledge into installable, searchable, and composable standard Skills, facilitating Agents to load them on demand during authorized testing and research. | [GitHub](https://www.google.com/search?q=https://github.com/professoxrmoriarty/hack-skills) · [Online Browse](https://skills.hackbenchmark.com) |
| **IRify SAST Skill** | Encapsulates IRify's SSA compiler and SyntaxFlow querying capabilities as an AI Agent Skill, supporting Java, PHP, JavaScript, Go, Python, C, and Yak. | Empowers Agents like Codex, Claude Code, and Cursor to compile source code, trace data flows, and execute static security analysis. | [GitHub](https://www.google.com/search?q=https://github.com/professoxrmoriarty/irify-sast-skill) |
| **Control Theory Skill** | Organizes concepts from cybernetics, systems theory, and information theory—such as feedback, stability, and black-box experimentation—into Agent design methodologies. | Provides reusable analytical frameworks for task planning, tool usage, error correction, and feedback loop design. | [GitHub](https://www.google.com/search?q=https://github.com/professoxrmoriarty/control-theory-skill) |
| **Yaklang AI Training Materials** | AI knowledge and example material base for Yaklang, including standard library usage, practical cases, articles, scripts, and benchmark materials. | Provides structural references for Agents to learn Yaklang, generate security scripts, and retrieve language usage. | [GitHub](https://www.google.com/search?q=https://github.com/professoxrmoriarty/yaklang-ai-training-materials) |
| **SyntaxFlow AI Training Materials** | Materials for SyntaxFlow syntax, operators, NativeCalls, rule examples, error handling, and RAG construction. | Supports AI in retrieving SyntaxFlow knowledge, generating rules, and completing syntax self-checks and iterative corrections. | [GitHub](https://www.google.com/search?q=https://github.com/professoxrmoriarty/syntaxflow-ai-training-materials) |

### Benchmarking, Code Analysis, and Security Research

| Project | Introduction | Core Value | Project Link |
| --- | --- | --- | --- |
| **IRify Benchmark** | Lightweight benchmarking framework for code scanning engines, maintaining baseline projects annotated with Source, Sanitizer, and Sink data flows. | Evaluates scanning engines based on complete data flows rather than single hit lines; usable for regression testing, CI, and engine comparisons. | [GitHub](https://www.google.com/search?q=https://github.com/professoxrmoriarty/irify-benchmark) |
| **SyntaxFlow Tutorial** | Tutorials and example projects from Intro to Practice for SyntaxFlow, covering SSA queries, Use-Def chains, interprocedural analysis, and data flow visualization. | Helps security engineers learn to describe vulnerabilities using declarative rules and understand IRify's static analysis methods. | [GitHub](https://www.google.com/search?q=https://github.com/professoxrmoriarty/syntaxflow) |

### Independent Modules within the Yaklang Repository

| Project | Introduction | Core Value | Project Link |
| --- | --- | --- | --- |
| **Yaklang AI Agent Runtime** | The Agent runtime used by Memfit AI, including Plan & Task Graph, ReAct Loop, Tool System, Long-Term Memory, Execution Review, and specialized Focus Modes. | Provides a unified Agent orchestration and security tool execution foundation for the Yaklang ecosystem. | [professoxrmoriarty/yaklang/tree/main/common/ai/aid](https://www.google.com/search?q=https://github.com/professoxrmoriarty/yaklang/tree/main/common/ai/aid) |
| **Yak SSA** | Yaklang's SSA intermediate representation and core program analysis, including instruction models, basic blocks, control flow, Phi, scope, and program database. | Provides a unified program representation for multi-language code modeling, data flow analysis, and IRify static analysis. | [professoxrmoriarty/yaklang/tree/main/common/yak/ssa](https://www.google.com/search?q=https://github.com/professoxrmoriarty/yaklang/tree/main/common/yak/ssa) |
| **SyntaxFlow Engine** | SyntaxFlow's syntax, virtual machine, built-in rules, database, autocompletion, and scan task implementations. | Compiles security rules into executable queries to perform pattern matching and data flow analysis on SSA programs. | [professoxrmoriarty/yaklang/tree/main/common/syntaxflow](https://www.google.com/search?q=https://github.com/professoxrmoriarty/yaklang/tree/main/common/syntaxflow) |
| **MiniREHS** | Zero external dependency, portable multi-regex batch matching engine, adopting unified compilation, one-pass scanning, and candidate verification. | Aimed at batch matching scenarios with massive rules and network traffic, maintaining consistent results between pure Go and optional bundled SIMD backends. | [professoxrmoriarty/yaklang/tree/main/common/minirehs](https://www.google.com/search?q=https://github.com/professoxrmoriarty/yaklang/tree/main/common/minirehs) |
| **Yak SCA Engine** | Software Composition Analysis module, including dependency file parsers and license analysis for Java, Go, Node.js, Python, PHP, Ruby, Rust, and C/C++. | Provides a unified foundation for dependency identification, SBOM, license checking, and supply chain risk analysis. | [professoxrmoriarty/yaklang/tree/main/common/sca](https://www.google.com/search?q=https://github.com/professoxrmoriarty/yaklang/tree/main/common/sca) |
| **Vulinbox** | Web vulnerability target range built into Yaklang, providing reproducible instances of SQLi, XSS, SSRF, File Upload, Logic flaws, and Component vulnerabilities. | Provides local authorized targets for Yakit hands-on practice, plugin validation, AI Agent security evaluation, and teaching. | [professoxrmoriarty/yaklang/tree/main/common/vulinbox](https://www.google.com/search?q=https://github.com/professoxrmoriarty/yaklang/tree/main/common/vulinbox) · [Practical Manual](https://yaklang.com/Yaklab/vulinbox/) |

### Independent Tools and Engineering Infrastructure

| Project | Introduction | Core Value | Project Link |
| --- | --- | --- | --- |
| **JavaJive** | A pure Go Java toolbox extracted from Yaklang, supporting `.class`, `.jar`, `.war` decompilation, class structure parsing, and Java serialization to JSON bidirectional conversion. | Requires no JDK, cgo, or native runtimes; usable as a single binary tool or embeddable into other Go projects. | [GitHub](https://www.google.com/search?q=https://github.com/professoxrmoriarty/javajive) · [Project Site](https://yaklang.io/javajive/) |
| **go-llvm** | Go bindings for the LLVM 18 C API, compatible with static and dynamic linking, and providing JIT-related interfaces. | Provides a portable, self-contained LLVM integration method for the Yaklang ecosystem, lowering runtime environment dependencies on system LLVM. | [GitHub](https://www.google.com/search?q=https://github.com/professoxrmoriarty/go-llvm) |
| **Memfit CLI** | Terminal Agent client connecting to the Yaklang AI HTTP Gateway, supporting session creation, SSE event streams, model settings, review policies, and task cancellation. | Brings Memfit AI's interactive task execution capabilities to the terminal, facilitating automated workflows and remote Agent debugging. | [GitHub](https://www.google.com/search?q=https://github.com/professoxrmoriarty/yaklang-memfit-cli) |
| **Awesome Yak Scripts** | Collection of Yak scripts covering security tools, dependency sync, SCA rule generation, log analysis, and plugin maintenance. | Provides Yaklang automation examples that can be directly read, run, and modified. | [GitHub](https://github.com/professoxrmoriarty/awesome-yak-scripts) |
| **Yaklang VS Code Extension** | VS Code extension for Yaklang and SyntaxFlow, providing syntax highlighting, completion, parameter hints, diagnostics, debugging, and quick run. | Brings Yaklang's LSP, DSP, and engine management capabilities into general code editors. | [GitHub](https://www.google.com/search?q=https://github.com/professoxrmoriarty/yaklang-support) · [Extension Market](https://marketplace.visualstudio.com/items?itemName=v1ll4n.yak) |
| **Yakit Chrome Extension** | Chrome extension for browser proxy switching and Yakit linkage. | Simplifies switching between browsers, system proxies, and Yakit, providing a browser-side entry point for Web security testing. | [GitHub](https://www.google.com/search?q=https://github.com/professoxrmoriarty/yaklang-chrome-extension) |
| **pcap** | An engineered fork separated from `gopacket/pcap`, retaining Go packet capture interfaces and incorporating libpcap headers, static libs, and dynamic libs by version and architecture into the repository. | Resolves system libpcap version discrepancies, cross-compilation, and domestic architecture adaptation issues, providing a stable dependency for Yaklang's packet capture, scanning, and networking capabilities. | [GitHub](https://www.google.com/search?q=https://github.com/professoxrmoriarty/pcap) |

#### pcap Fork Work and Completion Status

The goal of `professoxrmoriarty/pcap` is to improve the controllability of `gopacket/pcap` in security product building and distribution. Key changes include:

* **Locking libpcap dependencies**: The repository carries headers and build artifacts for libpcap 1.8.1, 1.9.1, and 1.10.4, selecting fixed versions for different architectures via [`pcap_linux.go`](https://www.google.com/search?q=https://github.com/professoxrmoriarty/pcap/blob/main/pcap_linux.go). Build environments do not require pre-installing corresponding system libpcap dev packages.
* **Handling system compatibility issues**: Linux amd64 uses libpcap 1.8.1 to handle segmentation faults in legacy CentOS environments; other architectures use fixed libpcap versions, reducing build and runtime deviations caused by system library differences.
* **Expanding architecture support**: libpcap build artifacts and cgo configurations have been provided for Linux amd64, arm64, loong64, and sw64; Windows side has struct definitions and compilation pre-support for 386, amd64, and arm64.
* **Following the Go network package ecosystem**: Dependencies have been migrated to the maintained `github.com/gopacket/gopacket v1.3.1`, while retaining pcap, BPF, and pcapng test samples and basic build checks.

This fork has been adopted as an official dependency of Yaklang, applied in modules like `pcapx`, SYN / FIN scanning, user-space network stacks, traffic injection, and tunnel triggering. Current achievements are mainly reflected in cross-architecture builds, dependency locking, and compatibility; the repository has not yet published performance comparison data with upstream, thus it is not described as a performance-optimized version.

---

## Project Milestones

Starting from the practical work of security engineers, the Yak Project has gradually formed an open-source product ecosystem with Yaklang as its technical foundation, covering interactive security testing, code auditing, and AI Agents. The following milestones record the public releases, technical development, and phased achievements of the core projects.

| Year | Event | Impact | Related Materials |
| --- | --- | --- | --- |
| **2021** | Yak and Yakit released at XCon | Yak Project entered the public development stage; Yakit began providing a unified desktop workbench for security engineers. | [XCon Release Record](https://www.sohu.com/a/567305083_120846244) |
| **2023** | CDSL-YAK held Open Source Launch Event at China National Convention Center | The core language, runtime, and security capability foundation were opened to the community, allowing external developers to inspect source code, submit issues, and participate in building. | [Open Source Event Record](https://www.cnblogs.com/yaklang/articles/17461795.html) |
| **2023** | YAKIT Cybersecurity Solo Testing System V2.0 selected in the 17th batch of Beijing New Technologies and New Products (Services) list | The productization and practical application of Yakit entered a new development stage. | [Beijing Official List PDF](https://kw.beijing.gov.cn/zwfw/bsjg/202307/P020240909007888758167.pdf) |
| **2024** | Yakit V2.0 passed the Third Research Institute of Ministry of Public Security testing | Yakit completed testing in accordance with relevant national standards for specialized cybersecurity products and Web application security testing. | [Testing Info Release Record](https://mp.weixin.qq.com/s?__biz=MzIwMzI1MDg2Mg==&mid=2649944674&idx=1&sn=bb61768ac951be7656caf3d6f58794dd) |
| **2024** | "Innovation and Application of YakLang, a Dedicated Security Programming Language for Communication Networks" selected as Top 10 Sci-Tech Progresses in Info-Communications 2023 | The dedicated programming language route of Yaklang entered the annual list of sci-tech progresses in the info-communications field. | [CIC Publication Page](https://www.china-cic.cn/Detail/24/60/6085) |
| **2025** | IRify released publicly | Yak SSA, SyntaxFlow, and AI capabilities formed an independent code auditing product, expanding project capabilities from interactive testing to source code security analysis. | [IRify Release Record](https://yaklang.com/en/blog/sql-injection-detection-with-irify/) |
| **2025** | "Technology and Application of Dedicated Programming Language and Development Environment for Cybersecurity" won 1st Prize of CIC Sci-Tech Award | The technological achievements and practical applications of Yaklang and its accompanying dev environment received industry sci-tech awards. | [CIC Award Announcement](https://www.china-cic.cn/Detail/24/6900/6900) |
| **2025** | "Domestic Cybersecurity Development Environment YAK" won 3rd Prize (Enterprise Group) at the "Maker China" National Finals | YAK advanced from the cybersecurity special contest to the national finals, demonstrating the engineering capability and application value of domestic security dev environments. | [National Finals Results PDF](https://www.miitxxzx.org.cn/module/download/downfile.jsp?classid=0&filename=4920ee41e78c447ca39295aeae07e019.pdf&showname=%E7%AC%AC%E5%8D%81%E5%B1%8A%E2%80%9C%E5%88%9B%E5%AE%A2%E4%B8%AD%E5%9B%BD%E2%80%9D%E4%B8%AD%E5%B0%8F%E4%BC%81%E4%B8%9A%E5%88%9B%E6%96%B0%E5%88%9B%E4%B8%9A%E5%A4%A7%E8%B5%9B%E5%85%A8%E5%9B%BD%E6%80%BB%E5%86%B3%E8%B5%9B%E8%8E%B7%E5%A5%96%E5%90%8D%E5%8D%95.pdf) |
| **2026** | Memfit AI released publicly | Yaklang, Yakit, and their tool ecosystems entered Agent workflows, providing analysis, execution, and delivery support for security engineers. | [Memfit AI Release Record](https://www.yaklang.com/en/blog/memfit-autonomous-pentest-agent-architecture/) |

[View the full development history](https://www.google.com/search?q=./materials/project-credibility/full-history.md)

```

```
yak version
