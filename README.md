<h1>Network Traffic Investigation</h1>

<h2>Description</h2>
This project involves analyzing network traffic using Wireshark and hex editing tools to identify and extract suspicious files. The investigation focuses on HTTP traffic, file signature identification, and forensic file reconstruction.
<br />
<br />



<h2>Highlights:</h2>


<p align="center"> 
<h4 align="center">
Logical diagram of lab: <br/>
<br/>
<img src="https://github.com/user-attachments/assets/711558cd-cb0a-4baf-81e7-bebf9aaf28ae" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<h4 align="center">
The Agent has now been set up in Wazuh:  <br/>
<br/>
<img src="https://github.com/user-attachments/assets/68815baf-ea4b-4230-aac9-1803a5ef2cce" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<h4 align="center">
The tested alert was generated because Mimikatz was executed using a different image field value. The alert system was configured to look at the original FileName, hence why the alert: <br/>
<br/>
<img src="https://github.com/user-attachments/assets/421550f1-169b-4c00-adf8-896c0e4d5d82" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<h4 align="center">
Utilized shuffle to build a workflow; Wazuh was able to send an alert to shuffle:  <br/>
<br/>
<img src="https://github.com/user-attachments/assets/8b64bbb0-7560-440e-b888-dbc0e26ddb0a" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<h4 align="center">
Wazuh alerts Shuffle of Mimikatz; Shuffle checks the file hash on VirusTotal and sends details to TheHive to generate an alert. An analyst will also receive an email to start investigating:  <br/>
<br/>
<img src="https://github.com/user-attachments/assets/fc53e4ba-5494-4619-b823-658acb705530" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<h4 align="center">
The Agent has now been set up in Wazuh:  <br/>
<br/>
<img src="https://github.com/user-attachments/assets/4f98a4c7-466d-4d4d-8490-dd6674be5eb3" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<h4 align="center">
The Agent has now been set up in Wazuh:  <br/>
<br/>
<img src="https://github.com/user-attachments/assets/fc0dad94-8e3b-49b3-91fe-0e0d071315cc" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<h4 align="center">
The Agent has now been set up in Wazuh:  <br/>
<br/>
<img src="https://github.com/user-attachments/assets/d3957845-d8ed-46ed-86e4-4396d10ff31a" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<h4 align="center">
The Agent has now been set up in Wazuh:  <br/>
<br/>
<img src="https://github.com/user-attachments/assets/0b05f5bc-7e51-4fc4-a00c-951726859688" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
</p>

<br />

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
