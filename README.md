# CyberDefender--PsExec-Hunt


PsExecHunt – Network Forensics & Lateral Movement Investigation

Project Overview

This project involved investigating PCAP files from a CyberDefenders challenge, PsExecHunt, to understand how an attacker gained access to a system and performed lateral movement within a network.

The investigation focused on identifying suspicious network activity, analysing SMB communication, examining administrative share access, and tracing attacker activity through TCP streams.

Investigation & Analysis

1. Network Traffic Analysis

* Analysed PCAP files using Wireshark.
* Reviewed network conversations to identify suspicious communication patterns.
* Identified the suspected attacker IP address by examining conversation statistics and traffic details.

2. TCP Stream Analysis

* Used the Follow TCP Stream feature to reconstruct communication between systems.
* Examined the exchanged data to understand the attacker’s activities and communication patterns.
* Investigated relevant network streams for evidence of remote system access.

3. SMB & Administrative Share Investigation

* Analysed SMB2 traffic to understand remote access and authentication activity.
* Investigated connections to Windows administrative shares:
    * IPC$ – Interprocess Communication.
    * ADMIN$ – Administrative share mapped to the Windows directory.
* Examined SMB2 Tree Connect requests and responses to understand share access.

4. PsExec & Lateral Movement Investigation

* Investigated the abuse of PsExec for remote system access and lateral movement.
* Examined evidence of malicious executable deployment on the target system.
* Traced network communication associated with the attacker’s remote execution activity.

Tools & Technologies

* Wireshark
* PCAP Analysis
* SMB / SMB2
* TCP Stream Analysis
* Windows Administrative Shares
* PsExec
* Network Forensics

Key Takeaways

* Understanding SMB2 communication and Windows administrative shares.
* Identifying suspicious network conversations.
* Reconstructing network communication using TCP streams.
* Recognising potential PsExec abuse and lateral movement techniques.
* Understanding how attackers can leverage legitimate Windows administration mechanisms for malicious purposes.

Conclusion

This investigation provided practical experience in network traffic analysis, identifying suspicious communication, and understanding lateral movement techniques commonly observed in Windows environments.
