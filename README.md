# Task 2- Cloud Computing

**Name** : CODTECH IT SOLUTIONS

**Name** : Khushboo Vijay Patil

**Intern ID** : CT06DF672

**Domain** : Cloud Computing

**Duration** : 6 Weeks

**Mentor** : Neela Santosh

**Description of Task**

Step 1: Access AWS CloudWatch
Go to AWS Console
In the Services, search for and open CloudWatch

Step 2: Create a Log Group (if not already)
This is for storing logs from your application (EC2, Lambda, etc.)
Navigate to Logs > Log groups
Click on Create log group
Enter a name 
Click Create

Step 3: Enable Monitoring on Your Service
Go to EC2 Dashboard
Select your instance
In the Monitoring tab, click on View in CloudWatch
CloudWatch automatically collects basic metrics (CPUUtilization, NetworkIn/Out, etc.)
Optionally, install CloudWatch Agent on the EC2 for custom metrics (like memory, disk).

Step 4: Create a CloudWatch Alarm (Alert)
In CloudWatch, go to Alarms > Click Create Alarm
Click Select Metric
EC2 > Per-Instance Metrics > CPUUtilization
Select the instance and click Select metric
Set the conditions:
CPUUtilization > 80% for 5 minutes
Click Next
Create or select an SNS topic to notify via email or SMS
Add your email and confirm subscription
Name the alarm: HighCPUAlarm
Click Create alarm

Step 5: Create a Dashboard
In CloudWatch, go to Dashboards
Click Create dashboard
Name it
Choose widget types:
Line graph, Number, Text, etc.
Add widgets:
Add CPUUtilization, NetworkIn, etc., from EC2
Add Lambda invocation count, error count, duration, etc.
Adjust titles and graph setting
Click Save dashboard

Step 6: Test Alerts
Simulate high CPU usage (e.g., by running a load script)
Wait for 5 minutes to trigger the alarm
You should receive an email/SMS alert from CloudWatch

**OUTPUT**

![Image](https://github.com/user-attachments/assets/082d6fe0-5f33-4a7b-add1-90ae2ac73817)
![Image](https://github.com/user-attachments/assets/c1319b15-f14b-4ca7-8181-46009f823d13)
![Image](https://github.com/user-attachments/assets/980eac55-ee97-47a8-bd66-b153ee333d06)
![Image](https://github.com/user-attachments/assets/b3347647-db91-410b-a5dc-3f61a44745b1)
![Image](https://github.com/user-attachments/assets/ced95afb-2c41-4532-9b44-94672b8e6178)
![Image](https://github.com/user-attachments/assets/7684f655-5e4d-4d58-b3df-4348f38a31aa)
![Image](https://github.com/user-attachments/assets/ccebbda5-16db-453d-a0d7-c322a9ed6aff)
![Image](https://github.com/user-attachments/assets/c1046158-f5a7-4481-9014-b08a1a922825)
![Image](https://github.com/user-attachments/assets/8464a42d-fe1d-4da6-af0a-61fba9c92110)
![Image](https://github.com/user-attachments/assets/32bea412-1d5d-4021-8e14-a4f352e35e93)
![Image](https://github.com/user-attachments/assets/504cb674-782d-44de-a721-0ba240da3ea1)
![Image](https://github.com/user-attachments/assets/1af7b4d2-1a19-4c23-bbe7-df593090d5a4)
