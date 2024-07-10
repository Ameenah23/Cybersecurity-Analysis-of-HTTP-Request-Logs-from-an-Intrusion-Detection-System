# Analysis-of-HTTP-Request-Logs-from-an-Intrusion-Detection-System
Author: 
### Ameenah Al-Haidari
Date: April 2024

### Abstract
This report details the analysis of a log file containing HTTP requests recorded by an Intrusion Detection System (IDS). The primary focus is to identify the three most commonly seen hosts, describe their characteristics, and visualize their activity over time. The analysis is performed using a systematic approach to parse the log data, convert timestamps, and generate informative visualizations.

### Introduction
Intrusion Detection Systems (IDS) play a critical role in monitoring and analyzing network traffic to detect potential security threats. The log file (part2.log) analyzed in this report contains HTTP request records, which provide valuable insights into network activities and potential security breaches. This analysis aims to:

1. Identify the three most commonly seen hosts in the log file.
2. Describe these hosts.
3. Visualize the activity of these hosts over time.

### Methodology
#### Data Collection
The log file (part2.log) was obtained from a provided link. The file records various HTTP request details, including timestamps, hostnames, source IP addresses, request methods, URLs, protocols, response codes, content sizes, referers, and user agents.

#### Data Processing
The log file was processed to extract relevant fields from each record. This involved reading the log file line by line, splitting each line into fields, and recording these fields in a structured format. The extracted fields included:

- Timestamp
- Host
- Source IP
- Request Method
- URL
- Protocol
- Response Code
- Content Size
- Referer
- User Agent

### Data Analysis
1. Identifying Common Hosts:
The most frequently occurring hosts in the log file were identified by counting the occurrences of each host and selecting the top three.

2. Host Description:
Brief descriptions of the top three hosts were provided based on their characteristics and potential relevance to the network traffic.

3. Visualization:
The activity of the top three hosts was visualized over time. This involved converting the timestamp field to a datetime object and generating time series plots to show the number of requests per minute for each host. Additionally, a bar plot was created to illustrate the number of requests per source IP for the top three hosts.

### Results
Common Hosts
The three most commonly seen hosts in the log file were identified as follows:

1. Host A: The most frequent host, potentially indicating a significant source of traffic.
2. Host B: The second most common host, likely related to consistent or automated traffic.
3. Host C: The third most common host, possibly associated with specific services or applications.

### Host Descriptions
- Host A: This host appears to generate a high volume of requests, possibly due to automated processes or high user activity.
- Host B: This host may be part of a routine network operation, contributing to regular traffic patterns.
- Host C: This host could be linked to specific applications or services that generate periodic requests.

### Visualizations
1. Time Series Plot:
The time series plot illustrated the number of requests per minute for the top three hosts, showing peaks and patterns in their activity over time. This visualization helps in identifying periods of high activity and potential anomalies.

2. Bar Plot:
The bar plot displayed the number of requests per source IP for the top three hosts. This visualization provided insights into the distribution of requests among different source IP addresses, highlighting any concentrated or distributed traffic sources.

### Discussion
The analysis revealed distinct patterns in the activity of the top three hosts, which could indicate normal network operations or potential security threats. The visualizations helped in identifying peak traffic periods and understanding the distribution of requests across source IPs. Further investigation into the nature of these hosts and their traffic patterns could provide deeper insights into network behavior and security.

### Conclusion
This report demonstrates a comprehensive approach to analyzing log files from an Intrusion Detection System. By identifying and describing the most common hosts and visualizing their activity, valuable insights into network traffic and potential security issues were gained. This methodology can be applied to similar log analyses in various domains, enhancing the ability to detect and respond to network anomalies and threats.

### References
Intrusion Detection System (IDS) Logs: https://web.cs.dal.ca/~kuzniar/a2_files/part2.log
Python for Data Analysis, Wes McKinney, O'Reilly Media, 2017
Matplotlib Documentation: https://matplotlib.org/stable/contents.html

