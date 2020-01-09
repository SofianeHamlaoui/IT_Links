|    | A                                                                                                                                                                                             |
|----|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1  | A workaround to install .NET Framework 1.1 in Windows 7 can be implemented through the following steps:                                                                                     |
| 2  | Create a new folder named DotNet in C: drive (Example: C:DotNet)                                                                                                                        |
| 3  | Download Microsoft .NET Framework 1.1 Redistributable Package (dotnetfx.exe)  . When downloading the setup file, use the SAVE AS option and save the file as dotnetfx.exe.            |
| 4  | Download Microsoft .NET Framework 1.1 Service Pack 1 (NDP1.1sp1-KB867460-X86.exe)  . When downloading the setup file, use the SAVE AS option and save the file as dotnetfxsp1.exe. |
| 5  | Move both installation files into the same directory (i.e. C:DotNet).                                                                                                                  |
| 6  | In the Start menu search box, type CMD, then right-click the cmd.exe item on the start menu and open a command prompt as Administrator.                                                    |
| 7  | Access the directory where the two installation setup files for .NET 1.1 are saved (i.e. C:DotNet).                                                                                  |
| 8  | Run the following commands individually. (These will create a unified install utility for .NET 1.1 called netfx.msi.)                                                                  |
| 9  | dotnetfx.exe /c:"msiexec.exe /a netfx.msi TARGETDIR=C:DotNet"                                                                                                                            |
| 10 | Click"Yes" when prompted to answer "would you like to install Microsoft .NET Framework 1.1. Package?"                                                                                      |
| 11 | dotnetfxsp1.exe /Xp:C:DotNetnetfxsp.msp                                                                                                                                                 |
| 12 | msiexec.exe /a c:DotNetnetfx.msi /p c:DotNetnetfxsp.msp                                                                                                                            |
| 13 | Install Microsoft .NET Framework 1.1 with slipstreamed/integrated Service Pack 1 by running netfx.msi created in the working folder.                                                      |
