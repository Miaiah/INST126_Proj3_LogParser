# INST126_Proj3_LogParser

Team member: Mingqian Huang

## Project Description
The program will based on the userlog.log to analyize and generate automated reports of different behavior. The reports will include 3 kinds of behavior: Suspicious activities, Irresponsible behavior, and System glitch. Each types of behavior will be counted for each user.\
When a user logs into any systems more then 5 times in one day or log in between 12:00am to 5:00am, will marked as Suspicious Activities. \
The program will also detect Irresponsible Behaviors when user forget to logout after login based on the number of logins and logouts. \
If the number of logouts is more than the number of logins, it will be marked as System Glitched. \
Finally, the program will list out all the domains and the number of users registered within each domain, each domain will only appear once.

## Project Flow
The flow for solving the project starts from first parsing the use log file and storing the user activity information into a log dictionary. \
Then by using the log dictionary, generate seperate dictionaries for Suspicious Activities, Irresponsible Behaviors and System Glitches. Then use the write report function to write the reports for each activity using title, file name, activity dictionary, activity count and log dictionary. \
Finally, count the domains and their user counts and write the report for Domain Count.