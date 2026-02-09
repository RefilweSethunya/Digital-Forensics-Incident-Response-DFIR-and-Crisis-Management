# Digital Forensics Incident Response (DFIR) and Crisis Management

Welcome to my documentation for Digital Forensics & Incident Response(DFIR) and Crisis Management learning. It is focused on digital evidence acquisition, forensic analysis and incident investigation.

Digital forensics has become a foundational skillset for cybersecurity professionals. Today’s security landscape demands practitioners who can:
- Collect and preserve digital evidence
- Investigate malware and identify breach vectors
- Analyze system artifacts across operating systems
- Reconstruct timelines and attacker activity
- Respond to security incidents efficiently and defensibly
The course covers core forensic principles that apply universally, while also diving deep into platform-dependent investigation techniques for multiple operating systems (Windows, Linux, and macOS).

This repository is part of my broader commitment to learning out loud and includes the basic concepts and techniques usually employed in digital forensics and malware analysis. The contents are divided into the following modules:
<br>

# Course Modules Covered
## <img src="https://img.shields.io/badge/Module%201-Volatile%20%26%20NonVolatile%20Data-blue?style=for-the-badge" />
🔍 **[Lab 1 Collecting Volatile and Non-Volatile Data](DFIR-main/Module-01/Lab-01.md)**<br>
🔍 **[Lab 2 Automating Volatile Data Acquisition](DFIR-main/Module-01/Lab-02.md)**<br>
🔍 **[Lab 3 System Memory Acquisition](DFIR-main/Module-01/Lab-03.md)**<br>

## <img src="https://img.shields.io/badge/Module%202-Disk%20Imaging%20%26%20Memory%20Analysis-purple?style=for-the-badge" />
🔍 **[Lab 1 Hard Drive and Media Imaging](DFIR-main/Module-02/Lab-01.md)**<br>
🔍 **[Lab 2 Analyzing Physical Memory](DFIR-main/Module-02/Lab-02.md)**<br>
🔍 **[Lab 3 Disk Investigation and Analysis](DFIR-main/Module-02/Lab-03.md)**<br>
🔍 **[Lab 4 Timeline Creation and Analysis](DFIR-main/Module-02/Lab-04.md)**<br>

## <img src="https://img.shields.io/badge/Module%203-Data%20Recovery%20%26%20Automation-green?style=for-the-badge" />
🔍 **[Lab 1 Data Recovery](DFIR-main/Module-03/Lab-01.md)**<br>
🔍 **[Lab 2 Automating Digital Forensics Analysis](DFIR-main/Module-03/Lab-02.md)**<br>

## <img src="https://img.shields.io/badge/Module%204-Metadata%20%26%20Network%20Forensics-orange?style=for-the-badge" />
🔍 **[Lab 1 File Metadata](DFIR-main/Module-04/Lab-01.md)**<br>
🔍 **[Lab 2 Geolocation and Metadata](DFIR-main/Module-04/Lab-02.md)**<br>
🔍 **[Lab 3 Email Forensics](DFIR-main/Module-04/Lab-03.md)**<br>
🔍 **[Lab 4 Web Server Forensics](DFIR-main/Module-04/Lab-04.md)**<br>
🔍 **[Lab 5 Network Forensics](DFIR-main/Module-04/Lab-05.md)**<br>
<br>

# Tools Covered
Name | Command | Repository | Installation Method
-------|-------------|--------------- | -----------
sysinternals| | https://learn.microsoft.com/sysinternals/|
NirSoft Suite|  | https://www.nirsoft.net/
DFIRTriage| DFIRTriage.exe| 
volatility| vol.py -h | https://github.com/volatilityfoundation/volatility.githttps://github.com/volatilityfoundation/volatility.git | 
RegRipper| rip.pl -h | https://github.com/keydet89/RegRipper3.0 |
log2timeline| log2timeline.py -h | https://github.com/log2timeline/plaso
psort.py| psort.py -h | https://github.com/log2timeline/plaso
Timeline Explorer| TimelineExplorer.exe | 
sleuthkit| fls -h | https://github.com/sleuthkit/sleuthkit
Foremost| foremost -h| https://github.com/korczis/foremost
rifiuti| rifiuti -h | https://github.com/abelcheung/rifiuti2
pasco| pasco -h | 
Autopsy| autopsy | https://www.sleuthkit.org/autopsy/
wmd.pl| wmd.pl -h | https://github.com/williballenthin/wmd
pdfparser.py| pdfparser.py -h | https://github.com/DidierStevens/DidierStevensSuite
exiftool| exiftool -h| https://exiftool.org/
Forensically|  | 
network tools|  | 
Tcpdump| tcpdump -h | https://www.tcpdump.org/
Wireshark| wireshark |https://www.wireshark.org/ 
Network Miner|NetworkMiner.exe | 

<br>

# Environment Setup
A secure and properly configured environment is essential when working with the labs. All analysis should be performed inside a dedicated virtual machine to prevent accidental system compromise and ensure clean, repeatable investigations. Using platforms such as VMware, VirtualBox, or Hyper-V, the VM should be provisioned with enough CPU, memory, and storage to comfortably support the required forensic tools and workloads.

Once the VM is prepared, install the necessary forensic tools( e.g Autopsy, Volatility, etc..) and ensure each tool is updated to its latest stable version.

To maintain reliability, take an initial VM snapshot after setup. This baseline creates a safe restore point should the system become corrupted or behave unpredictably during analysis.

If you prefer a pre-configured setup, you may use the ready-to-import OVA file prepared for these labs which already includes the essential forensic tools and configurations needed to begin the exercises immediately.:<br>

🔗 Pre-built Kali Linux OVA (15.8GB)<br>
MEGA Download: https://mega.nz/file/OFMHHTYS#cqW0aA4n4Q0Mr2zHba2boK3xO5AF-ZJg-x3xDMl2Ui8

So..
1. Install Virtualbox or any other virtualization solution of your choice
2. Import the kali Linux OVA into Virtualbox using VirtualBox’s Import Appliance wizard
3. Verify that the VM starts correctly, then take an initial snapshot
4. For the labs we will use the following sample forensics images from [NIST's Computer Forensic Reference DataSet Portal](https://cfreds.nist.gov/) :<br>
   a)  Memory Image: https://cfreds-arhive.nist.gov/mem/memory-images.rar<br>
   b)  Jean: https://digitalcorpora.s3.amazonaws.com/corpora/drives/nps-2008-m57-jean/nps-2008-jean.E01<br>
   c)  Jean: https://digitalcorpora.s3.amazonaws.com/corpora/drives/nps-2008-m57-jean/nps-2008-jean.E02<br>
   d)  Dell_laptop: https://cfreds-arhive.nist.gov/images/4Dell%20Latitude%20CPi.E01<br>
   e)  Dell_laptop: https://cfreds-arhive.nist.gov/images/4Dell%20Latitude%20CPi.E02
<br>

# ⚠️ Important Notice

As part of my Digital Forensics & Incident Response (DFIR) training, this repository may reference or analyze artifacts that are typically found in real-world incident investigations.
Although no executables or live malware samples are hosted directly in this repository, the tools, techniques, and exercises I have documented are often used to analyze potentially harmful files.

To protect yourself and your systems use a virtual machine, sandbox, or isolated lab environment.

This repository is meant for educational purposes and professional growth.

![Malware Safety](https://img.shields.io/badge/Safety%20Notice-Malware%20Analysis%20Content-red?logo=alert)
