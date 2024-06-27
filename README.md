# wsl-copy-ssh-keys

**Feel free to use, fork, modify.** 

Copy SSH keys from Windows to WSL2 and add specified private key to authentication agent in WSL.

By default, this script will look in `C:\Users\<your logged in Windows account>\.ssh\` for the keys. 

This translates to `/mnt/c/Users/<your account>/.ssh/` in WSL. You can hit enter to accept the default.
If you need to specify a different path, it must be accessible from WSL and entered in the linux format. For example: `/mnt/your/path/to/keys`, `/mnt/c/SomeDirectory/JohnSmith123/AnotherDirectory`

The next prompt will ask for the name of your private key. Once again, you can hit enter to accept the default, 'id_rsa'.
