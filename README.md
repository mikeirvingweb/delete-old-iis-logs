# Delete old IIS Logs

A simple Batch File to Delete IIS Logs older than 7 days on Windows Server.

### Installation

➕ Alter the script file to set your correct *IIS Logs Folder* and *number of days* you'd like to delete beyond (default 7).

forfiles /p `"C:\inetpub\logs\LogFiles"` /s /m *.* /c "cmd /c Del @path" /d -`7`

### Usage

🧑‍💻 Run `delete-old-iis-logs` in a *Command Prompt*.

⏰ Or setup a *Scheduled Task* to run the script, in *Windows Task Scheduler*.

### Contributions

🍴 Feel free to Fork / Branch / Modify, raise any Pull Requests for changes.

### Author

Written by Mike Irving © 2022
