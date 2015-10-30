CS3219 Assignment 3
Team 16: Gary, Qiyuan, Yusuf, Amir
readme for changes in CodeCraft source

To use send announcement feature, click group settings button > make
announcement

***changes in this readme file is for changes made for part a, changes
in part b consist of the same changes + changes in gui.js popup functions to implement CodeCraft style GUI***
======================================================================
PART A
================================GUI.JS=================================
Line 1779: 
Receive socket message from server for announcement sent
Message: ANNOUNCEMENT_SENT
Call popup function to display announcement

Line 1805:
Receive socket message from server for all announcement read
Message: INFORM_OWNER_READ
If client is owner, call popup function to display notification

Line 2917:
Popop function for owner to make announcement
Emit socket message to server with announcment (line 2924)
Message: SEND_ANNOUNCEMENT

Line 3538:
Popup function for displaying of announcement
Emit socket message to server that announcement is received (line 3542)
Message: ANNOUNCEMENT RECEIVED

Line 3694:
Popup function to notify owner that all members have read announcement

Line 6202:
Button for owner to make announcement

==================================WWW==================================

Line 100:
"count" attribute for room data representing number of members who 
have read the latest announcement

Line 171:
Receive socket message from client to send announcement
Message: SEND_ANNOUNCEMENT
Emit socket message to client to that announcement is sent(line 179)
Nessage: ANNOUNCEMENT_SENT

Line 189:
Receive socket message from client for that announcement is received
by member
Message: ANNOUNCEMENT_RECEIVED
Once all members have read, emit socket message to client to inform owner Line
Message: INFORM_OWNER_READ (line 198)



======================================================================
PART B
================================GUI.JS=================================
Line 1779: 
Receive socket message from server for announcement sent
Message: ANNOUNCEMENT_SENT
Call popup function to display announcement

Line 1805:
Receive socket message from server for all announcement read
Message: INFORM_OWNER_READ
If client is owner, call popup function to display notification

Line 2917:
Popop function for owner to make announcement
Emit socket message to server with announcment (line 2924)
Message: SEND_ANNOUNCEMENT

Line 3038:
Popop function to inform the owner that an announcement has successfully been sent


Line 3715:
Popup function for displaying of announcement
Emit socket message to server that announcement is received (line 3542)
Message: ANNOUNCEMENT RECEIVED

Line 3856:
Popup function to notify owner that all members have read announcement

Line 6433:
Button for owner to make announcement

==================================WWW==================================

Line 100:
"count" attribute for room data representing number of members who 
have read the latest announcement

Line 171:
Receive socket message from client to send announcement
Message: SEND_ANNOUNCEMENT
Emit socket message to client to that announcement is sent(line 179)
Nessage: ANNOUNCEMENT_SENT

Line 189:
Receive socket message from client for that announcement is received
by member
Message: ANNOUNCEMENT_RECEIVED
Once all members have read, emit socket message to client to inform owner Line
Message: INFORM_OWNER_READ (line 198)

