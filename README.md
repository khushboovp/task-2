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
