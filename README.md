# FCMPushClient
# Descripition

This is a Simple Client for sending push notifications to Firebase Cloud Messaging service

# Usage


from push_notification_client import FCMPushClient

client=FCMPushClient(server_key, url)

notification={"title":"Testing Object", "body":"Testing Class", "icon":""}
registration_id="your_reg_id"

# Sending Single Notifications
client.send_single(registration_id,notification)


# Sending Multiple Notifications
reg_ids=["reg_id_1","reg_id_2"]
client.send_multiple(reg_ids,notification)

# Sending Topics

client.send_topic("topic_name",notification)


# Returns
JSON
{ "code":"00","msg":"Successfully Sent Notification"}


# Requires
JSON
requests



