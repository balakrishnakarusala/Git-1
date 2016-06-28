Android-Data-Scraper
=======================
This project grabs all details from android device like user detalis, sms, call logs, contacts and location. This information can be stored in 
application database and at the same time send to server also. When we uninstall this application from device (or) cleared data from 
application database data remain in server for our future usage.

Author & Contributors List
------------------------------
PurnaChandra.Tanikonda

Balakrishna.Karusala

This project is developed under the guidance of Vikash sir.

All rights of this project belongs to "Perfios Software Solutions Pvt. Ltd." 

##Prerequisities
--------------------------------
For Running this project in your local machine, you need to install these softwares

1.Android Studio

	*For running this application in your local machine. You need build gradle file of this application with these dependencies.
	
		*compile 'com.android.support:appcompat-v7:23.4.0'
		
		*compile 'com.android.support:design:23.4.0'
		
		*compile 'com.android.support:support-v4:23.4.0'

2.JRE and JVM with configuration atleast 1.8

3.MySQL Server

4.Apache Tomcat Server 8.0

5.Java Servlets

	*These servlets code written in "Eclipse JeeMars" IDE.
	
	*To "Eclipse JeeMars" IDE you need to add server-api.jar path from tomcat server.
	
	*Create "servlet application" project in "Eclipse JeeMars" IDE.

6.Add these bulid paths to your System Environment Variables.

    * CATALINA_HOME C:\Program Files\Apache Software Foundation\Tomcat 8.0
    
    * CLASS_PATH C:\Program Files\Apache Software Foundation\Tomcat 8.0\lib\servlet-api.jar
    
    * JAVA_HOME C:\Program Files\Java\jdk1.8.0_91.
    
    * path C:\Program Files\Java\jdk1.8.0_91\bin.
    

##Directions
-----------------------------

**How to Run Android Project?**

In "./src/Android" directory you have all your android application code. For running this application code in your system, 
you need to install Android Studio tool. Place this Project folder in android workspace. After Opening Android Studio tool in your system, 
open this application from android workspace. After opening application, sometime will be taken for building gradle of application.
If gradle build successfully then everything is okay, your tool is up to date else you need add above mentioned dependencies in the gradle file 
and rebuild the grable. Gradle build successfully then you can run this application code and can do modifications also.

**How to create MySQL schema?**

In "./src/Sever/MySQL" directory you have all your MySQL code. For using MySQL, you need to install MySQL server in your system.
After installing you can use create database and tables by using given MySQL schema.

**How to use tomcat Server?**

In "./src/Sever/Tomcat" directory you have information about tomcat usage. For using tomcat server you need to add above mentioned build 
paths to your System Environment Variables.

**How to connect MySQL database with http?**

In "./src/Sever/Java" directory you have all your servlet code. By using servlets, you can connect MySQL with http. For Executing servlets you 
need to add some jar files to your "Eclipse JeeMars" IDE.

	1) Add "servlet-api.jar file" to your project in "Eclipse JeeMars" IDE. Follow below mentioned steps to 
	add "server-api.jar" file.
	
		*Right click on your project then go to "Build Path" -> "Configure Build Path" -> "Libraries" -> "External Jars" 
		then add file from this path "C:\Program Files\Apache Software Foundation\Tomcat 8.0\lib\servlet-api.jar".
		
	2) Add "mysql-connector-java-5.1.39.jar" file to your project in "Eclipse JeeMars" IDE. Follow below 
	mentioned steps to add "mysql-connector-java-5.1.39.jar" file.
	
		*Right click on your project then go to "New" -> "New Folder" then create a new folder with a name of 
		"external_lib".
		
		*Copy "mysql-connector-java-5.1.39.jar" file from "C:\Program Files (x86)\MySQL\mysql-connector-java-5.1.39" 
		this location and paste on this folder.
		
		*Open "external_lib" folder and right click on "mysql-connector-java-5.1.39.jar" -> "Build Path" -> 
		"Add Build Path". With this second jar file is added to your Servlet project.
		
	3) Add "java-json.jar" file to your project in "Eclipse JeeMars" IDE. Follow 2nd one steps to add this 
	jar file. This is also one external Library.

**How to send data to http?**

The android code it-self is having the code to send data to http. Referring that directory is sufficient.


