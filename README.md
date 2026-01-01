# security-log-analyzer
## Overview
A Python-based application designed to automate the analysis of system and application logs to identify suspicious activity and potential security incidents. This project simulates real-world SOC workflows by detecting anomalies such as brute-force log-in attempts, abnormal access patterns, and high-risk IP-behavior.

## Why This Project Matters?
Organizations generate massive volumes of logs that are often reviewed manually or reactively. This tool demonstrates how security automation can: 
- Reduce incident respone times.
- Improve threat visibility.
- Support compliance and audit readiness.

## Key Features
- Parses authentication and access logs.
- Detects brute-force and anomaly patterns.
- Aggregates suspicious IP activity.
- Generates structured reports (CSV/JSON)
- REST API for querying flagged events.

## Tech Stack
- Python
- FastAPI
- pandas
- Regex
- Docker
- AWS S3 (optional for cloud deployment)

## Architecture
- Log ingestion layer
- Analysis engine
- API layer for reporting
- Optional cloud storage integration

## Security Considerations
- Input validation on all log ingestion.
- Read-only access for log sources.
- Secure API end-points with authentication
- Designed with least privelege principles

## How to Run
1. Clone the repository
2. Install dependencies
3. Run the analysis engine
4. Access the API for results

## Sample output

```json
{
  "ip": 192.168.1.10,
  "failed attempts": 32,
  "risk_level": "high"
}


Author
JamesP
