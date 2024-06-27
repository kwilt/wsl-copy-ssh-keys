# wsl-copy-ssh-keys

## **Feel free to use, fork, modify.** 

#### This is a bash script that can be used to copy existing SSH keys from your Windows host to WSL and add a specified private key to the authentication agent within WSL.

- Tested and working with WSL2 Ubuntu-22.04

- By default, this script will target `C:\Users\<your logged in Windows account>\.ssh\` for the keys. 
  - This translates to `/mnt/c/Users/<your account>/.ssh/` in WSL. You can hit enter to accept the default.
  - The script will copy **ALL** of the files from the target directory on Windows to WSL at `/home/<current user>/.ssh/`, so your known_hosts, public key, etc., will all be available to your WSL distribution.
  - If you need to specify a different path, it must be accessible from WSL and entered in the linux format. For example: `/mnt/your/path/to/keys`, `/mnt/c/SomeDirectory/JohnSmith123/AnotherDirectory`
    - [Click to learn more about working across file systems in WSL](https://learn.microsoft.com/en-us/windows/wsl/filesystems#file-storage-and-performance-across-file-systems)

- The next prompt will ask for the name of your private key. Once again, you can hit enter to accept the default, 'id_rsa'.
