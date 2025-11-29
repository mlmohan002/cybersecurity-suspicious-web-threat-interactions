# Cybersecurity - Suspicious Web Threat Interactions

## Project Overview
This project analyzes suspicious web traffic and threat interactions detected by CloudWatch and WAF (Web Application Firewall). The dataset contains security logs capturing adversary infrastructure interactions with production web servers, including source IPs, geographic origin, bytes transferred, protocols, and detection rules triggered.

## Purpose
- Identify patterns in web-based attacks and suspicious traffic
- Analyze traffic from different geographic regions
- Understand threat signatures and detection mechanisms
- Provide insights for security incident response and threat intelligence

## Dataset Description
**File:** `CloudWatch_Traffic_Web_Attack.csv`

### Key Columns
- **bytes_in / bytes_out**: Data transferred in both directions (bytes)
- **creation_time / end_time**: Timestamp window of the traffic event
- **src_ip**: Source IP address of the attacker
- **src_ip_country_code**: Geographic location (country code) of the source
- **protocol**: Network protocol used (e.g., HTTPS)
- **response.code**: HTTP response code (e.g., 200)
- **dst_port**: Destination port (e.g., 443)
- **dst_ip**: Destination IP (production server)
- **rule_names**: Security rule triggered (e.g., "Suspicious Web Traffic")
- **observation_name**: Threat category (e.g., "Adversary Infrastructure Interaction")
- **detection_types**: Detection mechanism (e.g., "waf_rule")

## How to Run

### Prerequisites
- Python 3.7+ installed
- pip package manager

### Installation
1. Extract this ZIP file to your preferred location
2. Open Command Prompt or PowerShell in the project folder
3. Install dependencies:
   ```
   pip install -r requirements.txt
   ```

### Running the Analysis
1. Open the notebook:
   ```
   jupyter notebook notebooks/Cybersecurity_-Suspicious-Web-Threat-Interactions.ipynb
   ```
2. Or use Jupyter from VS Code or any Python IDE
3. Run all cells to generate analysis and visualizations

## Project Structure
```
cybersecurity-suspicious-web-threat-interactions/
├── notebooks/
│   └── Cybersecurity_-Suspicious-Web-Threat-Interactions.ipynb
├── data/
│   └── CloudWatch_Traffic_Web_Attack.csv
├── requirements.txt
├── README.md
└── .gitignore
```

## Key Libraries Used
- **pandas**: Data manipulation and analysis
- **matplotlib**: Static visualization
- **seaborn**: Statistical data visualization

## Potential Analysis Insights
- Geographic distribution of attacks
- Traffic volume patterns over time
- Top attacking IP addresses
- Bytes transferred analysis
- Protocol and port usage patterns
- Detection rule effectiveness

## Notes
- This is educational/analytical data for security research
- All IPs and data are for demonstration purposes
- Suitable for cybersecurity portfolio projects

## Author
Data Science Fresher | Security Analytics Project

---
*Last Updated: November 2025*
