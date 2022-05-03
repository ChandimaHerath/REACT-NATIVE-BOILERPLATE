# REACT NATIVE BOILERPLATE

This product is to be used as a starter template code for creating mobile applications for both android and ios devices since the technology used to build the project is React Native. Developers can easily start developing processes upon the supplied code base with selected dependencies in the project and the folder structures created. Using this product the developers can start their project in a short period of time and easily.

## 1. Boilerplate Setup

To work with this boilerplate, you have to download it. So follow these instructions to setup the boilerplate for customization.

### 1.1 Cloning the Repository

   **http Method**
   
    git clone https://dilankanirmal@bitbucket.org/paladinanalytics/react-native.git
    
   **SSH Method**
   
    git clone git@bitbucket.org:paladinanalytics/react-native.git
    
### 1.2 Install Packages

   **NPM Install**
   
    npm install
    
### 1.3 Run Project

   **Android**
   
    npx react-native run-android
   
   **IOS**
   
    npx react-native run-ios

## 2. Boilerplate Features

This product provides required and relevant Folder Structure, Creating Re-usable Components, Storage and Redux, Testing, Navigation, React-Native code templates and so on to the developers.

### 2.1 Folder Structure

The folders are arranged in a  moduler approach including the essential files inside each module, which increase the maintainability.

### 2.2 Re-usable Components

There are two re-usable components that can be used in entire project, "Custom Button Components" and "Custom Input Component".
     **Location : react-native/src/components/form**
     
If you have any other re-usable components you can add them by following the structure that we have used there. 

### 2.3 State Management

State management done using the Redux library. Example redux components (actions, reducers, store, root reducer, types) are already included for the reference of the developers in each module. 

### 2.4 Storage

A react native async storage is already build for persisting data.
  **Location : src/utils/storage.ts**

### 2.5 Testing 

For the testing purposes, we have created some testings such as, "Sign Up Testing", "Sign In Testing", "Forgot Pasword Testing", "Render Component Testing", and so on.
    
   **Location : react-native/__tests__**
   
If you have any other testings you can add them by following the structure that we have used there.

### 2.6 Navigation  

/**************************************************************/

### 2.7 Module Creating 

For easy understanding and maintainance, we have devided the project in to modules. As a start we have created two modules as "Auth Module" and "App Module".

   **Location : react-native/src/modules**

If you have any other modules you can add them by following the structure that we have used there.

### 2.8 http Class

An httpClass is build herewhich contains the http methods which can be used as reusable functions. Interceptors are also incuded here.

   **Location : src/utils/httpClass.ts**
