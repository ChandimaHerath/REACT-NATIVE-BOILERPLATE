# REACT NATIVE BOILERPLATE

This product is to be used as a starter template code for creating mobile applications for both android and ios devices since the technology used to build the project is React Native. Developers can easily start developing processes upon the supplied code base with selected dependencies in the project and the folder structures created. Using this product the developers can start their project in a short period of time and easily.

## Environment Setup

 This boilerplate is done by using React Native CLI. You will need Node, the React Native command line interface, a JDK, and Android Studio or Xcode to get started.
 you can refer React Native official documentation for more information. https://reactnative.dev/docs/environment-setup

### Installing Node, JDK

/*********************************************/

### Android development environment

#### 1. Installing Android Studio

Download and install Android Studio. While on Android Studio installation wizard, make sure the boxes next to all of the following items are checked:
 * Android SDK
 * Android SDK Platform
 * Android Virtual Device
 * If you are not already using Hyper-V: Performance (Intel ® HAXM) (See here for AMD or Hyper-V)

#### 2. Install The Android SDK

Android Studio installs the latest Android SDK by default. Building a React Native app with native code, however, requires the Android 11 (R) SDK in particular. Additional Android SDKs can be installed through the SDK Manager in Android Studio.

To do that, open Android Studio, click on "Configure" button and select "SDK Manager".

Select the "SDK Platforms" tab from within the SDK Manager, then check the box next to "Show Package Details" in the bottom right corner. Look for and expand the Android 11 (R) entry, then make sure the following items are checked:

 * Android SDK Platform 30
 * Intel x86 Atom_64 System Image or Google APIs Intel x86 Atom System Image

Next, select the "SDK Tools" tab and check the box next to "Show Package Details" here as well. Look for and expand the "Android SDK Build-Tools" entry, then make sure that 30.0.2 is selected.

Finally, click "Apply" to download and install the Android SDK and related build tools.

#### 3. 3. Configure The ANDROID_HOME Environment Variable

he React Native tools require some environment variables to be set up in order to build apps with native code.

1. Open the Windows Control Panel.
2. Click on User Accounts, then click User Accounts again
3. Click on Change my environment variables
4. Click on New... to create a new ANDROID_HOME user variable that points to the path to your Android SDK:
