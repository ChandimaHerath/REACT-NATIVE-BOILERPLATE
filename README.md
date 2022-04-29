# REACT NATIVE BOILERPLATE

This product is to be used as a starter template code for creating mobile applications for both android and ios devices since the technology used to build the project is React Native. Developers can easily start developing processes upon the supplied code base with selected dependencies in the project and the folder structures created. Using this product the developers can start their project in a short period of time and easily.

## 1. Environment Setup for React-Native

 This boilerplate is done by using React Native CLI. You will need Node, the React Native command line interface, a JDK, and Android Studio or Xcode to get started.
 
 You can refer [React Native Official Documentation](https://reactnative.dev/docs/environment-setup) for more information: 

### 1.1.1 Installing Node, JDK (Only for Android Development in macOS and Windows)

#### For Windows

We recommend installing Node via [Chocolatey](https://chocolatey.org/), a popular package manager for Windows.

It is recommended to use an LTS version of Node. If you want to be able to switch between different versions, you might want to install Node via [nvm-windows](https://github.com/coreybutler/nvm-windows), a Node version manager for Windows.

React Native also requires [Java SE Development Kit (JDK)](https://openjdk.java.net/projects/jdk/11/), which can be installed using Chocolatey as well.

Open an Administrator Command Prompt (right click Command Prompt and select "Run as Administrator"), then run the following command:

    choco install -y nodejs-lts openjdk11
    
#### For macOS with Android

##### Installing dependencies

You will need Node, Watchman, the React Native command line interface, a JDK, and Android Studio.

While you can use any editor of your choice to develop your app, you will need to install Android Studio in order to set up the necessary tooling to build your React Native app for Android.

###### Node & Watchman

We recommend installing Node and Watchman using [Homebrew](http://brew.sh/). Run the following commands in a Terminal after installing Homebrew:

 brew install node
 brew install watchman
 
###### Java Development Kit

We recommend installing the OpenJDK distribution called Azul Zulu using [Homebrew](http://brew.sh/). Run the following commands in a Terminal after installing Homebrew:

 brew tap homebrew/cask-versions
 brew install --cask zulu11

The Zulu OpenJDK distribution offers JDKs for **both Intel and M1 Macs.** This will make sure your build are faster on M1 Macs compared to using an Intel-based JDK.

If you have already installed JDK on your system, make sure it is JDK 11 or newer.

### 1.1.2 For macOS with iOS (Only for iOS Development in macOS)

#### Installing dependencies

You will need Node, Watchman, the React Native command line interface, Xcode and CocoaPods.

While you can use any editor of your choice to develop your app, you will need to install Xcode in order to set up the necessary tooling to build your React Native app for iOS.

##### Node & Watchman

We recommend installing Node and Watchman using [Homebrew](http://brew.sh/). Run the following commands in a Terminal after installing Homebrew:

 brew install node
 brew install watchman

If you have already installed Node on your system, make sure it is Node 14 or newer.

[Watchman](https://facebook.github.io/watchman) is a tool by Facebook for watching changes in the filesystem. It is highly recommended you install it for better performance.

### 1.2 Android development environment (Only for Android Development in macOS and Windows)

#### 1.2.1. Installing Android Studio

[Download and install Android Studio](https://developer.android.com/studio/index.html). While on Android Studio installation wizard, make sure the boxes next to all of the following items are checked:
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

#### 1.2.3.1. Configure The ANDROID_HOME Environment Variable (Only for windows)

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

#### 1.2.3.1. Configure the ANDROID_SDK_ROOT environment variable (only for macOS)

The React Native tools require some environment variables to be set up in order to build apps with native code.

Add the following lines to your $HOME/.bash_profile or $HOME/.bashrc (if you are using zsh then ~/.zprofile or ~/.zshrc) config file:

 export ANDROID_SDK_ROOT=$HOME/Library/Android/sdk
 export PATH=$PATH:$ANDROID_SDK_ROOT/emulator
 export PATH=$PATH:$ANDROID_SDK_ROOT/platform-tools
 
Type source $HOME/.bash_profile for bash or source $HOME/.zprofile to load the config into your current shell. Verify that ANDROID_SDK_ROOT has been set by running echo $ANDROID_SDK_ROOT and the appropriate directories have been added to your path by running echo $PATH.

#### 1.2.4. Add platform-tools to Path (Only for Windos)

 1. Open the Windows Control Panel.
 2. Click on User Accounts, then click User Accounts again
 3. Click on Change my environment variables
 4. Select the Path variable.
 5. Click Edit.
 6. Click New and add the path to platform-tools to the list.

**The default location for this folder is:**

    %LOCALAPPDATA%\Android\Sdk\platform-tools

### 1.3. iOS Development (Only for iOS development in macOS)

#### 1.3.1 Xcode

The easiest way to install Xcode is via the [Mac App Store](https://itunes.apple.com/us/app/xcode/id497799835?mt=12). Installing Xcode will also install the iOS Simulator and all the necessary tools to build your iOS app.

If you have already installed Xcode on your system, make sure it is version 10 or newer.

#### 1.3.2. Command Line Tools
You will also need to install the Xcode Command Line Tools. Open Xcode, then choose "Preferences..." from the Xcode menu. Go to the Locations panel and install the tools by selecting the most recent version in the Command Line Tools dropdown.

#### 1.3.3. Installing an iOS Simulator in Xcode

To install a simulator, open Xcode > Preferences... and select the Components tab. Select a simulator with the corresponding version of iOS you wish to use.

#### 1.3.4. CocoaPods

[CocoaPods](https://cocoapods.org/) is built with Ruby and it will be installable with the default Ruby available on macOS. You can use a Ruby Version manager, however we recommend that you use the standard Ruby available on macOS unless you know what you're doing.

Using the default Ruby install will require you to use sudo when installing gems. (This is only an issue for the duration of the gem installation, though.)

 sudo gem install cocoapods

For more information, please visit [CocoaPods Getting Started guide](https://guides.cocoapods.org/using/getting-started.html).

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
    
### 2.3 Run Project

   **Android**
   
    npx react-native run-android
   
   **IOS**
   
    npx react-native run-ios

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

For the testing purposes, we have created some testings such as, "Sign Up Testing", "Sign In Testing", "Forgot Pasword Testing", "Render Component Testing", and so on.
    
   **Location : react-native/__tests__**
   
If you have any other testings you can add them by following the structure that we have used there.

### 3.5 Navigation  

/**************************************************************/
