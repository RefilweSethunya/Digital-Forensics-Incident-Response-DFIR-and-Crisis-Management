# Digital Forensics Incident Response (DFIR) and Crisis Management

Welcome to my documentation for Digital Forensics & Incident Response(DFIR) and Crisis Management learning — focused on digital evidence acquisition, forensic analysis, and incident investigation.

Digital forensics has become a foundational skillset for cybersecurity professionals. Today’s security landscape demands practitioners who can:
- Collect and preserve digital evidence
- Investigate malware and identify breach vectors
- Analyze system artifacts across operating systems
- Reconstruct timelines and attacker activity
- Respond to security incidents efficiently and defensibly
The course covers core forensic principles that apply universally, while also diving deep into platform-dependent investigation techniques for multiple operating systems (Windows, Linux, and macOS).

This repository is part of my broader commitment to learning out loud and includes the basic concepts and techniques usually employed in digital forensics and malware analysis. The contents are divided into the following modules:

# Course Modules Covered
Module 1:<br>
🔍 Lab 1 Collecting Volatile and Non-Volatile Data<br>
🔍 Lab 2 Automating Volatile Data Acquisition<br>
🔍 Lab 3 System Memory Acquisition<br>

Module 2:<br>
🔍 Lab 1 Hard Drive and Media Imaging,<br>
🔍 Lab 2 Analyzing Physical Memory,<br>
🔍 Lab 3 Disk Investigation and Analysis,<br>
🔍 Lab 4 Timeline Creation and Analysis<br>

Module 3:<br>
🔍 Lab 1 Data Recovery,<br>
🔍 Lab 2 Automating Digital Forensics Analysis<br>

Module 4:<br>
🔍 Lab 1 File Metadata,<br>
🔍 Lab 2 Geolocation and Metadata,<br>
🔍 Lab 3 Email Forensics,<br>
🔍 Lab 4 Web Server Forensics,<br>
🔍 Lab 5 Network Forensics<br>

# Tools Covered
Name | Command | Repository | Installation Method
-------|-------------|--------------- | -----------
sysinternals| | |
NirSoft Suite|  | 
DFIRTriage| | 
volatility|  |
rip.pl|  | 
log2timeline|  | 
psort.py|  | 
Timeline Explorer|  | 
sleuthkit|  | 
Foremost| | 
rifiuti|  | 
pasco|  | 
Autopsy|  | 
wmd.pl|  | 
pdfparser.py|  | 
exiftool| | 
Forensically|  | 
network tools|  | 
Tcpdump|  | 
Wireshark|  | 
Network Miner| | 


# Environment Setup
A secure and properly configured environment is essential when working with the labs. All analysis should be performed inside a dedicated virtual machine to prevent accidental system compromise and ensure clean, repeatable investigations. Using platforms such as VMware, VirtualBox, or Hyper-V, the VM should be provisioned with enough CPU, memory, and storage to comfortably support the required forensic tools and workloads.

Once the VM is prepared, install the necessary forensic tools( e.g Autopsy, Volatility, etc..) and ensure each tool is updated to its latest stable version.

To maintain reliability, take an initial VM snapshot after setup. This baseline creates a safe restore point should the system become corrupted or behave unpredictably during analysis.

So..
1. Install Virtualbox or any other virtualization solution of your choice
2. Import the kali Linux OVA into Virtualbox
3. For the labs we will use the following sample forensics images from [NIST's Computer Forensic Reference DataSet Portal](https://cfreds.nist.gov/) :<br>
   a)  Memory: https://cfreds-arhive.nist.gov/mem/memory-images.rar<br>
   b)  Jean: https://digitalcorpora.s3.amazonaws.com/corpora/drives/nps-2008-m57-jean/nps-2008-jean.E01<br>
   c)  Jean: https://digitalcorpora.s3.amazonaws.com/corpora/drives/nps-2008-m57-jean/nps-2008-jean.E02<br>
   d)  Dell_laptop: https://cfreds-arhive.nist.gov/images/4Dell%20Latitude%20CPi.E01<br>
   e)  Dell_laptop: https://cfreds-arhive.nist.gov/images/4Dell%20Latitude%20CPi.E02

# ⚠️ Important Notice

As part of my Digital Forensics & Incident Response (DFIR) training, this repository may reference or analyze artifacts that are typically found in real-world incident investigations.
Although no executables or live malware samples are hosted directly in this repository, the tools, techniques, and exercises I have documented are often used to analyze potentially harmful files.

To protect yourself and your systems use a virtual machine, sandbox, or isolated lab environment.

This repository is meant for educational purposes and professional growth.

![Malware Safety](https://img.shields.io/badge/Safety%20Notice-Malware%20Analysis%20Content-red?logo=alert)
