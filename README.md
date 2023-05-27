# DBeaver Workspace for VS Code

How to use it:

1. As a prerequisite, you need a working dev environment in Eclipse. More about it here: https://github.com/dbeaver/dbeaver/wiki/Develop-in-Eclipse.
2. Create system environment variable `DBEAVER_DEVEL_ECLIPSE_PATH` that points to the path with your Eclipse installation used in the first step. 
On macOS, that should be the `Eclipse` folder inside `Eclipse.app/Contents`.
3. Create system environment variable `DBEAVER_DEVEL_ECLIPSE_WORKSPACE_PATH` that points to the path with your Eclipse workspace you used in step 1.
4. Clone this repo alongside the main dbeaver/dbeaver repo. It must result in a structure like the following:
```
some_root_folder_with_your_dbeaver_assets
    — dbeaver                  (a clone of dbeaver/dbeaver repo)
    — dbeaver-workspace-vscode (this repo)
```
5. Edit the `org.jkiss.dbeaver.tp.target` file so the location points to the same folder as `DBEAVER_DEVEL_ECLIPSE_PATH` variable.
6. Open the workspace in VS Code and install recommended extensions. Reload the window.
7. Now you can start DBeaver with the debugger attached using a predefined launch configuration for VS Code.

Happy hacking!
