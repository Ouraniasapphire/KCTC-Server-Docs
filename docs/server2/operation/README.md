# **Operation Info.**

## **Operating Debian**

## **Operating KVM**

    1. Open the apps menu from the top left of the screen
    2. Open the app Labeled KVM ...
    3. Click to run the VM

## **Troubleshooting KVM**

### **If the VM fails to start**:  

- Exit from the KVM app and request assistance

### **If the KVM app shows an error screen**
1. Check if the error message says:
"unable to connect to libvirt qemu:///system"  

2. If so, open the terminal app and run the following command
```bash
sudo systemctl status libvirtd
```

- Interpret the status:
    - Offline, run:
    ```bash
    sudo systemctl enable --now libvirtd
    ```
    - Online, request assistance.


