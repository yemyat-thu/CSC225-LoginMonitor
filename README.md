### Login Monitor ###

Project Description 

This project is a python-based login monitoring system that analyzes login records to track failed login attempts, suspcious IP addresses, and accounts with multiple failed login attempts. It also tracks users who connect from multiple IP addresses, determines the busiest hour for login activity. and genertate security alerts based on the results. 

How to Run

It is important to have Python installed on the device. Download this python file and open the file in IDEs like VSCode or terminal and run by using 
"python assignment_starter_login_monitor.py" command. 

How busiest_hour() method works

The timestamps are extracted from self.parsed_logs using a for loop. I split each timestamp at the space to separate the date from the time. Then, I use string slicing ([:2]) to get the first two characters of the time, which represent the hour. To count the login attempts, I create an empty dictionary called hour_counts and increase the count by 1 for each login attempt during that hour. If there are no records, the method returns None. Otherwise, I use max() to find the hour with the highest number of login attempts and store it in busiest_hour. Finally, the method returns a tuple containing the busiest hour and the total number of login attempts during that hour.

