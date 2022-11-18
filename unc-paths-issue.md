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
