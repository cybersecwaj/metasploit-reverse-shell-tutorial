<h1>JWipe - Disk Sanitization</h1>

 ### [YouTube Demonstration](https://youtu.be/7eJexJVCqJo)

<h2>Description</h2>
Project consists of a simple PowerShell script that walks the user through "zeroing out" (wiping) any drives that are connected to the system. The utility allows you to select the target disk and choose the number of passes that are performed. The PowerShell script will configure a diskpart script file based on the user's selections and then launch Diskpart to perform the disk sanitization.
<br />


<h2>Languages and Utilities Used</h2>

- <b>PowerShell</b> 
- <b>Diskpart</b>

<h2>Environments Used </h2>
[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/bpkukRnADlQ/0.jpg)](https://www.youtube.com/watch?v=bpkukRnADlQ)

- <b>Windows 10</b> (21H2)

<h2>Program walk-through:</h2>

<p align="center">

Launch the utility: <br/>
<img src="https://i.imgur.com/62TgaWL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Select the disk:  <br/>
<img src="https://i.imgur.com/tcTyMUE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Enter the number of passes: <br/>
<img src="https://i.imgur.com/nCIbXbg.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Confirm your selection:  <br/>
<img src="https://i.imgur.com/cdFHBiU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Wait for process to complete (may take some time):  <br/>
<img src="https://i.imgur.com/JL945Ga.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Sanitization complete:  <br/>
<img src="https://i.imgur.com/K71yaM2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Observe the wiped disk:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>


# Metasploit Reverse Shell Tutorial

Welcome to the Metasploit Reverse Shell Tutorial! This tutorial is designed to help you understand how to create and use a reverse shell payload using Metasploit, a popular penetration testing framework.

## What is a Reverse Shell?

A reverse shell is a type of shell where the target machine initiates the connection to the attacker's machine. This allows the attacker to gain shell access to the target system, enabling them to execute commands remotely.

## Prerequisites

Before proceeding with this tutorial, make sure you have the following prerequisites installed:
<iframe width="560" height="315" src="https://www.youtube.com/embed/YOUR_VIDEO_ID_HERE" frameborder="0" allowfullscreen></iframe>
- Metasploit Framework
- Kali Linux or any other Linux distribution with Metasploit installed
- Basic knowledge of command-line interface (CLI) and networking concepts

## Usage

1. **Generate Payload:** Use Metasploit to generate a reverse shell payload. You can customise the payload according to your requirements, such as the target platform and listening IP/port.
   
2. **Set Up Listener:** Start a listener on your machine to receive the incoming connection from the target. Make sure to specify the same IP and port as used in the payload.

3. **Execute Payload:** Execute the generated payload on the target system. Once executed, the target machine will establish a connection to your listener, providing you with a shell session.

4. **Explore and Control:** Once the connection is established, you'll have shell access to the target system. You can now execute commands, transfer files, or perform various tasks as per your requirement.

## Disclaimer

This tutorial is for educational purposes only. Do not use the techniques described herein for any malicious purposes. I am not responsible for any damage caused by the misuse of the information provided in this tutorial.

## Contributing

If you find any issues or have suggestions for improvement, feel free to open an issue or submit a pull request.

## Licence

This project is licensed under the MIT Licence - see the [LICENSE](LICENSE) file for details.