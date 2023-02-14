# Week 0 — Billing and Architecture

Setting Up Billing Alerts
Step 1: Go to the CloudWatch console
Navigate to https://console.aws.amazon.com/cloudwatch/

Step 2: Change the region
In the upper right hand corner, make sure your AWS region is set to US East (N. Virginia). This is the region where all billing data is stored.

Step 3: Create an alarm
Click on “Alarms” in the left side panel and in the dashboard that pops up click on the orange button that says “Create Alarm”.

Step 4: Select a metric
In the panel that pops up, click the button that says “select metric”. This will pop up a window that allows you to choose which type of service you’d like to use. Select “Billing”.

Step 5: Select the service
In the next window, you can choose to either base the alarm off a given service’s charges or the Total Estimated Charge on your account. We will set an alarm for our EC2 charges, so click “By Service”.

On the next step, mark the checkbox next to the specific service(s) you’d like to monitor. We’ll choose Amazon EC2.

Step 6: Select the time period
Next you’ll want to set the time period that the alarm will be active for. You can choose anything from 10 seconds to an entire day. The interface will also show a graph which plots your current usage in blue against the alarm threshold in red. If the blue line crosses the red at any point during the selected time period, the alarm will activate.

Step 7: Set the threshold
Next, set the threshold over or under which the alarm will ring. We’ll set our alarm to activate if our EC2 charges exceed $10 within the next 6 hours. You can also use the anomaly detection panel to specify a band around your usage outside of which you’d like the alarm to activate.

Step 8: Create a notification
Next you’ll want to create a notification using Amazon SNS. You just click “create new topic”, give it a name, and enter the email you’d like to be notified at into the box.

Step 9: Add a description
Now you can create a name and description that will help you to remember what trigger is set for your alarm.

Step 10: Preview and create
A final page will now open which summarizes and displays your alarm’s settings as you’ve created them. If everything looks good, you can click “Create Alarm” to have your alarm set.



# Architectural Logical Diagram of Cruddar App & CI/CD pipeline Diagram


<div style="width: 640px; height: 480px; margin: 10px; position: relative;"><iframe allowfullscreen frameborder="0" style="width:640px; height:480px" src="https://lucid.app/documents/embedded/aa7d9f25-3d6f-47e8-8835-bedc2ef08508" id="V32wKZ3HJUCE"></iframe></div>