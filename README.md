# Virtual Android System Simulation

This script simulates a virtual Android environment capable of running basic tasks such as launching a virtual Android system, installing an APK, and retrieving system information.

## Requirements

- Python 3.7 or higher
- QEMU 
- ADB (Android Debug Bridge) 
- An Android system image 
- A sample APK file 

## How to Run the Script

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/harsh16629/Virtual-android-system-simulation-using-python.git
   cd <repository-folder>
   ```

2. **Install Dependencies**:
   Ensure QEMU and ADB are installed and accessible from the system PATH.

3. **Run the Script**:
   ```bash
   python virtual_android_system.py
   ```

4. Follow the prompts displayed on the terminal.

## How to Install an App on the Virtual System

- Place the APK file you want to install in the same directory as the script.
- Update the `apk_path` variable in the script to the correct APK file name.
- The script will automatically install the app using ADB once the virtual system is launched.

## System Information Logged

The script retrieves and logs the following system details:

- **OS Version**: The Android operating system version running on the virtual device.
- **Device Model**: The model name of the virtual Android device.
- **Available Memory**: The amount of free memory available on the system.

### Log File

System information is saved in a file named `system_info.log` in the script's directory. Check this file for details about the virtual Android environment.

## Notes

- Ensure the Android system image (`android.img`) is present in the directory and is compatible with QEMU.
- Adjust the AVD name (`test_avd`) in the QEMU command if using a custom AVD.
- Modify the memory allocation or other QEMU settings as needed for performance.

