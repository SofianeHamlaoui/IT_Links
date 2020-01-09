|    | A                                                                                                                                                                                     |
|----|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1  | Boot from the Windows 10 DVD.                                                                                                                                                        |
| 2  | Make sure that your PC setup is configured to boot from a DVD and that UEFI and Secure Boot are disabled.                                                                            |
| 4  | Press SHIFT + F10 to open a command prompt.                                                                                                                                         |
| 6  | Replace the file utilman.exe with cmd.exe.                                                                                                                                         |
| 7  | Before you do this, you should make a copy of utilman.exe so that you can restore it later.                                                                                         |
| 8  | Note that you can only restore this file if you boot again from the Windows DVD.                                                                                                     |
| 9  | Windows 10 is usually installed on drive D: if you boot from a DVD.                                                                                                                  |
| 10 | You can verify this with "dir d:windowssystem32utilman.exe."                                                                                                                  |
| 11 | If the system can't find utilman.exe, try other drive letters.                                                                                                                      |
| 13 | move d:windowssystem32utilman.exe d:windowssystem32utilman.exe.bak                                                                                                     |
| 14 | copy d:windowssystem32cmd.exe d:windowssystem32utilman.exe                                                                                                              |
| 16 | After you have replaced utilman.exe successfully, you can remove the DVD and restart your problematic Windows 10 installation:                                                       |
| 18 | wpeutil reboot                                                                                                                                                                        |
| 19 | Reboot Windows 10                                                                                                                                                                     |
| 20 | On the Windows 10 sign-in page, click the Utility Manager icon                                                                                                                       |
| 22 | Since we replaced the Utility Manager with the cmd.exe, a command prompt should open now. Don’t worry about the error message.                                                     |
| 24 | You can now add a new user with the command below.                                                                                                                                   |
| 25 | We also have to add the user to the administrator group so that we regain full control of our Windows installation.                                                                  |
| 26 | Replace <username> with the account name of your choice.                                                                                                                             |
| 27 | Note that the account name must not exist on this Windows installation.                                                                                                              |
| 28 | Don’t let the Windows 10 screen saver distract you.                                                                                                                                  |
| 30 | net user <username> /add                                                                                                                                                              |
| 31 | net localgroup administrators <username> /add                                                                                                                                         |
| 33 | Click the screen to make the sign-in page appear again.                                                                                                                             |
| 34 | Your new account should show up, and you can sign in without a password.                                                                                                             |
| 35 | You can now access the files associated with your Microsoft account in the C:Users folder.                                                                                         |
| 37 | A shorter way to reset the password of a local account is to replace the first command in step 6 with the following command. (In this case, you don’t need to create a new user.) |
| 39 | net user <username> <password>                                                                                                                                                        |
| 41 | list users                                                                                                                                                                            |
| 42 | net user > users.txt                                                                                                                                                                 |
