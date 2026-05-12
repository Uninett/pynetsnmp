# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

This changelog only lists changes that have been made since this forked version
of pynetsnmp came under the care of Uninett, and later Sikt.

## [Unreleased]

### Changed

- Packaging modernized from `setup.py`/`setup.cfg` to `pyproject.toml` ([#9](https://github.com/Uninett/pynetsnmp/issues/9))

### Removed

- Dropped dependencies that were only there because of Python 2 compatibility in older versions:
  - `six` ([#13](https://github.com/Uninett/pynetsnmp/issues/13))
  - `ipaddr` ([#9](https://github.com/Uninett/pynetsnmp/issues/9))
- Dropped explicit support for Python < 3.9.

## [0.1.10] - 2023-11-16

### Fixed

- SNMPv3 error handling routines were not Python 3 compatible. ([#3](https://github.com/Uninett/pynetsnmp/issues/3))
- Broken `TableRetriever` behavior in certain SNMPv3 error situations. ([#4](https://github.com/Uninett/pynetsnmp/issues/4))

## [0.1.9] - 2022-03-18

### Fixed

- A regression that caused IPv6 support to stop working on NET-SNMP 5.9 (and possibly 5.8). ([#2](https://github.com/Uninett/pynetsnmp/issues/2))

## [0.1.8] - 2022-02-08

### Fixed

- A memory leak issue under NET-SNMP 5.8 and newer.

## [0.1.7] - 2021-07-28

### Fixed

- An incorrect link back to this repo in the package metadata.

## [0.1.6] - 2021-07-28

### Fixed

- Enable compatibility with NET-SNMP 5.8
