<!-- About Me Section-->
## About me

<p>
  Hello 😀 my name is Katherine Tipan! I'm a rising junior at Baruch College majoring in Computer Information Systems with a concentration in Information Risk Management & Cybersecurity. I'm currently a candidate for the CompTIA Security+ certification.
</p>

<!-- Projects Section -->
## Projects
#### Cybersecuity Pathway Program
###### *Summer 2025 | CodePath CYB 102: Intermediate Cybersecurity*

<!-- Project 7 -->
<details>
	<summary>IOC Detection in Splunk</summary> <br>
	✔️ <strong>Objective:</strong> Constructed a Splunk search that compares network log activities (NetworkProxyLog02.csv) against the SolarWinds IOC list (SolarWindsIOCs.csv) to find any potential matches within the data.<br>
	⚙️ <strong>Tools:</strong> Splunk, VirusTotal<br>

<pre lang="sql">
	(index=main source="SolarWindsIOCs.csv") OR (index=main source="NetworkProxyLog02.csv")
	| stats values(source) as sources, values("Computer Name") as ComputerName, values("User Agent String") as UserAgent, values(Date) as Date, values(Time) as Time by "IP Address" 
	| where mvcount(sources) > 1
	| table "IP Address", ComputerName, UserAgent, Date, Time
</pre>  
📋 <strong>Output:</strong><br>
  <table>
    <tr>
    <img src="https://i.ibb.co/nqQSsV6p/search1.png" width=550>    
    </tr>
    <tr>
   <img src="https://i.ibb.co/21d6v871/virustotalsearch1.png" width=535>
   </tr>
  </table>
</details>

<!-- Project 1 -->
<details>
  <summary>Linux Auditing</summary>
	✔️ <strong>Objective:</strong> Configured Audit rules to monitor file changes, launched three attacks on unknown files, and used Audit logs with ausearch to identify which files were altered and which attack caused each change.<br>
	⚙️ <strong>Tools:</strong> Linux <br>
  📋 <strong>Procedure:</strong><br>
  <table>
    <tr>
      <td><img src="https://i.ibb.co/fGXQVHhH/Screenshot-177.png"></td>
    </tr>
  </table>
</details>

<!-- Project 2 -->
<details>
  <summary>Network Traffic Analysis</summary>
	✔️ <strong>Objective:</strong> Used Wireshark to analyze SMTP packets in .pcap files, extract email content, and identify the malicious actor through IP extraction.<br>
	⚙️ <strong>Tools:</strong> Wireshark, Linux <br>
  📋 <strong>Procedure:</strong><br>
  <table>
    <tr>
      <td><img src="https://i.ibb.co/NdC35DL9/Screenshot-190.png"></td>
    </tr>
  </table>
</details>

<!-- Project 3 -->
<details>
  <summary>Directory Traversal Attack</summary>
	✔️ <strong>Objective:</strong> Used bash scripting to launch a directory traversal attack on an FTP server and analyzed a .pcap file to identify unauthorized file access.<br>
	⚙️ <strong>Tools:</strong> Linux <br>
  📋 <strong>Procedure:</strong><br>
  <table>
    <tr>
      <td><img src="https://i.ibb.co/HfnnjSk2/Screenshot-186.png"></td>
      <td><img src="https://i.ibb.co/S48v19Pq/Screenshot-187.png "></td>
    </tr>
  </table>
</details>

#### Cybersecuity Fellowship
###### *Spring 2025 | America On Tech*

<!-- Project 4 -->
<details>
  <summary>NBCU Tabletop Exercise</summary>
  ✔️ <strong>Objective:</strong> Collaboratively developed an intrusion kill chain based on the LAPSUS$ & OKTA breach.<br>
  📋 <strong>Procedure:</strong> <a href="https://drive.google.com/file/d/1M_r0ji2iwQcg0l3zVUs9leVVgH_gyUmV/view?usp=sharing">NBCU Tabletop Group Project</a><br>
</details>

<!-- Project 5 -->
<details>
  <summary>File Encryption with EFS</summary>
	✔️ <strong>Objective:</strong> Encrypted a folder and its contents using EFS, then configured access permissions by adding an encryption certificate for a specific user.<br>
  📋 <strong>Procedure:</strong><br>
  <table>
    <tr>
      <td><img src="https://i.ibb.co/7NN0XQZR/Screenshot-200.png"></td>
      <td><img src="https://i.ibb.co/nNMW0JJy/Screenshot-201.png"></td>
    </tr>
  </table>
</details>

#### Cybersecuity Pathway Program
###### *Fall 2024 | CodePath CYB101: Intro to Cybersecurity*

<!-- Project 6 -->
<details>
  <summary>Penetration Testing</summary>
	✔️ <strong>Objective:</strong> Set up a vulnerable docker container, scanned it with Nmap to identify open ports & vulnerabilities, and exploited the vsftpd backdoor using Metasploit.<br>
	⚙️ <strong>Tools:</strong> Metasploit, Nmap, Linux <br>
  📋 <strong>Procedure:</strong><br>
  <table>
    <tr><td><img src="https://i.ibb.co/Q38xjDTR/Screenshot-191.png"></td></tr>
    <tr><td><img src="https://i.ibb.co/8LqDzLWN/Screenshot-192.png"></td></tr>
    <tr><td><img src="https://i.ibb.co/xtmQBpWR/Screenshot-193.png"></td></tr>
    <tr><td><img src="https://i.ibb.co/TqpSR1nf/Screenshot-195.png"></td></tr>
    <tr><td><img src="https://i.ibb.co/VWxzrGdT/Screenshot-196.png"></td></tr>
  </table>
</details>

<!-- Project 7 -->
<details>
  <summary>Threat Analysis</summary>
	✔️ <strong>Objective:</strong> Used OSINT tools to discover host IPs and identify associated CVEs from the returned JSON data.<br>
	⚙️ <strong>Tools:</strong> Shodan, Linux <br>
  📋 <strong>Procedure:</strong><a href="https://drive.google.com/file/d/1Q0fcZjUnsuKFcuTUnf6yjbz0m9ZC7g6-/view?usp=sharing"> Threat Analysis Project</a><br>
</details>
  
<!-- Project 8 -->
<details>
  <summary>SSH Keys</summary>
	✔️ <strong> Objective </strong> Generated SSH keys and used them for authentication. Used SSH keys and openssl to encrypt and decrypt a text file. Verified the integrity of a Git commit using SSH. <br>
	⚙️ <strong>Tools:</strong> Linux <br>
  📋 <strong>Procedure:</strong> <a href="https://drive.google.com/file/d/1z6rw6uab-2Lz9FZkbGbAHH9be4WQqCo2/view?usp=sharing">SSH Keys Project</a><br>
</details>

<!-- Connect Section -->
## Connect
<table>
  <tr>
    <td>
      <img src="https://img.icons8.com/?size=100&id=xuvGCOXi8Wyg&format=png&color=000000" width="30">
    </td>
    <td>
      <a href="https://www.linkedin.com/in/katherinetipan">linkedin.com/in/katherinetipan</a>
    </td>
  </tr>
</table>
