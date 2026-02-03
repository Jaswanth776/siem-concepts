# SIEM Concepts

This repository is my structured knowledge base and practical documentation created while learning **SIEM Engineering** with a primary focus on **Splunk**, Windows Event Logs, and log ingestion fundamentals.

The goal of this repository is to clearly understand **how SIEM works internally** — from log collection to parsing, indexing, and analysis — supported by hands-on lab experiments.

---

## 🎯 Purpose

Most learners focus only on alerts and dashboards.  
This repository focuses on the **core SIEM foundation**:

- How logs enter SIEM
- How Splunk identifies and tracks files (CRC & Fishbucket)
- How forwarding works (`inputs.conf` / `outputs.conf`)
- How Windows Event Logs are collected using XML
- How log rotation affects ingestion
- How parsing happens using `props.conf` and `transforms.conf`
- Difference between restart and debug refresh
- Practical lab experiments performed in Linux and Windows environments

---

## 🧠 Topics Covered

### SIEM Basics
- What is SIEM
- Ingestion pipeline
- Inputs vs Ingestion

### Splunk Inputs
- `inputs.conf` basics
- Monitor stanza syntax
- `crcSalt` usage

### Splunk Outputs
- `outputs.conf` basics
- `tcpout` group syntax
- Forwarder to Indexer data flow

### CRC & Fishbucket
- First 256 bytes CRC behavior
- Fishbucket tracking
- Problems with static headers
- Testing ingestion scenarios

### Log Rotation
- What is log rotation
- Linux `logrotate`
- Impact on Splunk monitoring

### Windows Event Logs
- `WinEventLog` stanza syntax
- `renderXml = true`
- Important security Event IDs

### Parsing & Indexing
- `props.conf` basics
- `transforms.conf` basics
- Parsing vs Indexing

### Debug Refresh vs Restart
- Splunk restart behavior
- `/debug/refresh` endpoint usage

### Hands-On Labs
- Linux auth.log forwarder lab
- Windows Event Log forwarding lab
- CRC and `crcSalt` testing lab

---

## 🛠️ Tools & Platforms Used

- Splunk Enterprise
- Splunk Universal Forwarder
- Linux log sources (`/var/log/auth.log`, syslog)
- Windows Event Logs (Application, Security, System)
- Virtual lab environments for testing ingestion behavior

---

## 📌 Why this repository exists

This is not just notes.  
This is a **documented journey** of understanding SIEM from the inside, combining:

> Theory + Configuration + Practical Lab Observation

This repository also serves as:
- Personal revision material
- Interview preparation reference
- Proof of practical SIEM understanding

---

## 🚀 Ongoing Work

This repository will continuously grow as I learn more about:
- SIEM engineering concepts
- Detection engineering
- Advanced log parsing
- Additional SIEM platforms

---

## 👨‍💻 Author

Jaswanth — Cybersecurity student focused on becoming a SIEM Engineer.
