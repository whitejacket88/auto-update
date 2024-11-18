# Auto-update Application for Linux Systems

This application is designed to automatically update Linux systems that do not perform system updates automatically. It runs in the background and notifies you when updates are available, simplifying the update process.

> **Note:** Running the script with `sudo` may install shortcuts in the root user’s home directory. Run the script normally to avoid this issue. You will be prompted for your password when the application is moved to `/opt`. While dependencies are generally not required, you can run the `dependencies.sh` script to handle any that may be needed (no GUI is available for this step).

---

## Features

- **Automated Updates:** Runs `sudo apt update` in the background and notifies you of available updates.
- **User-Friendly Notifications:** Alerts you when upgrades are available to simplify system maintenance.
- **Flexible Installation Options:** Choose between script-based or GUI installation methods.

---

## Installation Methods

### 1. Script Install (For Advanced Users)

1. Open a terminal and navigate to your Downloads folder:

   cd ~/Downloads

2. Download the master file using `git`:
   
   git clone <repository-url>

      - If `git` is not installed, install it with:

           sudo apt install git

3. Extract the tar file:

   sudo tar xzf auto-update-master.tar.gz


4. Navigate into the extracted directory:

   cd auto-update-master


5. Make the `install.sh` script executable:
   
   sudo chmod +x install.sh


7. Run the installation script:
   
   ./install.sh

> **Important:** Running the script with `sudo` may install shortcuts in the root user’s home directory. Run the script normally to avoid this issue. You will be prompted for your password when the application is moved to `/opt`.

---

### 2. GUI Install (For Easy Setup)

1. In the Downloads folder, right-click the `auto-update-master.tar.gz` file and unzip it.
2. Open the newly created `auto-update-master` folder and then the `gui-install` folder.
3. Right-click the `install.desktop` file and select **Allow launching**.
4. Double-click the `install.desktop` file and follow the prompts to complete the installation.

---

## Uninstallation

### Script Method

1. Navigate to the `/opt/auto-update` directory:
   
cd ~/Auto-update/scripts/scripts

3. Make the uninstall script executable:
   
sudo chmod +x uninstall.sh

5. Run the script:
   
./uninstall.sh

---

### GUI Method

1. Go to the Auto-Update home location folder in your home directory.
2. Open the `scripts` folder and locate the `uninstall.desktop` file.
3. Right-click the `uninstall.desktop` file, select **Allow launching**, and click the file to follow the prompts.

---

## Summary

- **Easy Install:** Use the script for technical installs or the GUI method for a simpler approach.
- **Uninstall:** Easily uninstall through the script or GUI.
- **Automatic Updates:** Enjoy seamless updates with background notifications.

---

## Credits

**Developer:** Tom White  
**Company:** WhiteHat Security and Pen-Testing  
**Contact:** twhite1288@whitehat.icu  

**Special Thanks:**  
To the open-source community for their contributions to Linux system tools and utilities that make this application possible.

**Icons & Graphics:**  
Icons used in the application are from Icon Archive and are licensed for free use.

**Dependencies:**  
- `gnome-desktop` or `xdg-utils` (for `.desktop` file handling and application launcher)  
- `python3` or relevant Python libraries (if your app is Python-based)  
- `libnotify` (for desktop notifications)  
- `curl` or `wget` (for downloading updates, if applicable)  
- `git` (if you use Git for version control or cloning repositories)
