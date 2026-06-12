..Nmap Reconnaissance Report..

 Objective

To perform basic network reconnaissance and identify active hosts, open ports, and running services on a target machine in a controlled lab environment.

 Tools Used

* Nmap
* Kali Linux

 Methodology

A TCP SYN scan was conducted using Nmap to discover open ports and identify services running on the target system.

 Command Used

nmap -sS -sV <target-ip>


 Results

| Port | Service | State 

 22    SSH      Open  
 80    HTTP     Open  
 443   HTTPS    Open  

 Findings

* SSH service was accessible on port 22.
* Web services were running on ports 80 and 443.
* Service version detection provided additional information useful for further security assessment.

 Risk Assessment

Open services may increase the attack surface of a system if they are misconfigured, outdated, or exposed unnecessarily.

 Recommendations

* Restrict access to administrative services such as SSH.
* Regularly update and patch exposed services.
* Disable unnecessary services and ports.
* Implement firewall rules to limit unauthorized access.

 Conclusion

The reconnaissance phase successfully identified active services and open ports on the target machine. The collected information can be used for further vulnerability assessment and security analysis.

