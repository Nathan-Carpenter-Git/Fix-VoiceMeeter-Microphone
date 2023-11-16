# Fix-VoiceMeeter-Microphone

## Author
_Created by Nathan Carpenter_

## About
- Fixes "popping" sound from the microphone from VoiceMeeter.
- Script changes affinity of audiodg.exe which has been causing issues with VoiceMeeter.

## Prerequisites
- Supports only Windows operating systems.
- Windows system is remote signed, if it is not, the script will not run. See "How to remote sign Windows" below.

## How to use
- Make sure to run the program with PowerShell. Can be run through the PowerShell console, or double-clicked and run with PowerShell.

## How to remote sign Windows
1. Open PowerShell as administrator
2. Type in the following command: *Set-ExecutionPolicy RemoteSigned*
3. Now you should be able to run the script. 

## Recommendation (Task Scheduler)
- Windows will change the affinity of audiodg.exe back to default on startup.
- Create a task with a task scheduler to automatically run the script on Windows startup to override default affinity.
- Follow these settings when creating the task:
- ![image](https://github.com/Nathan-Carpenter-Git/Fix-VoiceMeeter-Microphone/assets/144058518/5eb1c7bf-6453-4b41-b8cc-c0092bb399ae)
- ![image](https://github.com/Nathan-Carpenter-Git/Fix-VoiceMeeter-Microphone/assets/144058518/d22ed525-8b58-4cf5-9038-fa7d29a936f2)
- Leave the rest of the settings default.
