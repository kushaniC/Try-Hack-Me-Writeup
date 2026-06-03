**Rooms Covered:** 
- Offensive Security Intro
- Defensive Security Intro

---

## Part 1: Offensive Security Intro

### What is Offensive Security?

Offensive security is the practice of **actively attacking** systems to discover vulnerabilities before malicious hackers do. Also known as "red teaming" or ethical hacking, it involves:

- Simulating real-world cyberattacks
- Identifying weak points in networks, applications, and human processes
- Reporting findings so they can be fixed

The core principle: *"To catch a thief, think like one."*

### Key Tool Covered: `dirb`

In this room, the most important command introduced was **`dirb`** – a web content scanner.

#### What does it do?
`dirb` brute-forces directories and files on a web server using a wordlist. It helps discover hidden admin panels, backup files, or sensitive endpoints.

#### Basic Syntax:
dirb <target_url> <wordlist_path>

#### Example from the room:
dirb http://MACHINE_IP

*Default wordlist is automatically used (usually /usr/share/wordlists/dirb/common.txt)*

#### Sample Output:
+ http://MACHINE_IP/admin (CODE:200)
+ http://MACHINE_IP/backup.zip (CODE:200)
+ http://MACHINE_IP/secret (CODE:403)

#### Why it matters:
Finding hidden directories is often the first step in exploiting a web application. Many breaches start with a simple `dirb` scan revealing an unprotected login page.

### Offensive Security Summary
- **Role:** Proactive attacker
- **Mindset:** Break things ethically
- **Key command:** `dirb http://target_IP`
- **Takeaway:** Always think like an attacker to build better defenses.

---

## Part 2: Defensive Security Intro

### What is Defensive Security?

Defensive security focuses on **protecting, monitoring, and responding** to cyber threats. Also called "blue teaming," it involves:

- Setting up firewalls, antivirus, and intrusion detection systems
- Continuously monitoring logs and network traffic
- Investigating incidents and recovering from attacks
- Patching vulnerabilities before they're exploited

The core principle: *"Assume breach, verify everything."*

### Key Concepts Covered

This room focused on concepts rather than commands. The fundamental defensive concepts include:

**1. Log Analysis** – Reviewing system logs to detect unauthorized access attempts or unusual behavior.

**2. Monitoring** – Continuously observing network traffic and system activity for indicators of compromise.

**3. Incident Response** – Having a plan to contain, eradicate, and recover from security incidents.

**4. Hardening** – Reducing attack surfaces by disabling unnecessary services and applying security patches.

### Defensive Security Summary
- **Role:** Protector and responder
- **Mindset:** Monitor everything, verify constantly
- **Key skill:** Understanding security concepts and alert analysis
- **Takeaway:** Defense is about visibility and quick reaction.
