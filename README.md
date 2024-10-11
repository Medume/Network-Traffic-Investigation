<h1>Network Traffic Investigation</h1>

<h2>Description</h2>
This project involves analyzing network traffic using Wireshark and hex editing tools to identify and extract suspicious files. The investigation focuses on HTTP traffic, file signature identification, and forensic file reconstruction.
<br />
<br />



<h2>Highlights:</h2>


<p align="center"> 
<h4 align="center">
The first action to take in this task is filtering the network traffic so you can view just the http traffic. This makes it easier to find the packets created when the user requested files for download: <br/>
<br/>
<img src="https://github.com/user-attachments/assets/711558cd-cb0a-4baf-81e7-bebf9aaf28ae" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<h4 align="center">
Then search through the filtered traffic until you find a GET request for the image:  <br/>
<br/>
<img src="https://github.com/user-attachments/assets/68815baf-ea4b-4230-aac9-1803a5ef2cce" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<h4 align="center">
Next, after finding the packet, right click on it, navigate to the follow option and select TCP stream. This brings up the TCP stream that contained the image download: <br/>
<br/>
<img src="https://github.com/user-attachments/assets/421550f1-169b-4c00-adf8-896c0e4d5d82" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<h4 align="center">
When looking for a jpg image, the best way to find that will be by searching for a jpgs file signature. This This is done by changing the view of the data from ascii to raw, allowing you to view the hex data sent over the network. Then search for the jpeg hexadecimal file signature "FFD8" in the search bar at the bottom. This shows where the data for the image begins:  <br/>
<br/>
<img src="https://github.com/user-attachments/assets/8b64bbb0-7560-440e-b888-dbc0e26ddb0a" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<h4 align="center">
Then searching for the file footer of a jpeg, "FFD9", will show you where the image data ends:  <br/>
<br/>
<img src="https://github.com/user-attachments/assets/fc53e4ba-5494-4619-b823-658acb705530" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<h4 align="center">
Then copy all of the data between the two file signatures:  <br/>
<br/>
<img src="https://github.com/user-attachments/assets/4f98a4c7-466d-4d4d-8490-dd6674be5eb3" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<h4 align="center">
Now paste the data into a hex editor:  <br/>
<br/>
<img src="https://github.com/user-attachments/assets/fc0dad94-8e3b-49b3-91fe-0e0d071315cc" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<h4 align="center">
Save the file as a jpg image:  <br/>
<br/>
<img src="https://github.com/user-attachments/assets/d3957845-d8ed-46ed-86e4-4396d10ff31a" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<h4 align="center">
Opening this image in the Paint app, for example, will let you see the image the user downloaded:  <br/>
<br/>
<img src="https://github.com/user-attachments/assets/0b05f5bc-7e51-4fc4-a00c-951726859688" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<h4 align="center">
Here are the rest of the jpg images the user downloaded:  <br/>
 
<br />

[Bankcard JPG](https://ibb.co/TK9QM4w) 
<br />
[ATM Image JPG](https://ibb.co/JpDC8tw) 
<br />
[ANZ1 JPG](https://ibb.co/G7GmN37) 
<br />
[ANZ2 JPG](https://ibb.co/PTn0PW0)
<br/>
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
