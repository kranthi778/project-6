# vulnerability-analysis-project

# Part 1 – Introduction to Vulnerability Analysis

## Objective

I want to understand what Vulnerability Analysis is and how to do an assessment using Nmaps scripts to find vulnerabilities.

---

# What is Vulnerability Analysis?

Vulnerability Analysis is a process to find security weaknesses in systems and services before someone can exploit them.

It is different from Network Scanning.

Network Scanning finds hosts and services.

Vulnerability Analysis checks if those services have known security weaknesses.

The goal of Vulnerability Analysis is to:

- Find vulnerabilities

- Check security risks

- Decide what to fix first

- Make the security

---

# Vulnerability Analysis Workflow

1. Find the target

2. See what services are running

3. Detect what software versions are used

4. Compare them to known vulnerabilities

5. Write down the findings

---

## 1. Update the Nmap Script Database

### Scenario

I need to update the Nmap script database before I do a vulnerability assessment.

### Command

```bash

sudo nmap --script-updatedb

```

### Description

This command updates the Nmap script database so it knows about scripts.

### Screenshot

![Alt text](screenshots/nmap-script-updatedb.png)

---

## 2. Run the Vulnerability Script Category

### Scenario

Now I do a vulnerability assessment, on the target.

### Command

```bash

sudo nmap --script vuln <target-ip>

```

### Description

This command runs all the Nmap scripts that check for vulnerabilities to see if the target has any.

Replace the IP address with the target IP address.

### Screenshot

![Alt text](screenshots/nmap-vuln-scan.png)

---

## 3. Save the Vulnerability Report

### Scenario

I need to save the vulnerability assessment results.

### Command

```bash

sudo nmap --script vuln <target-ip> -oN vulnerability-scan.txt

```

### Description

This command saves the scan results in a text file.

### Screenshot

![Alt text](screenshots/vulnerability-report.png)

---

## 4. Review the Saved Report

### Scenario

Now I review the vulnerability report.

### Command

```bash

less vulnerability-scan.txt

```

### Description

This command opens the report so I can read it easily.

### Screenshot

![Alt text](screenshots/review-vulnerability-report.png)

---

# Key Concepts Learned

- Vulnerability Analysis

- NSE Vulnerability Scripts

- Vulnerability Identification

- Security Assessment

- Scan Reporting

---

# Conclusion

In this part, I learned:

- The purpose of Vulnerability Analysis.
- How Nmap NSE scripts detect known vulnerabilities.
- How to document vulnerability findings.
- How vulnerability reports support remediation planning.
