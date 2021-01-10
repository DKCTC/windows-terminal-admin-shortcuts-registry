# windows-terminal-admin-shortcuts-registry
Windows Registry files for adding Explorer context-menu options for opening regular and elevated shells for Command Prompt, and Windows Terminal Command Prompt, Windows PowerShell, WSL Ubuntu, and WSL Debian (can be modified for other distros)

Includes files for adding both regular and elevated options to the same menu, or for adding the elevated options to the elevated menu (Shift+Right-click, Shift+Context menu key, or Shift+F10). Also includes keyboard shortcuts for the elevated menu.

These items are thoroughly documented at the links below:

https://dkcool.tailnet.net/2019/05/add-open-windows-terminal-command-prompt-to-the-explorer-context-menu-in-windows-10/
https://dkcool.tailnet.net/2019/05/add-open-admin-command-prompt-to-the-explorer-context-menu-in-windows-10/

If you don't bother going there to read the articles, then make sure that you download the **terminal.ico** file and place it in the folder below AFTER installing Windows Terminal from the Microsoft Store:

%localappdata%\Packages\Microsoft.WindowsTerminal_8wekyb3d8bbwe\LocalState

The icon is also available from the repo for Windows Terminal:

https://raw.githubusercontent.com/microsoft/terminal/master/res/terminal.ico

If you have multiple versions of Ubuntu or Debian installed, you will need to modify the values in the menu labels and the launch commands to specify which version to use.

Ubuntu and Debian both use the WSL Tux icon because there are no consistent paths to the EXEs for Windows Apps. This is why you need to download the Windows Terminal icon above and place it into the given folder.

**KNOWN ISSUE:** When trying to open a Windows Terminal instance on the root folder of a drive, instead of opening the root folder, it will open the user profile folder. I will update this if I ever find a fix. I am sure that there is some PowerShell scripting that can be put together to handle this situation, and that the command would still be one long line.

If anything besides that isn't working, please create an Issue.
