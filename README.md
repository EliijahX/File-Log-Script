# Log Analyzer Script
This Python script analyzes SSH log files (such as /var/log/auth.log) to help identify common security-related events. It focuses on three key areas:

1. IP addresses making connections

2. Invalid user login attempts

3. Failed login attempts by username
# 
Features
IP Address Tracking: Counts how many times each IP address appears in the log.

Invalid User Detection: Counts login attempts using non-existent usernames.

Failed Login Monitoring: Tallies failed password attempts for each username.
# 
Output Files
After the script runs, it creates three text files with summarized results:

max.txt: Contains the number of times each IP address appears.

invalid_users_output.txt: Shows how many "Invalid user" attempts were found.

failed_logins_output.txt: Lists failed login attempts by username.

Requirements
Python 3.x

A log file with SSH authentication events (e.g., auth.log, secure.log, or any file in similar format)
