# secondary DNS enhance by da3a16
	forked from https://github.com/xzer/wlanprofilemanager
# How to use

- install nodejs
- clone this repository
- add your own profile to profiles.js
- register a task in task scheduler(control panel->administration tools->task scheduler)
    - set wpm.bat as the operation of the task
    - make sure the task will be executed by user "SYSTEM"
    - define the trigger as following:
        - start at: event
        - basic, log: Microsoft-Windows-WLAN-AutoConfig/Operational
        - source: WLAN-AutoConfig
        - event id: 11001