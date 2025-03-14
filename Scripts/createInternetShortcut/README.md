# Create Internet Shortcut

### About

This Shell script creates custom shortcuts on user's desktops for http(s), smb, ftp, and vnc addresses. Administrators can set a display name and specify an icon if disired.  If no icon is specified, the script will use a default icon depending on the link type. 


### Dependencies

- Privacy Profile (PPPC) granting the Kandji Agent access to Finder Apple Events.


### Script Modification

1. Open the script in a text editor such as BBEdit or VSCode.
1. Update the `HOSTNAME` variable with the correct URI, `DISPLAYNAME` with the display name of the shortcut, and `ICON` with the full path of your desired icon if you do not want to use the default icons.

```Shell
        ########################################################################################
        ###################################### VARIABLES #######################################
        ########################################################################################

        # The address that you want the shortcut to open.
        HOSTNAME="https://kandji.io"

        # The name that will display to users.
        DISPLAYNAME="My Favorite MDM"

        # Full path to the icon to be used for the shortcut.  A blank variable will use a 
        # default icon, depending on the link type.
        # example: ICON="/Library/Kandji/Kandji Agent.app/Contents/Resources/AppIcon.icns"
        ICON=
```
1. Save and close the script.
1. In Kandji, create a new Custom Script.
1. Past your modified createInternetShortcut.zsh script in the body of the script.


### Examples

- Custom Icon:
<br><img src="/Scripts/createInternetShortcut/images/CustomIcon-code.png" width="600" align="middle"></img><img src="/Scripts/createInternetShortcut/images/CustomIcon-icon.png" width="150" align="middle"></img>

- HTTP and HTTPS Default Icon:
<br><img src="/Scripts/createInternetShortcut/images/DefaultHTTPS-code.png" width="600" align="middle"></img><img src="/Scripts/createInternetShortcut/images/DefaultHTTPS-icon.png" width="150" align="middle"></img>

- SMB and FTP Default Icon:
<br><img src="/Scripts/createInternetShortcut/images/DefaultSMB-code.png" width="600" align="middle"></img><img src="/Scripts/createInternetShortcut/images/DefaultSMB-icon.png" width="150" align="middle"></img>

- VNC Default Icon:
<br><img src="/Scripts/createInternetShortcut/images/DefaultVNC-code.png" width="600" align="middle"></img><img src="/Scripts/createInternetShortcut/images/DefaultVNC-icon.png" width="150" align="middle"></img>



