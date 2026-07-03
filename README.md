# rpm-wekactl

YUM/DNF (RHEL/Fedora/CentOS) package repository for
[`wekactl`](https://github.com/weka/goweka), the Go-based Weka CLI.

> **Generated content — do not edit by hand.**
> The `repodata/` metadata and the packaged RPM are produced by the release
> pipeline in `weka/goweka` (`scripts/build_repos.sh`) and published here
> automatically. Manual edits will be overwritten on the next release.

## What lives where

- **GitHub Pages (this repo)** serves the live YUM/DNF repository — the signed
  metadata (`repodata/repomd.xml` and friends) plus the **current** `wekactl`
  RPM. This is what `yum`/`dnf` reads.
- **[Releases](../../releases)** hold the **back-catalog** of `.rpm` packages for
  every published version, as downloadable assets. `yum`/`dnf` do not see these;
  they are for manual download when you need a specific older build.

## Installing

The canonical, supported install path is documented with the CLI itself. Use the
Weka-provided repository URL rather than pointing `yum`/`dnf` at this repo's Pages
URL directly, so your configured `baseurl` stays stable across hosting changes.

## Source

Packaging, signing, and publishing logic lives in
**[weka/goweka](https://github.com/weka/goweka)**. File issues and changes there,
not here.
