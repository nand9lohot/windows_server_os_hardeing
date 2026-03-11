# Windows Server OS Hardening

This repository contains a **Chef cookbook for automated Windows Server hardening** aligned with the **Center for Internet Security (CIS) Benchmarks**.

The cookbook enforces secure configuration baselines to reduce attack surface, improve compliance posture, and ensure consistent security configuration across enterprise Windows environments.

---

## Overview

Operating system misconfigurations remain one of the most common root causes of security breaches. This project provides an **Infrastructure-as-Code approach to OS hardening**, allowing organizations to automatically enforce secure configuration policies across Windows Server systems.

The cookbook applies CIS-recommended controls covering areas such as:

- Account policies
- Security options
- User rights assignments
- Audit policies
- Network security settings
- Local security configuration
- System services configuration

---

## Key Features

- Automated **CIS benchmark enforcement**
- Consistent security baselines across environments
- Chef-driven **Infrastructure-as-Code security**
- Supports **enterprise scale configuration management**
- Designed for integration with **DevSecOps pipelines**

---

## Supported Platforms

- Windows Server 2012
- Windows Server 2016
- Windows Server 2019
- Windows Server 2022

---

## Security Controls Implemented

Examples of CIS controls enforced:

- Password policy hardening
- Account lockout configuration
- Secure SMB configuration
- Audit policy enforcement
- Service configuration restrictions
- Windows Defender security settings
- Network security restrictions

The exact controls implemented follow the **CIS Windows Server Benchmark recommendations**.

---

## Usage

Include the cookbook in your Chef run list:

```ruby
run_list 'recipe[windows_server_os_hardening]'
