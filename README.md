# Virtualization-and-Virtual-Machines

## Objective

This lab provides hands-on experience in a controlled environment using Oracle VirtualBox with Kali Linux and Metasploitable 2. It simulates real-world cybersecurity scenarios to enhance skills in penetration testing, vulnerability assessment, and network security through practical exercises.

### Skills Learned
- **Penetration Testing**: Conducting and analyzing attacks on Metasploitable 2.
- **Vulnerability Assessment:** Identifying and assessing security weaknesses.
- **Network Configuration:** Setting up and managing virtual networks in VirtualBox.
- **Ethical Hacking:** Using Kali Linux tools for ethical hacking practices.
- **Incident Response:** Handling and responding to simulated security incidents.
- Enhanced knowledge of network protocols and security vulnerabilities.
- Development of critical thinking and problem-solving skills in cybersecurity.

### Tools Used

- **Oracle VirtualBox:** Virtualization software for creating and managing virtual machines.
- **Kali Linux:** Linux distribution with tools for penetration testing and security analysis.
- **Metasploitable 2:** Vulnerable virtual machine for practicing penetration testing.
- **Nmap:** Network scanning tool for discovering hosts and services.
- **Metasploit Framework:** Penetration testing framework for exploiting vulnerabilities.
- **Burp Suite:** Web vulnerability scanner and security testing tool (if included in Kali Linux setup).

## Steps
### Step 1: Setting up of Virtual Home Lab
  -First of all we need a virtualisation application, I choose Oracle Virtual box. Make sure your laptop/PC supports virtualisation, if yes enable it.
  -Download and install Oracle Virtual box: https://www.virtualbox.org/
 ![Screenshot (344)](https://github.com/user-attachments/assets/80589bff-91d5-4cd4-8938-7c5ebc39be90)
  
  -Downloading and installing the Kali Linux ISO file, you can choose Kali Installer images (.iso) files or ready to launch kali pre-built virtual. I'm doing with kali installer image  https://www.kali.org/get-kali/#kali-installer-images. you can also use the direct link, https://cdimage.kali.org/kali-2024.2/kali-linux-2024.2-installer-amd64.iso
![Screenshot (345)](https://github.com/user-attachments/assets/d6f2a976-916b-462c-95bf-5ef11269b6de)

-Download and install Metasploitable 2, from here: https://sourceforge.net/projects/metasploitable/files/latest/download
What is Metasploitable 2? 
A Linux virtual machine (VM) that's intentionally vulnerable to attacks and can be used for security training, testing security tools, and practicing penetration testing techniques. It's compatible with VMware, VirtualBox, and other virtualization platforms.
![Screenshot (346)](https://github.com/user-attachments/assets/fcd456a3-a569-4b49-a98d-8281f5a39c4a)

-Now we need to add these two files into the oracle virtual box, Open virtual box and click "New" and proceed as the application prompts, repeat same step for the metasploitable 2 also. Then you will get the following. Ignore the other 2 virtual machines not needed for now.
![Screenshot (343)](https://github.com/user-attachments/assets/9daaeaf8-fc58-44ba-a498-c66b340d45e0)

### Step 2: Now switch ON the Kali Linux and Metasploitable2 machines.
 -You can practice some linux commands on the linux terminal, https://www.geeksforgeeks.org/linux-commands-cheat-sheet/
 ![Screenshot (347)](https://github.com/user-attachments/assets/ae811fa6-59bb-4375-b927-39c43d07fd8f)

 -After turning ON the metasploitable2 use default username and password is msfadmin:msfadmin respectively.
 ![metasploitable](https://github.com/user-attachments/assets/685665c3-b7a9-454f-998d-2a965aeb48eb)

-To do attack on the purposefully made vulnerable metasploitable2 machine, the attacker machine (here, Kali linux) is should be on the same network. With help of the Virtualbox application we can use the network configuration for the same, put both the machines on the ssme network.
![Screenshot (348)](https://github.com/user-attachments/assets/85ffb1f5-6b04-488b-ada4-317aa7891147)

### Setp 3: Using Kali linux to attack Metasploitable 2 machine
-Here are some common practice attacks you can perform using Kali Linux on Metasploitable 2:
 #### To get additional tools you like that is not available in kali linux default tool box, you can get it mainly from github and other sources also. Command to get additional tools for kali linux is can be from https://www.kali.org/tools/ and follow along the instructions. Get tools from GitHub for Kali linux, command 'git clone [url of the github respository]' 
1. **Port Scanning:**
   - **Tool:** Nmap
   - **Objective:** Identify open ports and services running on Metasploitable 2.

2. **Service Enumeration:**
   - **Tool:** Nmap, Netcat
   - **Objective:** Determine the versions and configurations of services.

3. **Vulnerability Scanning:**
   - **Tool:** OpenVAS, Nikto
   - **Objective:** Scan Metasploitable 2 for known vulnerabilities.

4. **Exploitation:**
   - **Tool:** Metasploit Framework
   - **Objective:** Exploit vulnerabilities such as outdated services or weak configurations to gain unauthorized access.

5. **Password Cracking:**
   - **Tool:** Hydra, John the Ripper
   - **Objective:** Perform brute-force attacks on login credentials.

6. **Web Application Attacks:**
   - **Tool:** Burp Suite, SQLmap
   - **Objective:** Test web applications on Metasploitable 2 for SQL injection, XSS, and other vulnerabilities.

7. **Privilege Escalation:**
   - **Tool:** Metasploit, LinPEAS
   - **Objective:** Escalate privileges from a user to root on Metasploitable 2.

8. **Man-in-the-Middle Attacks:**
   - **Tool:** Wireshark
   - **Objective:** Intercept and manipulate network traffic between Metasploitable 2 and other systems.

9. **Social Engineering Attacks:**
   - **Tool:** SET (Social Engineering Toolkit)
   - **Objective:** Simulate phishing attacks or other social engineering techniques.

10. **Post-Exploitation:**
    - **Tool:** Meterpreter (part of Metasploit)
    - **Objective:** Maintain access, gather information, and perform actions on Metasploitable 2 after gaining initial access.

These attacks help in understanding the security posture of systems and practicing defensive measures.

 
