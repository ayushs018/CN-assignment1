# DNS Resolver Client-Server Project (Task-1)

## Overview
This project implements a **custom DNS resolution system** entirely in a single Google Colab notebook. The notebook handles both **client-side parsing of DNS queries from a PCAP file** and **server-side DNS resolution** with custom headers.  

- Extracts DNS queries from a PCAP file.  
- Adds a **custom 8-byte header** (`HHMMSSID`) to each DNS query.  
- Sends the modified query to a server function within the notebook.  
- Resolves DNS according to predefined rules and logs results.  
- Generates a table containing queries, custom header values, and resolved IP addresses.  

---

## Prerequisites
- Python 3.x (Google Colab already provides it)  
- Required packages:
```python
!pip install scapy pandas
```

## How to Use

### Step 1: Upload PCAP
- Upload your PCAP file containing DNS queries to Colab. In our case the file named 4 is used. 

### Step 2: Run the Notebook
- The notebook contains **both client and server code**.  
- Run all cells sequentially:
  1. Import libraries and define functions.  
  2. Load and parse the PCAP file.  
  3. Client adds **custom headers** to DNS queries.  
  4. Server function resolves DNS queries.  
  5. Logs results in the CSV file and displays output.

### Step 3: View Output
- The notebook generates a CSV file named: dns_resolution_csv.csv

  - Additionally, a **PDF** is provided containing:  
  - Observations from **Part 1**  
  - Answers for **Part 2** of the assignment
