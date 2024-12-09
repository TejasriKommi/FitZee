# **Flutter Installation and Setup Guide**

This guide will walk you through the steps to **install Flutter**, **set up Android Studio**, **download API 33 Android emulator**, **configure the Flutter toolchain**, and **run a Flutter application**. Additionally, it includes instructions to **build an Android APK**.

---

## **Prerequisites**

Before starting, ensure you have the following:
- A computer running **macOS**, **Windows**, or **Linux**.
- Administrator access to install software.
- At least **2GB of free disk space**.

---

## **Step 1: Install Flutter SDK**

1. **Download Flutter SDK**  
   - Visit the [Flutter Download Page](https://flutter.dev/docs/get-started/install).  
   - Choose the appropriate version for your operating system.

2. **Extract Flutter**  
   - Extract the downloaded zip file to a location of your choice (e.g., `C:\src\flutter` for Windows).

3. **Add Flutter to PATH**  
   - Update your system's environment variables:
     - **On Windows**: Add `flutter/bin` to the PATH variable.
     - **On macOS/Linux**: Add the following line to your `.bashrc` or `.zshrc` file:
       ```bash
       export PATH="$PATH:[PATH_TO_FLUTTER_DIRECTORY]/flutter/bin"
       ```

4. **Verify Installation**  
   - Run the following command in a terminal:
     ```bash
     flutter doctor
     ```
   - This will display a summary of your Flutter installation and indicate any missing dependencies.

---

## **Step 2: Install Android Studio**

1. **Download and Install**  
   - Download Android Studio from the [official website](https://developer.android.com/studio).  
   - Follow the installation instructions for your operating system.

2. **Set Up Android SDK**  
   - Install the Flutter plugin in Android Studio.  
   - Open Android Studio and go to **File > Settings > Appearance & Behavior > System Settings > Android SDK**.  
   - Ensure that the following components are installed:
     - **Android SDK Platform-Tools**  
     - **Android SDK Build-Tools**  
     - **API 33 (Android 13)**  

3. **Create an Android Emulator**  
   - Go to **Tools > Device Manager** and create a new virtual device.  
   - Select a hardware profile (e.g., Pixel 8).  
   - Choose **API 33** as the system image.  
   - Finish the setup and launch the emulator.

---

## **Step 3: Set Up Flutter Toolchain**

1. Run the following command to accept the Android licenses:
   ```bash
   flutter doctor --android-licenses

