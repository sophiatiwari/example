# example
new

**************************************************************************README****************************************************************************************

Introduction:

	The system automate the procedure of booking a meeting room in a company.Emplyees can search and book a meeting room based on thier requirement.

Prerequisites:
	
	1)Spring tools suite - Spring Tools Suite 4.4.0.0
			     Spring Tools Suite is used as developmentId for developing this project,Java is used for developing this application.
			     Link to download -

	2)Apache Derby       - Version 10:13.1 
			     This tool is used for Database purpose, Derby database is used in backed.
			     Link to download - https://db.apache.org/derby/releases/release-10.13.1.1.html

	3)Apache tomcat	     - Version 9.0
			     This is internal server used to run web application.
			     Link to download - https://tomcat.apache.org/download-90.cgi


Required jar files:
	
	1)derby.jar	     - Contains java classes which require to perform database operations.

	2)commons-fileupload-1.3
			     - Contains java classes which require to perform file opeations.

	3)commons-io-2.2
			     - Contains java classes which require to perform file operations.


Step by step guide for how to import this project into your systems:
	
	1)Clone project from git

	2)Open Spring tools suite

	3)File -> Import -> Existing Maven Project -> Next -> Browse (select directory where cloned) -> select checkbox Add project to working set -> finish.

	4)Windows in sts -> Show View -> Others -> Search server -> select server and open -> click on the link "No server available" -> Apache -> Tomcat v9.0 Server
																		-> Browse directory where you have install tomcat
																		-> next -> select meetingRooms and add
																		-> finish.

	5)Right click on meetingRooms project in Package Explorer -> select properties -> Targeted Runtimes -> select checkbox of Apache tomcat -> Apply and close. 
										       -> Java Build Path -> Order and Export -> select all -> apply and close.  

	6)In meetingRooms project directory -> click src -> main -> webapp -> Right click WEB-INF ->New -> create "lib" folder.
													-> copy all jar files inside lib folder.
													-> Right click on jar files starting with "commons".
														->Build path -> add to build path.
													->do this for both jar files starting with "commons" one by one.

	7)Refresh and clean the project.


How to connect to your derby database:

	1)Open directory where you have installed derby

	2)bin -> Open "ij.bat" file.

	3)Create database , for example - connect 'jdbc:derby:c:/database/meetingRoomsDB;create=true;user=admin;password=admin';

	4)All required tables and data are provided in dump.sql, copy everythig from dump.sql and paste in console of "ij.bat".

	5)Now,application is ready to use.


Git repository:

	1).application folder -
			      
			      This folder contains all the source code of the project including all runable files , jar files and sql files.
			      Link to folder -

	2).documents   folder -
			      
			      This folder contains System Requie Specification document.
			      Link to folder -
	
	
	3).videos      folder -
				
			      This folder contain video of workflow of the project.
			      Link to folder -

	4).readme        file -

			      This file contains the all information about project , readiness to launch the application and guidelines about project.
			      Link to   file -  
 		
	
		
