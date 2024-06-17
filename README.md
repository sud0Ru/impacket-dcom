# Impacket-DCOM
Adjusted version of the impacket-dcomexec script to work against Windows 10.

If you tried to run the impacket-dcomexec script against Windows 10 using ShellWindows or ShellBrowserWindow DCOM objects, the execution will hang, and you will not be able to execute any commands. After some investigation, it seems that the DCOM object is called successfully, but the problem appears when the smbclient tries to fetch the command output. You can see the whole problem here.

# Cautions
Please don't use this if you don't know how DCOM execution works. ShellWindows or ShellBrowserWindow DCOM objects will trigger pop-ups on the remote hosts.

# Acknowledgment
This script is under development to include more features and bypass some issues. It is part of research related to DCOM that will be published soon.
