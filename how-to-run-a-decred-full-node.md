# How to run a Decred full node?

**Why?**
Reasons are the same as in most other digital currencies: support the decentralized network.

**How?**
You can use all kinds of devices to run a Decred full node. Simply follow the steps below to set it up and find a place to leave it running. The node won't need a lot of maintenance.

### Requirements:
- Reliable internet connection
- Access to the settings of the router
- Any device to run the Decred software
- Stable operating system (OS) installed
- A safe place to leave your device running
- The device should have >2GB of RAM 
- The device should have >15GB of free storage
- If you need a silent node, use a SSD or USB drive

### Steps:
1. Get a cheap (refurbished) laptop or a Raspberry Pi 3B+ or better
2. Install the Decred CLI software for your device 
    - Check your whether you need amd or arm and x64 or x86
    - Folder structures will differ for each OS
    - https://docs.decred.org/wallets/cli/os-differences/
3. Simply configure dcrd, you don't need a wallet
    - Open a terminal (command line) in the folder that contains the software
    - Run the command for your OS to start dcrd
    - Keep dcrd running to download the Decred blockchain
4. While dcrd is syncing, figure out your local and external IP address
    - Local IP: [method will differ for each OS](https://www.howtogeek.com/236838/how-to-find-any-devices-ip-address-mac-address-and-other-network-connection-details/)
    - External IP: https://whatismyipaddress.com/
5. Edit the settings of your router to open port 9108 (port forwarding)
    - This process depends on the type of router you have
    - https://www.wikihow.com/Set-Up-Port-Forwarding-on-a-Router
6. Check a Decred block explorer for the latest block height and wait for dcrd to sync
7. Restart dcrd with `--externalip=[your.external.ip]`
8. Find a safe place for your node where it can run undisturbed
9. Check back once in a while to look for inbound connections

Congratulations, you are now running a Decred full node to support the network!
