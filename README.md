# change_velocity

### Variables alrady set FOR YOU across the JLLT-Apps organization:

# SECRETS
#
# SN_ORCHESTRATION_TOOL_ID
# - this is the ID associated with the Devops Change Velocity module installed into ServiceNow
#
# SN_DEVOPS_INTEGRATION_TOKEN
# - this is the JWT token used for authentication between the JLLT-Apps GitHub application called
# "jllt-change-velocity" and the JLL production ServiceNow instance

# VARIABLES
#
# SN_INSTANCE_URL
# - this is the URL of the JLL production ServiceNow instance


### Variables YOU SHOULD SET in your repo to enhance the content of your ServiceNow change records

# SN_ASSIGNMENT_GROUP_SYS_IDSN_ASSIGNMENT_GROUP_SYS_ID (required)
# - This is the unique ID for your team's service now assignment group
#
# *HOW DO YOU FIND YOUR TEAM's SYS ID?
#
#  METHOD #1
#  (1) - In your service now instance (e.g. jll.service-now.com), on the top menu select ALL ->
#  USERS -> GROUPS.
#  (2) - Near the top of the page in the action header next to "Groups" is a drop down.  Select
#  "Name" and in the Search field enter your ServiceNow group name.  Hit Enter to execute the
#  search.
#  (3) - Once you find your group in the list, right-click on the name of the group (a hyperlink) 
#  and select "Copy Sys_id".  This will be Value for the variable "SN_ASSIGNMENT_GROUP_SYS_ID"
#
# Example of a group sys_id:  c26e367d9343a210cd38fde08bba10e3
#
#
#  METHOD #2
#  In case "Copy sys_id" isn't an option based on your ServiceNow role, try this instead:
#  (1) - In your service now instance (e.g. jll.service-now.com), on the top menu select ALL ->
#  USERS -> GROUPS.
#  (2) - Near the top of the page in the action header next to "Groups" is a drop down.  Select
#  "Name" and in the Search field enter your ServiceNow group name.  Hit Enter to execute the
#  search.
#  (3) - Once you find your group in the list, click the name of the group (a hyperlink).  This
#  open group profile page.  In the brower's URL field, the sys_id will be imbedded.
#
#  Example group record URL: 
#  <your org name>.service-now.com/../../../sys_user_group.do%##sys_id##<your 32 char sys id>.   
#  
# Please NOTE it is 32 characters long.  ServiceNow sometimes leads the actual sys_id with 
# two characters like "3D" or "3F". Capture the next 32 characters before the next "%##".



# SN_ASSIGNED_TO_SYS_ID (optional)
# - This is the unique ID for you or a member on your team whose name can be assigned as owner of
# change records created under your workflows in this repos
#
# *HOW DO YOU FIND A PERSON'S SYS ID?
#
#  METHOD #1
#  (1) - In your service now instance (e.g. jll.service-now.com), on the top menu select ALL ->
#  USERS.
#  (2) - Near the top of the page in the action header next to "Users" is a drop down.  Select
#  "Name" and in the Search field enter the individuals first name <space> last name.  Hit Enter
# to execute the search.
#  (3) - Once you find the person in the list, right-click on the name (a hyperlink) 
#  and select "Copy Sys_id".  This will be Value for the variable "SN_ASSIGNED_TO_SYS_ID"
#
#  Example of a user sys_id:  5edf55fd934b6210cd38fde08bba10a0
#
#  METHOD #2
#  In case "Copy sys_id" isn't an option based on your ServiceNow role, try this instead:
#  (1) - In your service now instance (e.g. jll.service-now.com), on the top menu select ALL ->
#  USERS.
#  (2) - Near the top of the page in the action header next to "Users" is a drop down.  Select
#  "Name" and in the Search field enter individuals first name <space> last name.  Hit Enter to
#  execute the search.
#  (3) - Once you find your user in the list, click the name of the person (a hyperlink).  This
#  open user profile page.  In the brower's URL field, the sys_id will be imbedded.
#
#  Example group record URL: 
#  <your org name>.service-now.com/../../../sys_user_.do%##sys_id##<your 32 char sys id>.   
#  
# Please NOTE it is 32 characters long.  ServiceNow sometimes leads the actual sys_id with 
# two characters like "3D" or "3F". Capture the next 32 characters before the next "%##".



