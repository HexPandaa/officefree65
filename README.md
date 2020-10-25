### Here from "Your version of OfficeFree65 is outdated"?
The latest update broke older versions of scripts.
Please downloads the latest version at https://github.com/3rik/OfficeFree65/releases

# OfficeFree65
A simple script that easily activates and installs the latest microsoft office 365. <br>
## Table of contents
* [General info](#general-info)
* [Usage](#usage)
* [FAQ](#faq)
## General info
This script downloads the latest Office 365 from microsoft directly, installs it and finally activates it. <br>
The installed office will have full support for <b>Microsoft Sign In, Settings Sync, Addins, Connected Services like OneDrive, Office Updates directly from Microsoft (on Insider, DevMain and Standard channels)</b> and basically every other feature in office 365 apart from the 1TB Cloud Storage. <br>
<details>
  <summary>Click to see images</summary>
<img src="https://i.imgur.com/CnV1oFc.png" width="300"> <img src="https://i.imgur.com/M1JCrLw.png" width="300"> <img src="https://i.imgur.com/i0WnCoD.png" width="300"> <img src="https://i.imgur.com/DCP0bkK.png" width="300"> <img src="https://i.imgur.com/Gk95JEO.png" width="300"> <img src="https://i.imgur.com/Y78zc9q.png" width="300"> <img src="https://i.imgur.com/4xd2rOh.png" width="300"> <img src="https://i.imgur.com/kxgxjtX.png" width="300"><br>
<h3>Being 365 apps, the installed apps also have the new UI</h3>
<img src="https://i.imgur.com/S1RTKbt.png" width="900">
<br><img src="https://i.imgur.com/0fUxuIW.png" width="900">
</details>

The following apps will be installed: <br>

    Microsoft Office Word
    Microsoft Office Powerpoint
    Microsoft Office Publisher
    Microsoft Office Access
    Microsoft Office Outlook
    Microsoft Office OneNote
    Microsoft Office Excel
    Microsoft Skype for Business
    Microsoft Office Project
    Microsoft Office Visio

Support for Office 365 Insider builds and Alpha (DevMode) builds added in 2.0.0. <br>
Support for optionally deactivating specific components planned. <br>
<br>
Go to the releases tab to download.
<br>
Main repo with sources for the components is at: https://codeberg.org/3rik/OfficeFree65
<br>
This page should recieve updates on the releases channel a couple minutes after codeberg, but you may still want to check there for a newer version just in case.
<br>
<b> Note that it only supports 64bit Windows 8, 8.1 and 10. </b> <br><br>
<img src="https://i.imgur.com/8tWyKAo.png">

## Usage
1. Simply double click the script to run it.<br>
2. It requires administrator permissions and will try to ask for them, hit "yes" if the prompt appears. If it can't get administrator permissions, you will get this message:<br>
<img src="https://i.imgur.com/Ubt7QqB.png" width="500"><br>
    * An option to skip this check is available [here](#advanced-settings).
<br> 
3. For a normal installation, select 1 when asked to begin the installation.
<br> 
4. Selecting 1 when asked if you already have office installed will launch a script to delete it and all it's traces, which is important as not doing so could break the new installation. If you want to try without deleting it, or if you dont have office installed already, select 2.
    * The same script is also available [here](#built-in-tools). <br>
5. Select the number for the channel you want to install from.
    * 1 is the normal channel
    * 2 is the normal insider channel, for beta builds
    * 3 is the special DogfoodDevMain channel (same as the MicrosoftElite channel) and has alpha builds even newer than those in the insider channel. <br>
6. The script will download and run the installation. <br>
7. Before activating, you will be prompted to disable your antivurus. While this is likely not required to do with Windows Defender, other antivuruses may detect the KMS activation script as a virus. It is up to you whether you want to disable or not.
8. Done!

### Built in tools
From version 2.2.0 onwards, some tools have been included in the script. For now there are only two, though I plan to expand on this in the future.
#### Cleanup script
Normally run at the end of a successful installation, this cleans up any temproary files made by this script.
Useful if the script crashes or something stops it from doing this process itself.
#### Office uninstallation script
This was already present in the script itself (when asked if you already have office installed) but now is also in the utilities menu. Deletes <b>ALL</b> installations of Microsoft Office

### Advanced Settings
From version 2.2.0 onwards, the file includes some settings. <br>
* Skip version check - Skips checking for supported OS version. Set to 1 to enable.
* Skip admin check - Skips checking for administrator permissions. Set to 1 to enable.
* Options to run both utilties automatically (instantly upon running the script, no prior user input required.) Useful if you want to integrate one of the tools into your script or something.
* Debug Mode - Useless to most, outputs debug info prompts througout the script.
* Beta Script - Runs the 3rikscript from https://codeberg.org/3rik/OfficeFree65/raw/branch/main/Recources/Beta/3rikscript.bat instead of the standard source. May be unstable, as I use this to test releases before I release them.
* Custom Script - Run a custom script from your hard drive instead of downloading the latest 3rikscript from here. Useful if you want to run a modified version.
* Master settings toggle - sets whether or not to listen to the settings in the OfficeFree65.bat script. Default is 2, but when set to 1 it will not send settings variables to 3rikscript.bat, and the variables applied there will take over. Must also be set in 3rikscript.bat to work, use together with customscript.


## FAQ
<h3>Why does it say "Microsoft Office Mondo 2016" on the activation page?</h3>
Being a monthly activation subscription, KMS activation dosen't work well when you try to activate the product as a 365 subscription. Activating as Mondo 2016 fixes that. <b> You will still receive all features and feature updates as Office 365 ProPlus.</b>
<br>
<h3>Why are the files on codeberg and not github?</h3>
Github is owned by Microsoft. I don't know how long this repo would survive over here.
<br>
<h3>Bugs</h3>
I'm still a noob by most developer's standards, so there may be issues I haven't noticed yet, although I have tried to iron out as many as possible. Please report them here on the issues tab, or for a possibly faster reponse, at https://codeberg.org/3rik/OfficeFree65/issues.
<br><br>

## Credits
The credits for most of this project go to the developers of Yet Another Office Click To Run Installer and KMS activator. This is also based on a guide here: https://docs.google.com/document/d/1K-4oqnyomXCibQfOJkYbLqeKTmO7ApoGRk_EscaWnEk/preview which achieves the same but has more steps involved.
<br>
All I did was simplify the process a bit by putting it into one script that does most of the work for you.

