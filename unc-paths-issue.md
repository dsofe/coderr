Date of error: 11/18/22

<br>

- when `wd` is local drive: unc paths not supported...    
- when `wd` is cloud drive: error in loadNamespace(x): there is no package called 'jsonlite'    
> - not calling on jsonlite in quarto/qmd file  
> - jsonlite is installed and accessible in Rstudio folder; checked using `.libPaths()` and then `list.files("C:/Rstudio")`   

`Help` > `Diagnostics` > `Edit User Prefs File`

```
{
    "initial_working_directory": "~/00-OneDrive-mirror/r-posit",
    "editor_theme": "Tomorrow Night Bright",
    "windows_terminal_shell": "win-cmd",
    "rainbow_parentheses": true,
    "jobs_tab_visibility": "shown",
    "panes": {
        "quadrants": [
            "Source",
            "Console",
            "TabSet1",
            "TabSet2"
        ],
        "tabSet1": [
            "Environment",
            "History",
            "Connections",
            "Packages",
            "VCS",
            "Tutorial",
            "Presentation"
        ],
        "tabSet2": [
            "Files",
            "Plots",
            "Help",
            "Viewer",
            "Presentations"
        ],
        "hiddenTabSet": [
            "Build"
        ],
        "console_left_on_top": false,
        "console_right_on_top": true,
        "additional_source_columns": 0
    },
    "source_with_echo": true,
    "rmd_viewer_type": "pane",
    "default_project_location": "C:/Users/smithda/OneDrive - NYC O365 HOSTED/ofe-research/equity-dashboard/dashboard/dashboard-no1",
    "new_proj_use_renv": true,
    "save_files_before_build": true,
    "shiny_viewer_type": "browser",
    "full_project_path_in_window_title": true,
    "restore_last_project": false,
    "soft_wrap_r_files": true,
    "fold_style": "begin-only",
    "show_rmd_render_command": true,
    "use_tinytex": true
}
```

<br>

the settings supported in the user (or system) `rstudio-prefs.json` file

<br>    

To double check what environment variables are defined in the R environment, run...     

```
> Sys.getenv()
ALLUSERSPROFILE                     C:\ProgramData
APPDATA                             C:\Users\smithda\AppData\Roaming
CLICOLOR_FORCE                      1
CommonProgramFiles                  C:\Program Files\Common Files
CommonProgramFiles(x86)             C:\Program Files (x86)\Common Files
CommonProgramW6432                  C:\Program Files\Common Files
COMPUTERNAME                        DCA18C0263
ComSpec                             C:\WINDOWS\system32\cmd.exe
DISPLAY                             :0
DriverData                          C:\Windows\System32\Drivers\DriverData
GFORTRAN_STDERR_UNIT                -1
GFORTRAN_STDOUT_UNIT                -1
HOME                                //msdcanetapp001m.dca.nycnet/user_data$/SmithDA
HOMEDRIVE                           H:
HOMEPATH                            \
HOMESHARE                           \\msdcanetapp001m.dca.nycnet\user_data$\SmithDA
LOCALAPPDATA                        C:\Users\smithda\AppData\Local
LOGONSERVER                         \\DCABWDC01
MPLENGINE                           tkAgg
MSYS2_ENV_CONV_EXCL                 R_ARCH
NUMBER_OF_PROCESSORS                8
OneDrive                            C:\Users\smithda\OneDrive - NYC O365 HOSTED
OneDriveCommercial                  C:\Users\smithda\OneDrive - NYC O365 HOSTED
OS                                  Windows_NT
PATH                                C:\Program Files\R\R-4.1.3\bin\x64;C:\Program Files (x86)\Common
                                    Files\Oracle\Java\javapath;C:\Program Files\Intel\iCLS
                                    Client\;C:\WINDOWS\system32;C:\WINDOWS;C:\WINDOWS\System32\Wbem;C:\WINDOWS\System32\WindowsPowerShell\v1.0\;C:\WINDOWS\System32\OpenSSH\;C:\Program
                                    Files (x86)\OPOS\Epson2;C:\Program Files (x86)\Intel\Intel(R) Management
                                    Engine Components\DAL;C:\Program Files\Intel\Intel(R) Management Engine
                                    Components\DAL;C:\Users\smithda\AppData\Local\Microsoft\WindowsApps;C:\Users\smithda\AppData\Local\Programs\Microsoft
                                    VS
                                    Code\bin;C:\Users\smithda\AppData\Local\Programs\Quarto\bin;C:\Users\smithda\AppData\Local\Programs\Julia-1.7.3\bin;C:\Program
                                    Files\JetBrains\PyCharm Community Edition
                                    2022.2\bin;;C:\Users\smithda\AppData\Local\Programs\MiKTeX\miktex\bin\x64\;C:/Users/smithda/AppData/Local/Programs/Quarto/bin
PATHEXT                             .COM;.EXE;.BAT;.CMD;.VBS;.VBE;.JS;.JSE;.WSF;.WSH;.MSC
PROCESSOR_ARCHITECTURE              AMD64
PROCESSOR_IDENTIFIER                Intel64 Family 6 Model 94 Stepping 3, GenuineIntel
PROCESSOR_LEVEL                     6
PROCESSOR_REVISION                  5e03
ProgramData                         C:\ProgramData
ProgramFiles                        C:\Program Files
ProgramFiles(x86)                   C:\Program Files (x86)
ProgramW6432                        C:\Program Files
PSModulePath                        C:\Program
                                    Files\WindowsPowerShell\Modules;C:\WINDOWS\system32\WindowsPowerShell\v1.0\Modules
PUBLIC                              C:\Users\Public
PyCharm Community Edition           C:\Program Files\JetBrains\PyCharm Community Edition 2022.2\bin;
PYTHONIOENCODING                    utf-8
QT_D3DCREATE_MULTITHREADED          1
R_ARCH                              /x64
R_CLI_HAS_HYPERLINK_IDE_HELP        true
R_CLI_HAS_HYPERLINK_IDE_RUN         true
R_CLI_HAS_HYPERLINK_IDE_VIGNETTE    true
R_COMPILED_BY                       gcc 8.3.0
R_DOC_DIR                           C:/PROGRA~1/R/R-41~1.3/doc
R_HOME                              C:/PROGRA~1/R/R-41~1.3
R_LIBS_USER                         //msdcanetapp001m.dca.nycnet/user_data$/SmithDA/R/win-library/4.1
R_USER                              //msdcanetapp001m.dca.nycnet/user_data$/SmithDA
RMARKDOWN_MATHJAX_PATH              C:/Users/smithda/AppData/Local/Programs/RStudio/resources/mathjax-27
RS_LOCAL_PEER                       \\.\pipe\54842-rsession
RS_RPOSTBACK_PATH                   C:/Users/smithda/AppData/Local/Programs/RStudio/bin/rpostback
RS_SHARED_SECRET                    c913907e-7ef6-439c-bbaa-572d5dcac010
RSTUDIO                             1
RSTUDIO_CLI_HYPERLINKS              true
RSTUDIO_CONSOLE_COLOR               256
RSTUDIO_CONSOLE_WIDTH               80
RSTUDIO_MSYS_SSH                    C:/Users/smithda/AppData/Local/Programs/RStudio/bin/msys-ssh-1000-18
RSTUDIO_PANDOC                      C:/Users/smithda/AppData/Local/Programs/RStudio/bin/quarto/bin/tools
RSTUDIO_PROGRAM_MODE                desktop
RSTUDIO_SESSION_PID                 14320
RSTUDIO_SESSION_PORT                54842
RSTUDIO_USER_IDENTITY               smithda
RSTUDIO_WINUTILS                    C:/Users/smithda/AppData/Local/Programs/RStudio/bin/winutils
RTOOLS40_HOME                       C:\rtools40
SESSIONNAME                         Console
SystemDrive                         C:
SystemRoot                          C:\WINDOWS
TEMP                                C:\Users\smithda\AppData\Local\Temp
TERM                                xterm-256color
TMP                                 C:\Users\smithda\AppData\Local\Temp
USERDNSDOMAIN                       DCA.NYCNET
USERDOMAIN                          DCA
USERDOMAIN_ROAMINGPROFILE           DCA
USERNAME                            smithda
USERPROFILE                         C:\Users\smithda
windir                              C:\WINDOWS
```

