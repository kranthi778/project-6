# vulnerability-analysis-project

# Part 1 – Understanding Vulnerability Analysis and Setting Up Nessus

## Objective

I want to understand what Vulnerability Analysis is about. I need to learn how it is different from scanning networks and finding out what is on them. I also want to set up Nessus Essentials so I can use it to find vulnerabilities.

---

# What is Vulnerability Analysis?

Vulnerability Analysis is a process. It helps us find security weaknesses in operating systems, applications and network services. We do this before someone with intentions can find and use these weaknesses against us.

Vulnerability Analysis is not the same as scanning a network. When we scan a network we are just trying to find out what computers and services are available.. With Vulnerability Analysis we are trying to figure out if those computers and services have any known security problems. We also want to know how bad these problems could be.

The main things we want to do with Vulnerability Analysis are:

- Find vulnerabilities

- Figure out how risk they pose

- Decide which ones to fix first

- Make our organizations security better

---

# Difference Between Scanning Finding Out More and Vulnerability Analysis

| Phase | Purpose  |


| Network Scanning | Find computers, open ports and services on the network |

| Finding Out More | Get details about the services we found |

| Vulnerability Analysis | Find known security weaknesses in those services |

---

# How to Do a Vulnerability Assessment

To do a vulnerability assessment we need to follow some steps:

1. Decide what we want to assess.

2. Set up our vulnerability scanner.

3. Scan the computers and services we're interested in.

4. Look at the vulnerabilities we found.

5. Figure out which ones are the important to fix.

6. Recommend how to fix them.

---

# Our Lab Environment

## The Computer We Will Use to Attack

- We will use Kali Linux.

## The Computers We Will Attack

- 2

- Windows 7

## The Tool We Will Use to Find Vulnerabilities

- Nessus Essentials

---

## Step 1: Check if the Nessus Service is Running

### What We Are Doing

We need to make sure the Nessus service is installed and running before we start.

### What to Type

```bash

sudo systemctl status nessusd

```

### What This Does

This command tells us if the Nessus service is running or not.

### Screenshot

![Alt text](screenshots/nessus-service-status.png)

---

## Step 2: Start the Nessus Service

### What We Are Doing

If the Nessus service is not running we need to start it.

### What to Type

```bash

sudo systemctl start nessusd

```

### What This Does

This command starts the Nessus service.

### Screenshot

![Alt text](screenshots/start-nessus-service.png)

---

## Step 3: Open the Nessus Dashboard

### What We Are Doing

Now we need to open the Nessus web interface.

### Where to Go

```text

https://localhost:8834

```

### What This Does

We open the Nessus Essentials dashboard in our web browser and make sure the login page comes up correctly.

### Screenshot

![Alt text](screenshots/nessus-dashboard.png)
nessus-service-status
---

# Things I Learned

- What Vulnerability Analysis is

- How to do a Vulnerability Assessment

- What Nessus Essentials is

- How to use the Nessus web interface

- The steps to follow for a vulnerability assessment

---

# Key Concepts Learned

- Vulnerability Analysis
- Vulnerability Assessment
- Nessus Essentials
- Assessment Workflow
- Nessus Web Interface

