**Room:** Search Skills

---

## Overview

Knowing where to search is just as important as knowing what to search for. This room covers essential search resources for both offensive and defensive security.

---

## Key Resources Covered

### 1. Shodan

A search engine for internet-connected devices. Scans the entire internet for networking equipment, IoT devices, cameras, and more.

**Example search:** `apache 2.4.1`

**Useful filters:**

| Filter | Description | Example |
|--------|-------------|---------|
| `country` | Restrict to country code | `country:IE` |
| `port` | Filter by port | `port:22` |
| `org` | Filter by organisation | `org:Amazon` |
| `hostname` | Match specific domain | `hostname:example.com` |

---

### 2. VirusTotal

Aggregates results from 70+ antivirus engines. Submit a file, URL, domain, or hash to check if it's flagged as malicious.

**Use case:** Blue teaming - getting consensus on suspicious files or links.

---

### 3. CVE Programme (Common Vulnerabilities and Exposures)

Universal dictionary of known vulnerabilities.

**Format:** `CVE-YEAR-NUMBER` (e.g., CVE-2025-55182)

**CVSS Score factors:**
- Impact - What damage can it cause?
- Complexity - How easy to exploit?
- Availability - How likely is exploitation?

**Notable examples:** Heartbleed, Log4Shell, React2Shell

---

### 4. ExploitDB

Compiles vulnerabilities alongside Proof of Concept (PoC) scripts that demonstrate exploitation.

---

### 5. Official Documentation

Always the first stop for troubleshooting or learning tool usage. More reliable than third-party tutorials.

---

### 6. Linux Man Pages

Built-in terminal documentation for any command.

**Usage:** `man <command>`

**Example:** `man nc`

---

### 7. GitHub

Researchers publish PoC code, scanners, and technical reports. Search for CVE identifiers to find related repositories.

**⚠️ Warning:** Not all PoCs are reliable. Some are incomplete, flawed, or malicious. Verify before executing.

---

## Summary Table

| Resource | Best For |
|----------|----------|
| Shodan | Finding internet-connected devices |
| VirusTotal | Checking files/URLs against antivirus engines |
| CVE Database | Finding vulnerability details |
| ExploitDB | Finding working exploits |
| Official Docs | Learning tools properly |
| Man Pages | Quick command reference |
| GitHub | Finding PoC code and research |

---

## Key Takeaway

Effective searching is a critical cybersecurity skill. Know which resource to use for which task.