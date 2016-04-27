# mobile-android-simple

Android Sample Application

# Developer Workspace

[![Contribute](http://beta.codenvy.com/factory/resources/codenvy-contribute.svg)](http://beta.codenvy.com/f?id=aaccd6ani3r1x310)

# Recipe

FROM [codenvy/ubuntu_android](https://hub.docker.com/r/codenvy/ubuntu_android/)

# How to run

1. Project build is started automatically when a workspace starts. Click the Preview URL, right click on the gray screen to call a context menu and launch the Emulator. It may take a while. 
![Alt text](https://raw.githubusercontent.com/ddementieva/android-images/master/images/context-menu.png "Context menu")
2. Once the Emulator is started, right click on the gray screen and start the Terminal. In the Terminal run the following command to install apk: `adb install /projects/mobile-android-simple/target/maven-android-0.1.0.apk`.
![Alt text](https://raw.githubusercontent.com/ddementieva/android-images/master/images/adb-install-simple.png "adb install simple")
3. Find your application in the Emulator's Menu.
![Alt text](https://raw.githubusercontent.com/ddementieva/android-images/master/images/codenvy-example.png "Codenvy Example")
4. Go back to the IDE. Change your application, build it with `build-n-run` command, go to the previously opened VNC window and run `adb install -r /projects/mobile-android-simple/target/maven-android-0.1.0.apk` command to see the changes.       
![Alt text](https://raw.githubusercontent.com/ddementieva/android-images/master/images/update.png "Update")

| #       | Description           | Command  |
| :------------- |:-------------| :-----|
| 1      | Build and run | `cd ${current.project.path} && mvn clean install` |

