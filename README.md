# OHPC

![license](https://img.shields.io/badge/license-license-blue) ![offline-first](https://img.shields.io/badge/offline--first-air--gap-green) ![audit](https://img.shields.io/badge/audit-SHA3--256-orange) ![category](https://img.shields.io/badge/category-supercomputer-lightgrey)

> Anticloud-hardened packaging of the upstream project `OHPC` in category **SUPERCOMPUTER**. Upstream source is vendored in `UPSTREAM_CLONE/` at the pinned commit below; the 12-improvement overlay lives in `anticloud/`. Every fact in this file traces to a file on disk in this project directory.

**Category:** SUPERCOMPUTER · **Upstream:** https://github.com/openhpc/ohpc · **Upstream pin:** `25f7acb93d4e0536e3cb8d47c2a055c12a4fe1e5` · **Vendor:** Anticloud FZ LLE

---

## What This Project Does

<!-- markdownlint-disable MD013 MD033 -->
# <img src="https://github.com/openhpc/ohpc/blob/master/docs/recipes/install/common/figures/ohpc_logo.png" width="170" valign="middle" hspace="5" alt="OpenHPC"/>
<!-- markdownlint-enable MD013 MD033 -->

## Community building blocks for HPC systems

### Introduction

This stack provides a variety of common, pre-built ingredients required to
deploy and manage an HPC Linux cluster including provisioning tools, resource
management, I/O clients, runtimes, development tools, containers,
and a variety of scientific libraries.

There are currently three release series: the [2.x][2xbranch], the
[3.x][3xbranch] and the [4.x][4xbranch] which target different major Linux OS
distributions:

- The 2.x series targets EL8 and Leap15.
- The 3.x series targets EL9, Leap 15 and openEuler 22.03.
- The 4.x series targets EL10 and openEuler 24.03.

### Getting started

OpenHPC provides pre-built binaries via projects for use with standard
Linux package manager tools (e.g. ```dnf``` or ```zypper```). To get started,
you can enable an OpenHPC project locally through installation of an
```ohpc-release``` RPM which includes gpg keys for package signing and defines
the URL locations for [base] and [update] package projects. Installation
guides tailored for each supported provisioning system and resource manager
with detailed example instructions for installing a cluster are also available.
Copies of the ```ohpc-release``` package and installation guides along with
more information is available on the relevant release series pages
([2.x][2xbranch], [3.x][3xbranch] or [4.x][4xbranch]).

---

### Questions, Comments, or Bug Reports?

Subscribe to the [users email list][userlist] or see the
<https://openhpc.community/> page for more pointers.

### Additional Software Requests?

If you would like to see new software included in OpenHPC, please
[open an issue](https://github.com/openhpc/ohpc/issues) with as much
detail as possible. Even better, consider opening a pull request directly.
A PR for a new component should typically include tests and documentation,
but we are happy to guide contributors through the process.

### Contributing to OpenHPC

Please see the steps described in [CONTRIBUTING.md](CONTRIBUTING.md).

### Register your system

If you are using elements of OpenHPC, please consider registering your system(s)
using the [System Registration Form][register].

[2xbranch]: https://github.com/openhpc/ohpc/wiki/2.x
[3xbranch]: https://github.com/openhpc/ohpc/wiki/3.x
[4xbranch]: https://github.com/openhpc/ohpc/wiki/4.x
[register]: https://drive.google.com/open?id=1KvFM5DONJigVhOlmDpafNTDDRNTYVdolaYYzfrHkOWI
[userlist]: https://groups.io/g/openhpc-users

*Quoted from the upstream `README.md` file in `UPSTREAM_CLONE/`.*
Project-specific facts detected in this directory:

- Ecosystem: **Unknown (no standard manifest detected)** (manifests: none detected; scanned in UPSTREAM_CLONE)
- Top-level source layout: `components/`, `containers/`, `devel/`, `misc/`, `tests/`
- Snapshot size: **1443 files**, **71454 lines of code** (measured; see Benchmarks)
- Primary languages: `(none)` (272), `.f90` (183), `.j2` (141), `.hpp` (140), `.spec` (93), `.c` (70)
- Upstream commit pinned for this packaging: `25f7acb93d4e0536e3cb8d47c2a055c12a4fe1e5`

---

## Installation

No installation section was found in the upstream readme, so the commands below are generated from the manifests detected in this project directory.

```sh
# No standard manifest detected. Inspect UPSTREAM_CLONE/ for the upstream
# build system (Makefile, CMakeLists.txt, configure, ...) and follow it.
```

Overlay install (this project):

```sh
python -m pip install -e anticloud/     # overlay package with the 12 improvements
python anticloud/cli.py --help          # 13 subcommands, JSON stdout
```

---

## Usage

OpenHPC provides pre-built binaries via projects for use with standard
Linux package manager tools (e.g. ```dnf``` or ```zypper```). To get started,
you can enable an OpenHPC project locally through installation of an
```ohpc-release``` RPM which includes gpg keys for package signing and defines
the URL locations for [base] and [update] package projects. Installation
guides tailored for each supported provisioning system and resource manager
with detailed example instructions for installing a cluster are also available.
Copies of the ```ohpc-release``` package and installation guides along with
more information is available on the relevant release series pages
([2.x][2xbranch], [3.x][3xbranch] or [4.x][4xbranch]).

---

*Section quoted from the upstream readme.*
Anticloud overlay CLI (available in every project):

```sh
python anticloud/cli.py --help     # 13 subcommands, JSON stdout
python anticloud/cli.py checks     # run the 16-check suite
```

---

## API

and a variety of scientific libraries.

There are currently three release series: the [2.x][2xbranch], the
[3.x][3xbranch] and the [4.x][4xbranch] which target different major Linux OS
distributions:

- The 2.x series targets EL8 and Leap15.
- The 3.x series targets EL9, Leap 15 and openEuler 22.03.
- The 4.x series targets EL10 and openEuler 24.03.

*Section quoted from the upstream readme.*
---

## Dependencies

| Metric | Value |
|--------|-------|
| Ecosystem | Unknown (no standard manifest detected) |
| Manifests detected | none |
| Files in snapshot | 1443 |
| Lines of code | 71454 |
| Dependency references | 0 |
| Upstream license | Apache-2.0 |
| Overlay license | Anticommons 0.1.0 |

Pinned lockfile: `anticloud/requirements.lock` (hash-pinned, PEP 508). SBOM: `sbom.cdx.json` (CycloneDX 1.5, pinned to the upstream SHA).

---

## Configuration

No configuration section was found in the upstream readme. Configuration-relevant files detected in this project directory:

- None detected at the snapshot root; consult the upstream documentation link in the Upstream section.

Overlay configuration (Anticloud):

- `anticloud/` - improvement overlay; environment-driven, no cloud dependency
- `LEDGERS/` - aioss tamper-evident chain files (per-project, verified with `aioss verify --live`)
- `ISOLATED_LAB_RESULTS/` - reproducibility record (environment, reproduction steps, result register, evidence)
- `OFFICIAL_BENCHMARKS/` - 26 framework assessments for this project

---

## Contributing

*Excerpt from upstream `CONTRIBUTING.md`:*

# How to contribute to OpenHPC

General information about participating in the OpenHPC project can be found at
the [OpenHPC Community site][community]. The instructions below are
specifically for opening issues and pull requests against OpenHPC.

## **Did you find a bug?**

* **Ensure the bug was not already reported** by searching on GitHub under [Issues][issues].

* If you're unable to find an open issue addressing the problem, [open a new one][new].

* You may also send a message to the OpenHPC [user mailing list][userlist].

## **Did you write a patch that fixes a bug?**

* Open a new GitHub pull request with the patch.

* Ensure the PR description clearly describes the problem and solution.
  If there is an existing GitHub issue open describing this bug, please include
  it in the description so we can close it.

* Ensure the PR is based on the latest branch of the OpenHPC GitHub project.

* Before submitting, please read the [Contributing to OpenHPC][contribute] wiki.
  In particular, note that all git commits contributed to OpenHPC require a
  `Signed-off-by:` line.

## **Do you have a component suggestion for inclusion in the OpenHPC distribution?**

* [Open an issue][new] with details about the component you would like to see
  included. Even better, consider opening a pull request directly. A PR for a
  new component should typically include tests and documentation, but we are
  happy to guide contributors through the process.

[community]: https://openhpc.community/about/participate
[contribute]: https://github.com/openhpc/ohpc/wiki/Contributions
[issues]: https://github.com/openhpc/ohpc/issues
[new]: https://github.com/openhpc/ohpc/issues/new
[userlist]: https://groups.io/g/OpenHPC-users/topics

Overlay contributions: run the 16-check suite before opening a pull request:

```sh
python anticloud/bench/runner.py --cwd anticloud
```

---

## License

**Upstream license: Apache-2.0** (evidence: `LICENSE` in the upstream snapshot).

License file excerpt:

```text

                                 Apache License
                           Version 2.0, January 2004
                        http://www.apache.org/licenses/

   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION

   1. Definitions.

      "License" shall mean the terms and conditions for use, reproduction,
      and distribution as defined by Sections 1 through 9 of this document.

      "Licensor" shall mean the copyright owner or entity authorized by
      the copyright owner that is granting the License.

      "Legal Entity" shall mean the union of the acting entity and all
      other entities that control, are controlled by, or are under common
      control with that entity. For the purposes of this definition,
      "control" means (i) the power, direct or indirect, to cause the
      direction or management of such entity, whether by contract or
```

### Anticommons 0.1.0 overlay

The Anticloud integration overlay in `anticloud/` - improvements 1 through 12 listed under Benchmarks - is licensed under **Anticommons 0.1.0**. Upstream code remains under its original Apache-2.0 terms. See `ANTICOMMONS_LICENSE.md` in this directory for the overlay terms and contact.

SPDX: `Apache-2.0` (upstream) + Anticommons 0.1.0 (overlay, dual).

---

## Upstream

- **Project:** `OHPC` (category: SUPERCOMPUTER)
- **Upstream URL:** https://github.com/openhpc/ohpc
- **Pinned commit (SHA):** `25f7acb93d4e0536e3cb8d47c2a055c12a4fe1e5`
- **Branch:** 4.x
- **Pin provenance:** GitHub API commits/<branch> (response quoted in report). The parent-project stamp is explicitly rejected for this project.
- **Snapshot location:** `UPSTREAM_CLONE/` (vendored, not shipped as-is)
- **Benchmark snapshot:** `BENCH.json`

---

## Benchmarks

Measured by the Anticloud assurance suite. Every value below is read from this
project's `BENCH.json`, produced by a real run — the SHA3-256 of that file is
`87c962a81fa353e8718ca134ec64694697cc97857013e3471996a1eb89eea267`.

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
| DANS (KNAW/NWO, Netherlands) | 10.17026/PT | EU-recognised archive |
| Zenodo (CERN) | — | 146 records, DOI-registered |
| OSF | — | 144 preregistered records |
| Figshare | author 20849885 | Research data and figures |
| Internet Archive | aioss-format, Anticode | Permanent binary specification |
| ORCID | 0009-0009-2233-6107 | Permanent researcher ID |
| Kaggle | pax-millennium-20 | Reproducible T4 benchmark run |



## Press and Independent Publication

The PAX benchmark release was distributed by Newsfile wire to 336 outlets
(312 Web, 23 Terminal, 1 Application), including Yahoo Finance, The Globe
and Mail, Business Insider, National Post, Financial Post, StreetInsider,
Digital Journal, Barchart, International Business Times, and Fox News.
Wire distribution makes the announcement dated, public, and indexed, which
makes the claim checkable.

