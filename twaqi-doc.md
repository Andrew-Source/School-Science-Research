# WARNING:
This is a clone version of [this document](https://ascxz.ml/munucial/custom/twaqi/shutting-down-twaqi/) which is also written by *Andrew*, but since we've remove and edit some part, the document might have some exploit in it, if you encounter any error, read the original document first then contact *Andrew*.

Thanks!

---

# Menu

*   PC installation
    *   Windows
        *   [portable version](#windows-portable-version)
        *   [installation version](#windows-installation-version)
    *   [Other OS](#other-os)
*   Hosting installation
    *   [Have SSH access (Linux hosting)](#linux-hosting-have-ssh-access)
    *   [No SSH access (for all kind of Windows and Linux or other OS hosting)](#no-ssh-access)
*   File list
    *   Windows
        *   32-bit
            *   [portable](https://files.munucial.com/release/custom/tw-aqi-monitor/tw-aqi-data-monitor-win32-portable.zip)
            *   [installation](https://files.munucial.com/release/custom/tw-aqi-monitor/tw-aqi-data-monitor-win32.zip)
        *   64-bit
            *   [portable](https://files.munucial.com/release/custom/tw-aqi-monitor/tw-aqi-data-monitor-win64-portable.zip)
            *   [installation](https://files.munucial.com/release/custom/tw-aqi-monitor/tw-aqi-data-monitor-win64.zip)
    *   [Other OS](https://files.munucial.com/release/custom/tw-aqi-monitor/tw-aqi-data-monitor.zip)

* * *

# Portable Version (Windows)

1.  To install you'll need to download the package zip ([32-bit](https://files.munucial.com/release/custom/tw-aqi-monitor/tw-aqi-data-monitor-win32-portable.zip), [64-bit](https://files.munucial.com/release/custom/tw-aqi-monitor/tw-aqi-data-monitor-win64-portable.zip)) then extract it
2.  open the command prompt (by pressing **win+r** and type **cmd** then click **Enter**)
3.  Navigate to the folder you extracted (for navigating, type **cd** + path you wanna go)
4.  To start the application you'll need to run the commands below one by one in order
    1.  `npm i forever -g`
    2.  `npm install`
    3.  `set PORT=80`
        *   **WARNING: only run this command when you don't have Apache/XAMPP or other node.js application running on port 80 (Apache/XMAPP is using port 80 in default)**
    4.  `forever start monitor.min.js`
5.  To stop the application you'll need to run the commands below
    1.  `forever stop monitor.min.js`
    2.  To check if it really stops, go through these steps below
        1.  `forever list`
        2.  see if there is listing any things that say **No forever processes running**
            *   If not run `forever stopall` then repeat the process from step 2-1
            *   If yes, then the process should be stopped
            *   **WARNING: this way is only for the computer that has not been running any other node.js application with forever, if it does, you should know how to stop and check them properly, if you still don't know contact me at [mail@munuical.com](mailto:mail@munuical.com)**
6.  To view the application, visit **127.0.0.1** or  **localhost**
    *   If you skip the **set PORT=80** part, visit **127.0.0.1:5118** or **localhost:5118**

* * *

# Installation Version (Windows)

1.  Same download the zip and extract them first ([32-bit](https://files.munucial.com/release/custom/tw-aqi-monitor/tw-aqi-data-monitor-win32.zip), [64-bit](https://files.munucial.com/release/custom/tw-aqi-monitor/tw-aqi-data-monitor-win64.zip))
2.  Then go to the **installer** folder
3.  Run the **node-v8.9.1-x86.msi** file
4.  **OPTIONAL: Go back to the main folder and delete the installer folder**
5.  Open **CMD** (by pressing `WIN+R` and type `cmd`)
6.  Navigate to the folder you extracted (for navigating, type **cd** + path you wanna go)
7.  To start the application you'll need to run the commands below one by one in order
    1.  `npm i forever -g`
    2.  `npm install`
    3.  `set PORT=80`
        *   **WARNING: only run this command when you don't have Apache/XAMPP or other node.js application running on port 80 (Apache/XMAPP is using port 80 in default)**
    4.  `forever start monitor.min.js`
8.  To stop the application you'll need to run the commands below
    1.  `forever stop monitor.min.js`
    2.  To check if it really stops, go through these steps below
        1.  **forever list**
        2.  see if there is listing any things that say **No forever processes running**
            *   If not run `forever stopall` then repeat the process from step 2-1
            *   If yes, then the process should be stopped
            *   **WARNING: this way is only for the computer that has not been running any other node.js application with forever, if it does, you should know how to stop and check them properly, if you still don't know contact me at [_mail@munuical.com_](mailto:mail@munuical.com)**
9.  To view the application, visit `127.0.0.1` or  `localhost`
    *   If you skip the `set PORT=80` part, visit `127.0.0.1:5118` or `localhost:5118`

* * *

# Other OS

1.  Download and extract the All OS version ([here](https://files.munucial.com/release/custom/tw-aqi-monitor/tw-aqi-data-monitor.zip)) (We call the folder you extracted _**main code folder**_)
2.  Open your browser and goto [**Node.js download page**](https://nodejs.org/en/download/)
3.  Download the correct file that matches your OS
    1.  If you download **instal****ler** **version**, run the installer
    2.  If you download **Source code** or **Binary version**, extract it and take all the content from the extracted folder and put it into the _**main code folder**_ or** parent folder of** _**main code folder**_
4.  Open the terminal in your OS
5.  To start the application you'll need to run the commands below one by one in order
    1.  `npm i forever -g`
    2.  `npm install`
    3.  `set PORT=80`
        *   **WARNING: only run this command when you don't have Apache/XAMPP or other node.js application running on port 80 (Apache/XMAPP is using port 80 in default)**
    4.  `forever start monitor.min.js`
6.  To stop the application you'll need to run the commands below
    1.  `forever stop monitor.min.js`
    2.  To check if it really stops, go through these steps below
        1.  `forever list`
        2.  see if there is listing any things that say **No forever processes running**
            *   If not run `forever stopall` then repeat the process from step 2-1
            *   If yes, then the process should be stopped
            *   **WARNING: this way is only for the computer that has not been running any other node.js application with forever, if it does, you should know how to stop and check them properly, if you still don't know contact me at [_mail@munuical.com_](mailto:mail@munuical.com)**
7.  To view the application, visit `127.0.0.1` or  `localhost`
    *   If you skip the `set PORT=80` part, visit `127.0.0.1:5118`* or `localhost:5118`

* * *

# Have SSH access (Linux hosting)

1.  Download the All OS version ([here](https://files.munucial.com/release/custom/tw-aqi-monitor/tw-aqi-data-monitor.zip)) and extract it (we call the extracted folder **_main code folder_**)
2.  Connect to the SSH (**THIS SOMETIMES REQUIRE ADVANCE SKILL, IF YOU HAVE ANY ISSUE, CONTACT ME AT [MAIL@MUNUCIAL.COM](mailto:MAIL@MUNUCIAL.COM)**
    1.  **RECOMMENDED METHOD**
        1.  Download PuTTy ([here](https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html)) for the correct version that matches your OS
        2.  Ask your hosting provider for SSH login detail
            1.  **SAMPLE MAIL: **Hi, I would like to ask for the SSH login detail, can you tell me the login credential and the port to login?
        3.  Type the login credential into the correct field, if your hosting provider has changed the login port, remember to change the port field
        4.  Click **open** button
3.  Call your hosting provider to start the node.js application location at **main code folder/monitor.min.js**

* * *

# No SSH access

1.  Download the All OS version ([here](https://files.munucial.com/release/custom/tw-aqi-monitor/tw-aqi-data-monitor.zip)) and extract it (we call the extracted folder **_main code folder_**)
2.  Call your hosting provider to start the node.js application location at **main code folder/monitor.min.js**

---
