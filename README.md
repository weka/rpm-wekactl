# rpm-wekactl

YUM/DNF (RHEL/Fedora/CentOS) package repository for
[`wekactl`](https://github.com/weka/goweka), the Go-based Weka CLI.

> **Generated content — do not edit by hand.**
> The `repodata/` metadata and the packaged RPM are produced by the release
> pipeline in `weka/goweka` (`scripts/build_repos.sh`) and published here
> automatically. Manual edits will be overwritten on the next release.

## Installing

The canonical, supported way to install `wekactl` on RHEL/Fedora/Rocky/Amazon
Linux is through **[get.weka.io](https://get.weka.io/)**, which documents how to
enable the signed YUM/DNF repository and install the package:

```sh
dnf install wekactl
```

Use the `baseurl` from get.weka.io rather than pointing `yum`/`dnf` at this
repo's GitHub Pages URL directly, so your configured `baseurl` stays stable
across hosting changes. The repository is GPG-signed, so installing this way
also verifies the package.

## What lives where

- **GitHub Pages (this repo)** serves the live YUM/DNF repository — the signed
  metadata (`repodata/repomd.xml` and friends) plus the **current** `wekactl`
  RPM. This is the tree `yum`/`dnf` reads.
- **[Releases](../../releases)** hold the **back-catalog** of `.rpm` packages for
  every published version, as downloadable assets. `yum`/`dnf` do not see these;
  they are for manual download when you need a specific older build.

## Source

Packaging, signing, and publishing logic lives in
**[weka/goweka](https://github.com/weka/goweka)**. File issues and changes there,
not here.
