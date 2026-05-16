# Findings — Task 1 (Nmap Scan)

## Target
OWASP Juice Shop Demo

## Summary of Results
The scan identified multiple open ports and exposed services including FTP, DNS, HTTP, HTTPS, and additional web proxy services.

## Key Findings

### 1. FTP Service Exposed (Port 21)
- Risk Level: Medium
- Issue: FTP may transmit data without encryption
- Impact: Possible data exposure if misconfigured

### 2. Multiple Web Services (Ports 80, 443, 8080)
- Risk Level: Medium
- Issue: Multiple exposed web interfaces increase attack surface
- Impact: Higher exposure to potential vulnerabilities

### 3. Server Version Disclosure (Apache 2.4.67)
- Risk Level: Low
- Issue: Server version is visible
- Impact: Helps attackers identify known vulnerabilities

## Recommendations

- Disable unnecessary services (especially FTP if not required)
- Restrict exposed ports and services
- Hide server version information
- Ensure consistent security configuration across all web services

## Conclusion
The system shows a moderate exposure level with several services publicly accessible. Proper hardening is recommended to reduce attack surface.
