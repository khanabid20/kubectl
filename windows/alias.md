### Create Aliases
1. Create a folder %USERPROFILE%\.cmds
2. Create a batch script (`kubectl.bat`) with aliases  
    e.g
    ```
    @echo off
    
    doskey k="kubectl" $*
    doskey kgp="kubectl" get pods
    doskey myprog="switch-env.bat" myprog $*

    ```
3. Win + Run > regedit > "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Command Processor"  
   Create "AutoRun" as string value and set the path of the script along with the script name.
    ![image](https://github.com/khanabid20/kubectl/assets/33711981/bf6bc409-f88b-424d-ade8-0269f9353407)


### Ref:
* https://support.enthought.com/hc/en-us/articles/360000300703-Setting-Command-Aliases-on-Windows
