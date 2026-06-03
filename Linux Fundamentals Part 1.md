**Room:** Linux Fundamentals Part 1

---

## What is Linux?

Linux is an open-source operating system that powers most of the internet, cloud infrastructure, cybersecurity tools, and hacking platforms. Unlike Windows or macOS, Linux gives users fine-grained control over every aspect of the system. It's the preferred OS for security professionals because most hacking tools, servers, and CTF platforms run on Linux. Learning Linux is not optional in cybersecurity — it's essential.

---

## Commands Covered

### 1. `echo`

**What it does:** Outputs text or variables to the terminal.

**Example:**
```bash
echo "Hello World"
```
Output: `Hello World`

```bash
echo $HOME
```
Output: `/home/username`

---

### 2. `whoami`

**What it does:** Displays the current logged-in username.

**Example:**
```bash
whoami
```
Output: `tryhackme`

---

### 3. `ls`

**What it does:** Lists files and directories in the current location.

**Examples:**
```bash
ls              # List files
ls -a           # List all files (including hidden)
ls -l           # List with details (permissions, size, date)
ls -la          # List all files with details
```

---

### 4. `cd`

**What it does:** Changes the current directory.

**Examples:**
```bash
cd /etc         # Move to /etc directory
cd ..           # Move up one level
cd ~            # Move to home directory
cd              # Move to home directory
```

---

### 5. `cat`

**What it does:** Displays the entire contents of a file.

**Example:**
```bash
cat file.txt
```
Output: Contents of file.txt

---

### 6. `pwd`

**What it does:** Prints the full path of your current location.

**Example:**
```bash
pwd
```
Output: `/home/tryhackme`

---

### 7. `find`

**What it does:** Searches for files and directories.

**Examples:**
```bash
find / -name "flag.txt"       # Find file named flag.txt
find /home -name "*.conf"     # Find all .conf files in /home
find . -type d -name "backup" # Find directory named backup
```

---

### 8. `grep`

**What it does:** Searches inside files for specific text.

**Examples:**
```bash
grep "password" file.txt      # Find lines containing "password"
grep -i "error" log.txt       # Case-insensitive search
grep -r "API_KEY" /etc        # Recursively search directory
```

---

### 9. Shell Operators

#### `&` (Background)

Runs a command in the background.

```bash
python3 scanner.py &
```

#### `&&` (AND)

Runs second command ONLY if first succeeds.

```bash
mkdir folder && cd folder
```

#### `>` (Redirect - Overwrite)

Sends output to a file, overwriting existing content.

```bash
echo "Hello" > file.txt
```

#### `>>` (Redirect - Append)

Adds output to the end of a file.

```bash
echo "World" >> file.txt
```

---

## Command Summary

| Command | Purpose | Example |
|---------|---------|---------|
| `echo` | Print text | `echo "Hi"` |
| `whoami` | Show user | `whoami` |
| `ls` | List files | `ls -la` |
| `cd` | Change directory | `cd /tmp` |
| `cat` | Show file content | `cat file.txt` |
| `pwd` | Show current path | `pwd` |
| `find` | Search for files | `find / -name "*.txt"` |
| `grep` | Search inside files | `grep "root" /etc/passwd` |
| `&` | Background | `./script &` |
| `&&` | Run if success | `make && make install` |
| `>` | Overwrite file | `ls > list.txt` |
| `>>` | Append to file | `echo "x" >> log.txt` |

---

## Key Takeaways

- Linux is case-sensitive
- `Tab` auto-completes commands
- `↑` arrow recalls previous commands
- `man <command>` shows the manual page
```