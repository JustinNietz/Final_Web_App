# Project Description

This website is designed for NJIT's course IS-601. We needed to research and develop one unique feature per team member
and integrate it into our application (Pycharm, Docker, Flask, MySQL). Justin Nietzer worked on creating a login and registration process that includes
email verification, and Nikolett Muller worked on using the statistics project to create API endpoints and then consume
those endpoints using a JavaScript chart.

# Installation Instructions for Using the App with Docker

## 1. Installing Docker

**A, Instructions for Windows Users**

There are needed requirements to install Docker Desktop:

* Windows 10, version 1903 or higher
* WSL 2 feature is enabled
* Prerequisites for running WSL 2 on Windows 10
* 64 bit processor
* 4GB system RAM
* BIOS-level hardware virtualization support must be enabled in the BIOS settings
* Linux kernel update package is installed

If all requirements are met, we can download Docker Desktop Installer.exe from Docker Hub. After that, we need to just
double-click on the file to run the installer. It is highly important that we ensure the Enable WSL 2 Features option is
selected on the Configuration page. By following the instructions given by the installation wizard, we can proceed with
the installation. Docker Desktop does not run automatically after we installed it. To start the program, we need to
search for it on our computer.

![finding Docker](screenshots/Docker_in_Search.png)

Docker is running when the whale icon appears on the taskbar; we can access it from any terminal now.

![whale icon](screenshots/whale_Microsoft.png)

**B, Instructions for Mac users**

Needed requirements to install Docker Desktop:

* macOS must be version 10.14 or newer (Mojave, Catalina, or Big Sur)
* At least 4 GB of RAM.
* VirtualBox prior to version 4.3.30 must not be installed as it is not compatible with Docker Desktop

Installing Docker on macOS is just as easy as on Windows. We need to double-click on Docker.dmg, then drag the Docker
icon to our Applications folder.

![dragging Docker app](screenshots/Docker_app.png)

After dragging it, we just need to double-click on Docker.app in the Applications folder to start the program the first
time.

![starting Docker](screenshots/Docker_run.png)

When we notice the whale icon in the top status bar, it shows that Docker Desktop is up and running.

![running Docker](screenshots/whale_IOS.png)

## 2. How to Run the Final Web Application

After Docker started running, we need to add a Configuration in Pycharm. We choose Docker, then Docker-compose. After
choosing, we give the path to docker-compose.yml; we check both checkboxes under Options, then we click on Apply and OK.

![adding configuration](screenshots/add_configuration.png)

After the configuration, we can run the project. If the project is running successfully, we can connect our MSQL
database to our project. We go to View, then Tool Windows; finally, we choose Database. Here, we click on the + sign, on
Data Source, then on MYSQL. We give our database a name: "homesData". The port needs to be set to 32000. We give "root"
as user, and "root" as password. Finally, we can click on Test Connection, then Apply and OK.

![connecting database](screenshots/database.png)

After these steps, we need to add an interpreter. We choose Docker Compose, give the path to docker-compose.yml and
select app as a service. Finally, we click on OK. Now, we are able to choose the newly added interpreter.

![adding interpreter](screenshots/add_interpreter.png)

We run the app again, then in order to see the website, we type "http://localhost:5000" into the address bar of our
internet browser.

# Postman Screenshot

![postman request output](screenshots/postman.PNG)

# SQL Data Screenshot

![pycharm data query](screenshots/query.PNG)

# Bootstrap HTML template

![bootstrap data](screenshots/bootstrap.PNG)

