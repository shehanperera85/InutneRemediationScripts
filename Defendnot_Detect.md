**About the Script**
<br>
Since we need this to be identified sooner rather than later, if the device is enrolled in Intune, we can use a Remediation script to detect and report the event logs. My goal is to detect the Application Event ID 15 and notify it via Microsoft Teams.

I'm using a Webhook to create the script and my report-back method, wrap it as a PowerShell script, and create the remediation script policy in Intune to run hourly. This will look at the latest event and notify. Surely the script can be modified as you need, so it will not flood your alerts.

1. Create the Webhook Using Microsoft Teams.
2. Create the detection script.
3. Create the remediation (in this case action) script.
<br><br>
**Generated Event** Log<br>
![Screenshot 2025-05-23 111400](https://github.com/user-attachments/assets/f7cec1b2-31cb-4890-a4f7-2cac41446be3)
<br><br>
**Teams Notification**<br>
![Screenshot 2025-05-23 111138](https://github.com/user-attachments/assets/19089a7d-f919-496a-a6a4-9596e161fdc4)
