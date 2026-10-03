# sybase-ase-recovery
Read-only Sybase ASE recovery tool. Repair corrupted Sybase ASE database files and damaged backup dumps, supports Sybase ASE 11–16.
# Sybase ASE Recovery Tool

A read-only Sybase ASE recovery utility for corrupted database files and damaged backup dump files.

## Overview

Sybase ASE Recovery Tool performs offline, read-only analysis on Sybase ASE database device files and backup dump files. It parses corrupted database page structures directly, extracts usable table data from broken files, and salvages records from damaged dumps without writing any changes to your source evidence.

All scanning operations run in **read-only mode** — your original database files and backup files remain untouched.

## Supported Versions
--mssql 6.5
- Sybase ASE 11
- Sybase ASE 12
- Sybase ASE 15
- Sybase ASE 16

## Core Capabilities

- Repair and recover data from corrupted Sybase ASE database device files
- Recover data from damaged Sybase ASE backup dump files
- Extract table data from broken, unmountable or inconsistent database files
- Preview recoverable table data before export
- **100% read-only scan**: source files will never be modified

## Use Cases

- Sybase ASE database file corruption
- Damaged or broken backup dump files
- Database device file cannot be loaded or mounted
- Data rescue from corrupted Sybase data files
- Recovery from damaged database dump files

## How It Works

1. The tool scans the corrupted Sybase ASE database file or backup dump in read-only mode.
2. It parses internal database page structures directly.
3. Recoverable tables and records are identified and extracted.
4. Recoverable data is displayed in a preview view.
5. Verified data can be exported after preview.

## Important Notice

This is an offline forensic analysis tool.

We do **not** write or modify the original database files or backup files during scanning. Always work on copies of your source files for evidence safety.

## Download

Get the latest Windows binary release on GitHub Releases.

> Pre-built Windows x64 zip package, contains the read-only Sybase ASE recovery client.


## Antivirus Note

> ⚠️ The Windows binary is protected with VMProtect for anti-tampering. Some antivirus software may incorrectly flag it as malware (false positive). This tool works in fully read-only mode and will not modify your database source files.

## Contact

For technical feedback, bug reports or feature requests, please open a GitHub issue.
