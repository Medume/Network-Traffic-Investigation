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
<img src="https://github.com/MichaelOmali/SOC-Automation-Lab/assets/163071085/63f7e41f-299a-4dd2-8f3b-7e8eb6eef3eb" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<h4 align="center">
The Agent has now been set up in Wazuh:  <br/>
<br/>
<img src="https://github.com/MichaelOmali/SOC-Automation-Lab/assets/163071085/be3c7121-b135-455c-ab66-cb35b94f6dcf" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<h4 align="center">
The tested alert was generated because Mimikatz was executed using a different image field value. The alert system was configured to look at the original FileName, hence why the alert: <br/>
<br/>
<img src="https://github.com/MichaelOmali/SOC-Automation-Lab/assets/163071085/8d0edf7e-3179-4e43-8116-e67838c4548d" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<h4 align="center">
Utilized shuffle to build a workflow; Wazuh was able to send an alert to shuffle:  <br/>
<br/>
<img src="https://github.com/MichaelOmali/SOC-Automation-Lab/assets/163071085/f20f3f76-7de0-4cab-bdcc-67da3d92d85b" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<h4 align="center">
Wazuh alerts Shuffle of Mimikatz; Shuffle checks the file hash on VirusTotal and sends details to TheHive to generate an alert. An analyst will also receive an email to start investigating:  <br/>
<br/>
<img src="https://github.com/MichaelOmali/SOC-Automation-Lab/assets/163071085/b85cc255-73ce-4027-a1b3-61a63e747ace" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<h4 align="center">
The Agent has now been set up in Wazuh:  <br/>
<br/>
<img src="https://github.com/MichaelOmali/SOC-Automation-Lab/assets/163071085/be3c7121-b135-455c-ab66-cb35b94f6dcf" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<h4 align="center">
The Agent has now been set up in Wazuh:  <br/>
<br/>
<img src="https://github.com/MichaelOmali/SOC-Automation-Lab/assets/163071085/be3c7121-b135-455c-ab66-cb35b94f6dcf" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<h4 align="center">
The Agent has now been set up in Wazuh:  <br/>
<br/>
<img src="https://github.com/MichaelOmali/SOC-Automation-Lab/assets/163071085/be3c7121-b135-455c-ab66-cb35b94f6dcf" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<h4 align="center">
The Agent has now been set up in Wazuh:  <br/>
<br/>
<img src="https://github.com/MichaelOmali/SOC-Automation-Lab/assets/163071085/be3c7121-b135-455c-ab66-cb35b94f6dcf" height="80%" width="80%" alt="Disk Sanitization Steps"/>
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
