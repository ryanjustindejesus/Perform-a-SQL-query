<h1>Performing a SQL query </h1>



<h2>Description</h2>
In this lab, I learned how to retrieve information from a database using SQL. I will be using the MariaDB shell to run my SQL queries.
<br />


<h2>Practical experience gained in this Lab</h2>

- <b>Selecting specific columns from a table</b> 
- <b>Selecting all columns from a table by using an asterisk</b>
- <b>Sorting query results using the ORDER BY keyword</b> 


<h2>Environments Used </h2>

- <b>Qwiklabs</b> 

<h2>Lab walk-through:</h2>

<h2>Task 1: Retrieve employee device data </h2>
In this task, I obtained information on employee devices because my team needs to update them. The information I need is in the machines table in the organization database.
 <br/> <br/>
(1) First, I used the query "SELECT * FROM machines;" to retrieve all the information about the employee devices. 
<br/> <br/>  <p align="center">
<img src="https://imgur.com/1EdrAcB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 
<br /> <br /> 
(2) Next, I used the query "SELECT device_id, email_client FROM machines;" to focus on the email client running on various devices.
<br/> <br/> 
<img src="https://imgur.com/DDBWpUn.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 
<br /> <br /> 
(3) Finally, I used the query "SELECT device_id, operating system, OS_patch_date FROM machines;" to find information on the operating systems used on various devices and their last patch date.
<br/> <br/> 
<img src="https://imgur.com/lUp8QBM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 
<br /> <br /> 

<h2>Task 2: Investigate login activity </h2>
In this task, I analyzed the information from the `log_in_attempts` table to determine if any unusual activity has occurred.
 <br/> <br/> 
(1) First, I used the query "SELECT event_id, country FROM log_in_attempts;" to investigate the locations where login attempts were made to ensure that they’re in expected areas (the United States, Canada, or Mexico). 
<br /> <br /> <p align="center">
<img src="https://imgur.com/rKcX2nX.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 
<br /> <br />
(2) Next, I used the query "SELECT username, login_date, login_time FROM log_in_attempts;" to check if login attempts were made outside of the organization's working hours.
<br /> <br /> 
<img src="https://imgur.com/SposxtI.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 
<br /> <br />
(3) Finally, I used the query "SELECT * FROM log_in_attempts;" to get a complete picture of all login attempts. 
<br /> <br />
<img src="https://imgur.com/lg2Imwp.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 
<br /> <br />

<h2>Task 3: Order login attempts data </h2>
In this task, I used the `ORDER BY` keyword to sequence the data that my query returns according to the login date and time.
 <br/> <br/> 
(1) First, I used the query "SELECT * FROM log_in_attempts ORDER BY login_date; to sort the information by date. 
<br /> <br /> <p align="center">
<img src="https://imgur.com/3zwFG02.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 
<br /> <br />
(2) Finally, I used the query "SELECT * FROM log_in_attempts ORDER BY login_date, login_time; to further organize the previous results by ordering them by login_time.  <br/>
<p align="center">
<img src="https://imgur.com/4eTaUX2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 
