# Phase 2: Splunk Forwarder Integration

This phase demonstrates the process of setting up **Splunk Universal Forwarder** on the Metasploitable3 machine and forwarding logs to **Splunk Enterprise** running on Kali Linux. The steps include installation, configuration, and verification of successful log ingestion.

---

## Step 1: Download and Install Splunk Forwarder on Metasploitable

### 1. Download the Splunk Forwarder `.deb` Package
![Step 1](pictures/p1.png)

### 2. Install the Package
![Step 2](pictures/p2.png)

### 3. Start Splunk Forwarder and Accept the License
![Step 3](pictures/p3.png)

### 4. Enable Splunk Forwarder to Start on Boot
![Step 4](pictures/p4.png)

---

## Step 2: Configure the Forwarder to Send Logs

### 1. Add the Splunk Indexer (Kali Machine) as the Receiving Target
![Step 5](pictures/p5.png)

### 2. Add Log File for Monitoring (`/var/log/auth.log`)
![Step 6](pictures/p6.png)

---

## Step 3: Configure and Launch Splunk Enterprise on Kali Linux

### 1. Start Splunk Enterprise on Kali
![Step 7](pictures/p7.png)
![Step 8](pictures/p8.png)

### 2. Configure Splunk to Listen on Port `9997` for Incoming Logs
![Step 9](pictures/p9.png)

---

## Step 4: Final Steps and Verification

### 1. Restart Splunk Forwarder on Metasploitable
![Step 10](pictures/p10.png)

### 2. Confirm Logs Are Received and Indexed
![Step 11](pictures/p11.png)

### 3. Visualize and Analyze the Collected Logs
![Step 12](pictures/p12.png)

### 4. Verify the Logs on Metasploitable Are Consistent
![Step 13](pictures/p13.png)

The logs displayed in Splunk on Kali match those on the Metasploitable machine, confirming that log forwarding has been successfully configured and is working as intended.

---

## Conclusion

In this phase, we successfully:
- Installed and configured Splunk Universal Forwarder on Metasploitable.
- Set up log forwarding to a Splunk Enterprise instance on Kali Linux.
- Verified the complete pipeline from log generation to visualization.

This setup enables real-time log collection and monitoring from the target machine, which is essential for security event analysis.
