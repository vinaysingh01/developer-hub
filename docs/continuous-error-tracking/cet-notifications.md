---
title: Notifications
description: Notify your team when an event occurs.
sidebar_position: 4
---

# CET notifications

You can set up notifications to alert your team whenever new, resurfaced, or critical events occur. These events can include exceptions, log events, or custom events.
With these alerts, you can ensure that your team is aware of important events and takes appropriate action as needed.

To set up notifications in CET:

1. In your Harness project, go to **Continuous Error Tracking** > **Monitored Services**, and then select the monitored service for which you want to set up notifications.

2. On the monitored service details page, go to the **Notifications** tab and select **+ New Notification Rule**.  
   
   The New Notification wizard appears.

3. In the New Notification wizard, enter a name for the notification and select **Continue**.

4. On the Conditions page, select one of the following notification formats to define when you wish to receive a notification:
     - **Aggregate**: Receive an aggregate of events over a specified duration defined by the **Event Volume Threshold** settings.
     - **Immediate**: Get notified as soon as an event occurs.

5. You can configure notification settings to receive alerts for specific events by choosing a saved filter setting that you have created in the Events tab of the Events Summary page. When you select a saved filter setting, notifications are sent only for the events specified by that filter. If you wish to filter notifications for particular events, select your desired saved filter settings from the dropdown.

6. If you wish to receive an aggregate of all events when the event volume reaches a certain threshold, then select **Event Volume Threshold**, and specify the threshold value and notification frequency. For example, set up a notification to trigger every 5 minutes if the event volume exceeds 80.

7. Optionally, add multiple conditions by selecting **+ Add Condition**.
   
8. Select **Continue** to go to the Notification Method page.

9.  Select a **Notification Method**, such as Slack or Email, and complete the following settings:

   
     | Notification Method | Settings |
     | ------------------- | -------- |
     | **Slack**               |    Enter the **Slack Webhook URL** to which the notification should be sent.   |
     | **Email**               |    Enter the email addresses to which the notifications should be sent.      |

        
     If you choose Slack as your notification method, you can select a Harness user group that is part of a Harness project, organization, or account. Notifications are sent to the Slack channels that are associated with the selected user group.

     To create a new user group, click on **Select User Group(s)** and then **+ User Group**. In the New User Group dialog, enter a name for the group, an optional **description**, and **tags**, and then **Add Users**. Select **Save**. The new user group appears in the user group list.
   
10. Select **Test** to verify that the alert is functioning correctly.

11. Select **Finish** to save the settings. The notification rule appears in the **Notifications** section. 

12. Enable the notification rule by toggling the switch to start receiving alert notifications.

