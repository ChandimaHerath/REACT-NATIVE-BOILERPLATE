# REACT NATIVE BOILERPLATE

This product is to be used as a starter template code for creating mobile applications for both android and ios devices since the technology used to build the project is React Native. Developers can easily start developing processes upon the supplied code base with selected dependencies in the project and the folder structures created. Using this product the developers can start their project in a short period of time and easily.

## 1. Environment Setup for React-Native

 This boilerplate is done by using React Native CLI. You will need Node, the React Native command line interface, a JDK, and Android Studio or Xcode to get started.
 You can refer React Native official documentation for more information: https://reactnative.dev/docs/environment-setup

### 1.1 Installing Node, JDK

/*********************************************/

### 1.2 Android development environment

#### 1.2.1. Installing Android Studio

Download and install Android Studio. While on Android Studio installation wizard, make sure the boxes next to all of the following items are checked:
 * Android SDK
 * Android SDK Platform
 * Android Virtual Device
 * If you are not already using Hyper-V: Performance (Intel ® HAXM) (See here for AMD or Hyper-V)

#### 1.2.2. Install The Android SDK

Android Studio installs the latest Android SDK by default. Building a React Native app with native code, however, requires the Android 11 (R) SDK in particular. Additional Android SDKs can be installed through the SDK Manager in Android Studio.

To do that, open Android Studio, click on "Configure" button and select "SDK Manager".

Select the "SDK Platforms" tab from within the SDK Manager, then check the box next to "Show Package Details" in the bottom right corner. Look for and expand the Android 11 (R) entry, then make sure the following items are checked:

 * Android SDK Platform 30
 * Intel x86 Atom_64 System Image or Google APIs Intel x86 Atom System Image

Next, select the "SDK Tools" tab and check the box next to "Show Package Details" here as well. Look for and expand the "Android SDK Build-Tools" entry, then make sure that 30.0.2 is selected.

Finally, click "Apply" to download and install the Android SDK and related build tools.

#### 1.2.3. Configure The ANDROID_HOME Environment Variable

The React Native tools require some environment variables to be set up in order to build apps with native code.

 1. Open the Windows Control Panel.
 2. Click on User Accounts, then click User Accounts again
 3. Click on Change my environment variables
 4. Click on New... to create a new ANDROID_HOME user variable that points to the path to your Android SDK:

**The SDK is installed, by default, at the following location:**

    %LOCALAPPDATA%\Android\Sdk

You can find the actual location of the SDK in the Android Studio "Settings" dialog, under Appearance & Behavior → System Settings → Android SDK.

**Open a new Command Prompt window to ensure the new environment variable is loaded before proceeding to the next step.**

 1. Open powershell
 2. Copy and paste Get-ChildItem -Path Env:\ into powershell
 3. Verify ANDROID_HOME has been added

### 1.2.4. Add platform-tools to Path

 1. Open the Windows Control Panel.
 2. Click on User Accounts, then click User Accounts again
 3. Click on Change my environment variables
 4. Select the Path variable.
 5. Click Edit.
 6. Click New and add the path to platform-tools to the list.

**The default location for this folder is:**

    %LOCALAPPDATA%\Android\Sdk\platform-tools

## 2. Boilerplate Setup

To work with this boilerplate, you have to download it. So follow these instructions to setup the boilerplate for customization.

### 2.1 Cloning the Repository

   **http Method**
    git clone https://dilankanirmal@bitbucket.org/paladinanalytics/react-native.git
    
   **SSH Method**
    git clone git@bitbucket.org:paladinanalytics/react-native.git
    
### 2.2 Install Packages

   **NPM Install**
    npm install

## 3. Boilerplate Features

This product provides required and relevant Folder Structure, Creating Re-usable Components, Store and Redux, Testing, Navigation, React-Native code templates and so on to the developers.

### 3.1 Folder Structure

/**********************************************************/

### 3.2 Re-usable Components

There are two re-usable components that can be used in entire project, "Custom Button Components" and "Custom Input Component".
     **Location : react-native/src/components/form**
     
If you have any other re-usable components you can add them by following the structure that we have used there. 

### 3.3 Store and Redux

/**************************************************************/

### 3.4 Testing 

/**************************************************************/

### 3.5 Navigation 

/**************************************************************/
