# DNS-HTTP-Log-Analysis-using-Splunk-
This project focuses on analyzing DNS and HTTP logs using Splunk SIEM to detect suspicious network behavior, abnormal web traffic, and potential indicators of compromise (IOCs). The objective is to simulate real-world SOC monitoring and threat analysis scenarios.
Objectives 

# Objectives 
• Ingest JSON-formatted DNS logs into Splunk • Extract useful DNS metadata (queries, IPs, record types) • Write SPL queries for DNS traAic analysis • Detect suspicious or abnormal DNS activity • Build a strong foundation for DNS-based threat detection
Ingest and analyze HTTP logs using Splunk • Detect client-side (4xx) and server-side (5xx) HTTP errors • Identify suspicious User-Agents and URIs • Detect large file transfers that may indicate data exfiltration • Gain practical experience with SPL (Search Processing Language)

# Tools & Technologies
•	Splunk Enterprise
•	SPL (Search Processing Language)
•	HTTP & DNS log dataset (CSV)
•	SOC monitoring techniques

# Data Information
Field	Description
timestamp	Event time (ISO format)
log_type	http / dns
src_ip	Source IP
dest_ip	Destination IP
method	HTTP method / DNS QUERY
uri	Web URI (HTTP only)
status	HTTP status or DNS response
user_agent	Client user agent
bytes	Data size
tls_version	TLS version (HTTP only)
domain	Website / DNS domain

# How to Add This File into Splunk
1.	Open Splunk Web
2.	Settings → Add Data
3.	Select Upload
4.	Upload splunk_http_dns_dataset.csv
5.	Source type: csv
6.	Index: web_logs (or any you like)
7.	Finish 

# Key Use Cases Implemented
•	DNS query monitoring and domain resolution analysis
•	Detection of suspicious or abnormal DNS request patterns
•	HTTP request analysis (GET/POST, status codes)
•	Identification of suspicious URLs and repeated requests
•	Source IP behavior analysis
•	Time-based traffic analysis using timecharts

# SPL Queries Implemented
•	Top queried domains and URLs
•	DNS request frequency per source IP
•	HTTP status code distribution (200, 401, 403, 404)
•	High-volume request detection
•	Suspicious domain lookup detection

# Outcome
•	Built SOC-style dashboards for network visibility
•	Improved understanding of log correlation and threat hunting
•	Hands-on experience with SIEM-based monitoring
