# Project: Personal Cloud Storage Setup on Windows

## Overview

This project aims to set up a personal cloud storage system using a Windows laptop's SSD. The setup will enable file sharing over a local network and allow optional remote access.


## Objectives

- Set up a personal cloud storage solution using a Windows laptop.
- Enable file sharing over a local network.
- Optionally configure remote access to shared files.
- Implement security measures to protect shared data.
- Establish a backup strategy for data protection.

## Prerequisites

- A laptop running Windows with sufficient SSD storage.
- A reliable local network connection.
- Basic knowledge of Windows file sharing and network settings.

## Setup Instructions

### Enable File Sharing

1. Open **Control Panel** and navigate to **Network and Sharing Center**.
2. Click on **Change advanced sharing settings**.
3. Ensure that **Turn on network discovery** and **Turn on file and printer sharing** are selected.
4. Save changes.

### Create Shared Folders

1. Navigate to the folder you want to share.
2. Right-click on the folder and select **Properties**.
3. Go to the **Sharing** tab and click **Share**.
4. Select the user accounts you want to share with and set permissions (Read/Write).
5. Click **Share** and then **Done**.

![Screenshot](https://github.com/Riyanshj/Personal-Cloud-Storage-on-Windows-SSD/blob/main/Images-Videos/Test-Folder.png)




### Set Up Remote Access (Optional)

#### Port Forwarding

1. Access your router’s settings (usually accessible via a web browser at 192.168.1.1 or similar).
2. Find the **Port Forwarding** section.
3. Add a new rule to forward port 445 to your laptop’s local IP address.

#### Dynamic DNS

1. Register for a Dynamic DNS (DDNS) service such as No-IP or DynDNS.
2. Follow the DDNS provider’s instructions to set up a hostname that maps to your laptop’s public IP address.

### Security Considerations

#### Firewall Settings

1. Open **Windows Defender Firewall**.
2. Allow SMB traffic by enabling file and printer sharing for your network profile.
3. Disable public sharing.
4. Disable Password Protected Sharing(for mobile use).


## Accessing Your Personal Cloud Storage

### Using Solid Explorer File Manager

1. Open **Solid Explorer** on your Android device.
2. Tap the **+** button and select **New cloud connection**.
3. Choose **SMB/CIFS** from the list of protocols.
4. Enter your laptop's local IP address or DDNS hostname, along with the shared folder name.
5. Enter your Windows username and password.
6. Tap **Connect** to access your shared folders.

![Screenshot](https://github.com/Riyanshj/Personal-Cloud-Storage-on-Windows-SSD/blob/main/Images-Videos/mobile-file-manager.mp4)


## Troubleshooting

- Ensure that network discovery and file sharing are enabled on all devices.
- Verify that your laptop’s firewall settings allow incoming SMB traffic.
- Check the router’s port forwarding settings if remote access is not working.

## Contributing

Feel free to fork this repository and submit pull requests. Contributions are welcome!

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
