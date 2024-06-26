# Personal Cloud Storage Setup on Windows

This project demonstrates how to set up a personal cloud storage system using a Windows laptop's SSD. By following this guide, you can share files over your local network and optionally access them remotely.

## Prerequisites

- A laptop running Windows with sufficient SSD storage
- A reliable local network connection
- Basic knowledge of Windows file sharing and network settings

## Setup Instructions

### 1. Enable File Sharing

1. Open **Control Panel** and navigate to **Network and Sharing Center**.
2. Click on **Change advanced sharing settings**.
3. Ensure that **Turn on network discovery** and **Turn on file and printer sharing** are selected.
4. Save changes.

### 2. Create Shared Folders

1. Navigate to the folder you want to share.
2. Right-click on the folder and select **Properties**.
3. Go to the **Sharing** tab and click **Share**.
4. Select the user accounts you want to share with and set permissions (Read/Write).
5. Click **Share** and then **Done**.

### 3. Set Up Remote Access (Optional)

#### Port Forwarding

1. Access your router’s settings (usually accessible via a web browser at 192.168.1.1 or similar).
2. Find the **Port Forwarding** section.
3. Add a new rule to forward port 445 to your laptop’s local IP address.

#### Dynamic DNS

1. Register for a Dynamic DNS (DDNS) service such as No-IP or DynDNS.
2. Follow the DDNS provider’s instructions to set up a hostname that maps to your laptop’s public IP address.

### 4. Security Considerations

1. **Firewall Settings**:
   - Open **Windows Defender Firewall**.
   - Allow SMB traffic by enabling file and printer sharing for your network profile.

2. **User Authentication**:
   - Ensure strong passwords for user accounts that have access to shared folders.

### 5. Backup and Data Protection

Implement a backup strategy to protect your data:
- Use Windows Backup and Restore to create periodic backups of your important files.
- Consider cloud backup solutions for additional redundancy.

## Accessing Your Personal Cloud Storage

### From Other Devices

1. On another Windows device, open **File Explorer**.
2. Click on **Network** in the left sidebar.
3. Find and select your laptop from the network devices list.
4. Enter the username and password if prompted.

### Remote Access

1. If you set up port forwarding and DDNS, you can access your shared folders remotely using the DDNS hostname.
2. For enhanced security, consider setting up a VPN for remote access.

## Troubleshooting

- Ensure that network discovery and file sharing are enabled on all devices.
- Verify that your laptop’s firewall settings allow incoming SMB traffic.
- Check the router’s port forwarding settings if remote access is not working.

## Contributing

Feel free to fork this repository and submit pull requests. Contributions are welcome!

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

