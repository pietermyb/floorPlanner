# Floor Planner
Ionic, Cordova and Electon based Floor Planner with Meta data recorder.

# Getting Started (Windows Guide)

* Install NodeJS!
* Open a terminal and install ionic and cordova: 
 ```bash
 npm i ionic cordova -g
 ```
 * 

# Serving the app in a browser

Run `ionic serve` in the console from the root directory
```bash
ionic serve
```

# Serving the app on Android

* You will need Java's JDK:\
https://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html

* Second you need to have the Android SDK installed:
Download if from here https://developer.android.com/studio/#command-tools

Extract the zip to C:\android\
Next, inside tools\bin directory run the following

```bash
sdkmanager.bat "platform-tools"
```
Accept the licence agreement.

Now setup a android sdk

```bash
sdkmanager.bat --list
sdkmanager "platforms;android-8"
```

Now download and isntall Gradel via Chocolatey:
https://chocolatey.org/docs/installation#installing-chocolatey
```bash
choco install gradle -y
```

## Environment Variables ##
Now that everything’s installed, we’ll need to set some environment variables for our command line. From the startmenu, search for “System Environment Variables”. From here, we’ll update the user variable PATH and create a new variable of ANDROID_HOME

ANDROID_HOME : The path to where the Android SDK is installed.
PATH : Two entries, one where Tools are installed for the Android SDK, and another for Platform tools

## Project Setup ##

Add the android platform:
```bash
ionic cordova platform add android
```

Build with `ionic cordova build android`
```bash
ionic cordova build android
```

Run `ionic cordova run android -l` to run the app live on a Developer enabled Android device with USB debugging enabled.
```bash
ionic cordova run android -l --device --verbose
```



