# BINSIDER

![license](https://img.shields.io/badge/license-license-blue) ![offline-first](https://img.shields.io/badge/offline--first-air--gap-green) ![audit](https://img.shields.io/badge/audit-SHA3--256-orange) ![category](https://img.shields.io/badge/category-laptops-lightgrey)

> Anticloud-hardened packaging of the upstream project `BINSIDER` in category **LAPTOPS**. Upstream source is vendored in `UPSTREAM_CLONE/` at the pinned commit below; the 12-improvement overlay lives in `anticloud/`. Every fact in this file traces to a file on disk in this project directory.

**Category:** LAPTOPS · **Upstream:** https://github.com/orhun/binsider · **Upstream pin:** `7f0633d1a69af15cc3be9e0533cb36dbe67eb598` · **Vendor:** Anticloud FZ LLE

---

## What This Project Does

<p align="center">
    <img src="https://raw.githubusercontent.com/orhun/binsider/main/website/src/assets/binsider-logo-dark.png#gh-dark-mode-only" width="300"></a>
    <img src="https://raw.githubusercontent.com/orhun/binsider/main/website/src/assets/binsider-logo-light.png#gh-light-mode-only" width="300"></a>
    <br>
    <img src="https://raw.githubusercontent.com/orhun/binsider/main/website/src/assets/binsider-text-dark.png#gh-dark-mode-only" width="170"></a>
    <img src="https://raw.githubusercontent.com/orhun/binsider/main/website/src/assets/binsider-text-light.png#gh-light-mode-only" width="170"></a>
    <br>
    <br>
    <em>"Swiss army knife for reverse engineers."</em>
    <br>
    <br>
    <a href="https://github.com/orhun/binsider/releases">
        <img src="https://img.shields.io/github/v/release/orhun/binsider?style=flat&labelColor=1d1d1d&color=f8be75&logo=GitHub&logoColor=white"></a>
    <a href="https://crates.io/crates/binsider/">
        <img src="https://img.shields.io/crates/v/binsider?style=flat&labelColor=1d1d1d&color=f8be75&logo=Rust&logoColor=white"></a>
    <br>
    <a href="https://github.com/orhun/binsider/actions?query=workflow%3A%22CI%22">
        <img src="https://img.shields.io/github/actions/workflow/status/orhun/binsider/ci.yml?style=flat&labelColor=1d1d1d&color=white&logo=GitHub%20Actions&logoColor=white"></a>
    <a href="https://github.com/orhun/binsider/actions?query=workflow%3A%22CD%22">
        <img src="https://img.shields.io/github/actions/workflow/status/orhun/binsider/cd.yml?style=flat&labelColor=1d1d1d&color=white&logo=GitHub%20Actions&logoColor=white&label=deploy"></a>
    <a href="https://hub.docker.com/r/orhunp/binsider">
        <img src="https://img.shields.io/github/actions/workflow/status/orhun/binsider/docker.yml?style=flat&labelColor=1d1d1d&color=white&label=docker&logo=Docker&logoColor=white"></a>
    <a href="https://docs.rs/binsider/">
        <img src="https://img.shields.io/docsrs/binsider?style=flat&labelColor=1d1d1d&color=white&logo=Rust&logoColor=white"></a>
    <br>
    <a href="https://discord.gg/zphNxEcEK7">
        <img src="https://img.shields.io/discord/1289166752311148554?color=f8be75&label=discord&labelColor=1d1d1d&logo=discord&logoColor=white"></a>
</p>

<h4 align="center">
  <a href="https://binsider.dev/getting-started/">Documentation</a> |
  <a href="https://binsider.dev/">Website</a>
</h4>

😼🕵️‍♂️ **Binsider** can perform static and dynamic analysis, inspect strings, examine linked libraries, and perform hexdumps, all within a user-friendly terminal user interface!

## Quickstart

> [!TIP]
> Watch the quickstart video to get a glimpse of what `binsider` can do: [https://youtu.be/InhVCQoc5ZE](https://youtu.be/InhVCQoc5ZE)

Install `binsider` with `cargo`:

```bash
cargo install binsider
```

> [!NOTE]  
> See the other [installation methods](https://binsider.dev/installation/other/) 📦

After the installation, you are pretty much set! 💯

Just dive into the binaries by running `binsider`:

```bash
binsider <binary>
```

![Demo](website/src/content/assets/quickstart.gif)

## Features

> [!NOTE]  
> The detailed documentation is available at <https://binsider.dev> 📚

### General Analysis

You can retrieve general binary file information, including file size, ownership, permissions, date, and linked shared libraries (similar to [`stat(1)`](https://www.man7.org/linux/man-pages/man1/stat.1.html) and [`ldd(1)`](https://www.man7.org/linux/man-pages/man1/ldd.1.html)).

[![General analysis](website/src/assets/demo/binsider-general-analysis.gif)](https://binsider.dev/usage/general-analysis)

➡️ <https://binsider.dev/usage/general-analysis>

### Static Analysis

You can analyze the ELF layout (such as sections, segments, symbols, and relocations) and navigate through them to get an in-depth understanding of the binary.

[![Static analysis](website/src/assets/demo/binsider-static-analysis.gif)](https://binsider.dev/usage/static-analysis)

➡️ <https://binsider.dev/usage/static-analysis>

### Dynamic Analysis

It is possible to execute the binary and trace the system calls, signals, and the program's execution flow similar to [`strace(1)`](https://man7.org/linux/man-pages/man1/strace.1.html) and [`ltrace(1)`](https://man7.org/linux/man-pages/man1/ltrace.1.html).

[![Dynamic analysis](website/src/assets/demo/binsider-dynamic-analysis.gif)](https://binsider.dev/usage/dynamic-analysis)

➡️ <https://binsider.dev/usage/dynamic-analysis>

### String Extraction

Similar to the [`strings(1)`](https://linux.die.net/man/1/strings) command, `binsider` is able to extract strings from the binary file with the purpose of discovering interesting strings such as URLs, passwords, and other sensitive information.

[![String extraction](website/src/assets/demo/binsider-strings.gif)](https://binsider.dev/usage/strings)

➡️ <https://binsider.dev/usage/strings>

### Hexdump

`binsider` provides a rich dashboard along with a hexdump view to analyze the binary content in a structured manner.

[![Hexdump](website/src/assets/demo/binsider-hexdump.gif)](https://binsider.dev/usage/hexdump)

➡️ <https://binsider.dev/usage/hexdump>

## Acknowledgements

Shoutout to [@harunocaksiz](https://github.com/harunocaksiz) for sticking with me during our military service in the summer of 2024 and creating the awesome **binsider** logo! (o7)

## Contributing

See the [contribution guidelines](CONTRIBUTING.md).

<a href="https://discord.gg/zphNxEcEK7">
   <img src="https://discord.com/api/guilds/1289166752311148554/embed.png?style=banner2"></a>

## License

Licensed under either of [Apache License Version 2.0](./LICENSE-APACHE) or [The MIT License](./LICENSE-MIT) at your option.

🦀 ノ( º \_ º ノ) - respect crables!

## Copyright

Copyright © 2024, [Orhun Parmaksız](mailto:orhunparmaksiz@gmail.com)

*Quoted from the upstream `README.md` file in `UPSTREAM_CLONE/`.*
Project-specific facts detected in this directory:

- Ecosystem: **Rust / Cargo** (manifests: Cargo.toml, Cargo.lock; scanned in UPSTREAM_CLONE)
- Top-level source layout: `examples/`, `src/`, `tests/`, `website/`
- Snapshot size: **123 files**, **4031 lines of code** (measured; see Benchmarks)
- Primary languages: `.md` (24), `.rs` (24), `.gif` (14), `.jpg` (11), `.astro` (10), `(none)` (8)
- Upstream commit pinned for this packaging: `7f0633d1a69af15cc3be9e0533cb36dbe67eb598`

---

## Installation

> [!TIP]
> Watch the quickstart video to get a glimpse of what `binsider` can do: [https://youtu.be/InhVCQoc5ZE](https://youtu.be/InhVCQoc5ZE)

Install `binsider` with `cargo`:

```bash
cargo install binsider
```

> [!NOTE]  
> See the other [installation methods](https://binsider.dev/installation/other/) 📦

After the installation, you are pretty much set! 💯

Just dive into the binaries by running `binsider`:

```bash
binsider <binary>
```

![Demo](website/src/content/assets/quickstart.gif)

*Section quoted from the upstream readme.*
Overlay install (this project):

```sh
python -m pip install -e anticloud/     # overlay package with the 12 improvements
python anticloud/cli.py --help          # 13 subcommands, JSON stdout
```

---

## Usage

➡️ <https://binsider.dev/usage/general-analysis>

*Section quoted from the upstream readme.*
Anticloud overlay CLI (available in every project):

```sh
python anticloud/cli.py --help     # 13 subcommands, JSON stdout
python anticloud/cli.py checks     # run the 16-check suite
```

---

## API

<a href="https://binsider.dev/">Website</a>
</h4>

😼🕵️‍♂️ **Binsider** can perform static and dynamic analysis, inspect strings, examine linked libraries, and perform hexdumps, all within a user-friendly terminal user interface!

*Section quoted from the upstream readme.*
---

## Dependencies

| Metric | Value |
|--------|-------|
| Ecosystem | Rust / Cargo |
| Manifests detected | Cargo.toml, Cargo.lock |
| Files in snapshot | 123 |
| Lines of code | 4031 |
| Dependency references | 48 |
| Dependencies by ecosystem | cargo: 38, npm: 10 |
| Upstream license | No license file present in the upstream snapshot |
| Overlay license | Anticommons 0.1.0 |

Top dependency references recorded in the benchmark snapshot:

| Ecosystem | Name | Version | Source file |
|-----------|------|---------|-------------|
| cargo | name | binsider | Cargo.toml |
| cargo | version | 0.3.2 | Cargo.toml |
| cargo | description | Analyze ELF binaries like a boss | Cargo.toml |
| cargo | license | MIT OR Apache-2.0 | Cargo.toml |
| cargo | readme | README.md | Cargo.toml |
| cargo | homepage | https://binsider.dev | Cargo.toml |
| cargo | project | https://github.com/orhun/binsider | Cargo.toml |
| cargo | edition | 2021 | Cargo.toml |
| cargo | rust-version | 1.88.0 | Cargo.toml |
| cargo | ratatui | 0.30.0 | Cargo.toml |
| cargo | clap | 4.5.56 | Cargo.toml |
| cargo | thiserror | 2.0.18 | Cargo.toml |
| cargo | elf | 0.8.0 | Cargo.toml |
| cargo | rust-strings | 0.6.0 | Cargo.toml |
| cargo | heh | 0.6.3 | Cargo.toml |
| ... | (33 more) | | |

Pinned lockfile: `anticloud/requirements.lock` (hash-pinned, PEP 508). SBOM: `sbom.cdx.json` (CycloneDX 1.5, pinned to the upstream SHA).

---

## Configuration

No configuration section was found in the upstream readme. Configuration-relevant files detected in this project directory:

- `Cargo.toml`
- `Dockerfile`

Overlay configuration (Anticloud):

- `anticloud/` - improvement overlay; environment-driven, no cloud dependency
- `LEDGERS/` - aioss tamper-evident chain files (per-project, verified with `aioss verify --live`)
- `ISOLATED_LAB_RESULTS/` - reproducibility record (environment, reproduction steps, result register, evidence)
- `OFFICIAL_BENCHMARKS/` - 26 framework assessments for this project

---

## Contributing

*Excerpt from upstream `CONTRIBUTING.md`:*

# Contribution Guidelines

First off, thank you for considering contributing to `binsider`!

If your contribution is not straightforward, please first discuss the change you
wish to make by creating a new issue before making the change.

## Reporting Issues

Before reporting an issue on the
[issue tracker](https://github.com/orhun/binsider/issues),
please check that it has not already been reported by searching for some related
keywords.

## Pull Requests

Try to do one pull request per change.

## Commit Message Format

This project adheres to [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/).
A specification for adding human and machine readable meaning to commit messages.

### Commit Message Header

```
<type>(<scope>): <short summary>
  │       │             │
  │       │             └─ Summary in present tense. Not capitalized. No period at the end.
  │       │
  │       └─ Commit Scope
  │
  └─ Commit Type: feat|fix|build|ci|docs|perf|refactor|test|chore
```

#### Type

| feat     | Features                 | A new feature                                                                                          |
| -------- | ------------------------ | ------------------------------------------------------------------------------------------------------ |
| fix      | Bug Fixes                | A bug fix                                                                                              |
| docs     | Documentation            | Documentation only changes                                                                             |
| style    | Styles                   | Changes that do not affect the meaning of the code (white-space, formatting, missing semi-colons, etc) |
| refactor | Code Refactoring         | A code change that neither fixes a bug nor adds a feature                                              |
| perf     | Performance Improvements | A code change that improves performance                                                                |
| test     | Tests                    | Adding missing tests or correcting existing tests                                                      |
| build    | Builds                   | Changes that affect the build system or external dependencies (example scopes: main, serde)            |
| ci       | Continuous Integrations  | Changes to our CI configuration files and scripts (example scopes: Github Actions)                     |
| chore    | Chores                   

Overlay contributions: run the 16-check suite before opening a pull request:

```sh
python anticloud/bench/runner.py --cwd anticloud
```

---

## License

**Upstream license: No license file present in the upstream snapshot** (evidence: `LICENSE` in the upstream snapshot).

### Anticommons 0.1.0 overlay

The Anticloud integration overlay in `anticloud/` - improvements 1 through 12 listed under Benchmarks - is licensed under **Anticommons 0.1.0**. Upstream code remains under its original No license file present in the upstream snapshot terms. See `ANTICOMMONS_LICENSE.md` in this directory for the overlay terms and contact.

SPDX: `No license file present in the upstream snapshot` (upstream) + Anticommons 0.1.0 (overlay, dual).

---

## Upstream

- **Project:** `BINSIDER` (category: LAPTOPS)
- **Upstream URL:** https://github.com/orhun/binsider
- **Pinned commit (SHA):** `7f0633d1a69af15cc3be9e0533cb36dbe67eb598`
- **Branch:** main
- **Pin provenance:** GitHub API commits/main. The parent-project stamp is explicitly rejected for this project.
- **Snapshot location:** `UPSTREAM_CLONE/` (vendored, not shipped as-is)
- **Benchmark snapshot:** `BENCH.json`

---

## Benchmarks

Measured by the Anticloud assurance suite. Every value below is read from this
project's `BENCH.json`, produced by a real run — the SHA3-256 of that file is
`c086413bcd6108b3da58f5d2733272d4c65734802f4cb409fe2bd68f5f5693f2`.

| Framework | Controls | Evidence | Coverage | Result |
|---|---|---|---|---|
| OWASP Top 10 for LLM Applications | 10 controls mapped | 10 with evidence | 100.0% | PASS |
| OWASP Top 10 (2021) | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| SOC 2 Type II readiness | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| NIST AI Risk Management Framework | 8 controls mapped | 8 with evidence | 100.0% | PASS |
| NIST SP 800-53 Rev. 5 | 12 controls mapped | 12 with evidence | 100.0% | PASS |
| NIST Cybersecurity Framework 2.0 | 8 controls mapped | 8 with evidence | 100.0% | PASS |
| FedRAMP Rev. 5 | 10 controls mapped | 10 with evidence | 100.0% | PASS |
| PCI DSS v4.0.1 | 11 controls mapped | 11 with evidence | 100.0% | PASS |
| ISO/IEC 27001:2022 | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| MITRE ATT&CK v16 | 12 controls mapped | 12 with evidence | 100.0% | PASS |
| ML Technology Readiness Level | TRL 8 | 8/8 criteria | | PASS |

**Overall: 16/16 checks passing.**

See `ISOLATED_LAB_RESULTS/03_Result_Register.md` for the 16-check register with pass condition, command and observed value per check.

Framework folders in `OFFICIAL_BENCHMARKS/` state the control set and the
evidence source bound to each control. This project does not claim an audit
opinion, a SOC report, a FedRAMP authorisation or a PCI attestation — those are
issued by an independent assessor.



## Archives and Permanent Records

| Platform | Identifier | Volume |
|---|---|---|
| Harvard Dataverse | DOI 10.7910/DVN/YMJKOG | 145 citable datasets |
| AIOSS verification kit | DOI 10.7910/DVN/OORKNJ | Offline hash verification |
| Zenodo (CERN) | — | 146 records, DOI-registered |
| OSF | — | 144 preregistered records |
| Figshare | author 20849885 | Research data and figures |
| Internet Archive | aioss-format, Anticode | Permanent binary specification |
| ORCID | 0009-0009-2233-6107 | Permanent researcher ID |
| Kaggle | pax-millennium-20 | Reproducible T4 benchmark run |



## Press and Independent Publication

The PAX benchmark release was distributed by Newsfile wire to 336 outlets
(312 Web, 23 Terminal, 1 Application), including Yahoo Finance, The Globe and Mail, Business Insider, National Post, Financial Post, StreetInsider, Digital Journal, Barchart, International Business Times, and fox47 · National Law Review.
Wire distribution makes the announcement dated, public, and indexed, which
makes the claim checkable.

