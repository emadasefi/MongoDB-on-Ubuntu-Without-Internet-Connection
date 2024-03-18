Install Offline Repository MongoDB on Ubuntu 
====================================
▚ Install Offline Repository MongoDB v4.4.15 on Linux — Ubuntu / Debian — Without Internet Connection

▚ Let's say you have a machine with no internet connection which runs Ubuntu, and you wish to install MongoDB not included in the provided apt-get repository Or installation online process is very difficult.

▚ You Followed The Steps In This Guide and Download and Extract the "mongodb4-emadasefi.ir.zip" and Move the Directory to the Desired.

▚ I will show you how to install MongoDB on linux step by step, in this tutorial I’m using Ubuntu 18.04 distro. Okay, let’s get started.


## ▚ Step 1: Downloading Offline Repository MongoDB (.deb)
To Download An ZIP File (Include Its deb Package) and Extract ZIP File

Link Download : https://www.mediafire.com/file/a5u4edms7smdyvp/mongodb4-emadasefi.ir.zip/file


## ▚ Step 2: Using Offline Repository MongoDB
#> cd /etc/apt/

Rename File sources.list to sources.list_2

Make New File to be Name: sources.list

Now You Can Add Line to the /etc/apt/sources.list file :

deb [trusted=yes] file:/home/username/mongodb4-emadasefi.ir/ ./
#

Run the command:

Maybe You Have an Error in NOT Permission Directory "mongodb4-emadasefi.ir" Assign Completely Full Permission to the Directory and Give a User

#> sudo apt update


## ▚ Step 3: Installing Offline Repository
#> sudo apt install mongodb-org


## ▚ Step 4: Enable Service
After You Installing the Service, Next You Need to Enable it, so Mongodb Will Automatically Started When You Turn on the PC. Enable it by This Command:

#> sudo systemctl enable mongod.service


## ▚ Step 5: Start the MongoDB
Final Step of this Installation is to Start the Mongodb, Your MongoDB is Ready. Start by This Command:

#> sudo systemctl start mongod.service


## — Completed—
Go to Directory /etc/apt/ and Remove File "sources.list" and Replace "sources.list_2" and Run Message ($ sudo apt update)
#
Finish…
#
Please Leave Your Comments if You Got Some Trouble.
