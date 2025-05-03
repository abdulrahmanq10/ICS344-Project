# Phase 3: This phase focuses on mitigating the vulnerabilities identified in earlier phases by implementing security hardening measures such as disabling anonymous FTP access, deploying intrusion prevention (Fail2Ban), and enforcing application confinement (AppArmor).
# Phase 3 work:
## Step 1-  Disable Anonymous FTP Login
Objective : Prevent unauthorized access via anonymous FTP login.
sudo apt-get install vsftpd
This replaces the default FTP service (proftpd) with vsftpd, a more secure alternative.
SCREENSHOT#1


### 1- Download Splunk Server .deb Package:
![p1](pictures/p1.png)

### 2- Installing the Splunk Server Package:
![p2](pictures/p2.png)

