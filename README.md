# creating-a-backdoor-with-SET
creating a backdoor with SET - Ethical Hacking Techniques course

# AIM:
To Create a backdoor with Social Engineering Toolkit (SET)

## DESIGN STEPS:

### Step 1:

Install kali linux either in partition or virtual box or in live mode


### Step 2:

Investigate on the various categories of tools as follows:

### Step 3:

Open terminal and try execute some kali linux commands

## EXECUTION STEPS AND ITS OUTPUT:
Social Engineering attacks are the various cons used by the hackers to trick people into providing sensitive data to the attackers. 
The command sudo setoolkit in the prompt gives menu with set prompt:
## OUTPUT

<img width="1920" height="1200" alt="image - 1" src="https://github.com/user-attachments/assets/320ca4fa-b6d1-464e-8ef4-b5d024536d23" />

Explanation:

sudo → Runs the command with administrator (root) privileges.
setoolkit → Launches the Social Engineering Toolkit (SET).

Purpose:
SET is a penetration testing framework used for simulating social engineering attacks in authorized security labs.

What happens:

Opens the SET main menu
Displays attack modules like:
Social Engineering Attacks
Penetration Testing Tools
Third Party Modules
Update SET

The command sudo setoolkit in the prompt gives menu with set prompt. Select menu1 for Social Engineering Attacks:
## OUTPUT
<img width="1920" height="213" alt="image-2" src="https://github.com/user-attachments/assets/745e7223-c9ca-44e0-82eb-f29da6794636" />


Selection:

1

Explanation:
Chooses the Social Engineering Attack menu.

Purpose:
Contains modules to simulate attacks such as:

Credential harvesting
Spear phishing
Website cloning
Payload generation (authorized testing only)

It displays the following menu and select 2 for Website Attack Vectors:
## OUTPUT
<img width="1920" height="292" alt="image-3" src="https://github.com/user-attachments/assets/81675d89-fc44-4646-b6f9-9581449b94f2" />


Website Attack Vectors (Menu Option 2)

Selection:

2

Explanation:
Opens web-based attack simulation options.

Purpose:
Used for testing how users respond to cloned or simulated websites in controlled environments.

Options usually include:

Java Applet Attack
Metasploit Browser Exploit
Credential Harvester
Web Templates
Custom Import
The Credential Harvester Attack Method displays the following menu. In this menu1 for Web Templates is selected:
## OUTPUT

<img width="1920" height="816" alt="image-5" src="https://github.com/user-attachments/assets/ef1429a8-9ae1-41d7-8b78-7c3ef2ffd0a1" />


Selection:

3

(or the corresponding menu number shown)

Explanation:
Starts the credential harvester module.

Purpose:
Creates a simulated login page to demonstrate how credential phishing works during awareness training or lab exercises.

Function:

Hosts a fake login page
Collects submitted form data
Logs test submissions locally

It shows the following screen in which the ip address of the attacker need to be given which is the default value:
## OUTPUT

<img width="1920" height="349" alt="image-6" src="https://github.com/user-attachments/assets/9c58ba14-d9e4-4ec3-8910-50ef2ce87228" />


It shows the following screen in which the option Google can be selected:
## OUTPUT


<img width="1920" height="431" alt="image-7" src="https://github.com/user-attachments/assets/13841c36-8f31-4d18-ae02-d1503fa337c8" />


SET asks:

Enter the IP address for the POST back in Harvester

Explanation:
This is the IP address where the local test web server will listen.

Example:

10.50.252.7
Purpose:
Allows test machines on the same network to connect to the hosted simulation page.
SET starts my Kali Linux Webserver on port 80, with the fake Google account login page. The setup is done:
## OUTPUT

<img width="1920" height="189" alt="image-8" src="https://github.com/user-attachments/assets/df908a5b-f8f3-40dd-90c4-6e05c79dfc41" />



In windows IE, on giving the url http://192.168.1.2 (use appropriate IP address), the fake Google page is displayed. The victim can enter the username and password
## OUTPUT
<img width="1920" height="1200" alt="image-9" src="https://github.com/user-attachments/assets/192839e6-628a-4c0f-be37-8b04b59f9ccb" />


SET asks:

Enter the IP address for the POST back in Harvester

Explanation:
This is the IP address where the local test web server will listen.

Example:

192.168.1.2

Purpose:
Allows test machines on the same network to connect to the hosted simulation page.
SET logs the information regarding the Google credentials:
## OUTPUT
<img width="1920" height="486" alt="mage-10" src="https://github.com/user-attachments/assets/8eff9643-4fe8-4722-8fbf-7c3a2e10d2e2" />


2

(if Google corresponds to option 2)

Explanation:
Chooses the Google login template.

Purpose:
Loads a pre-made mock login page resembling Google for awareness demonstration.
SET logs the information in the xml file under /root/.set directory:
## OUTPUT
<img width="1920" height="1200" alt="hc" src="https://github.com/user-attachments/assets/47930c92-1a8f-4914-8c69-148afe656aa3" />












## RESULT:
The Social Engineering Toolkit (SET) is used to create backdoor is  examined successfully
