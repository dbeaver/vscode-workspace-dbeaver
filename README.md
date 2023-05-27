# DBeaver Workspace for VS Code

How to use it:

1. As a prerequisite, you need a working dev environment in Eclipse. More about it here: https://github.com/dbeaver/dbeaver/wiki/Develop-in-Eclipse.
2. Create system environment variable `DBEAVER_DEVEL_ECLIPSE_PATH` that points to the path with your Eclipse installation used in the first step. 
On macOS, that shoud be the `Eclipse` folder inside `Eclipse.app/Contents`.
3. Create system environment variable `DBEAVER_DEVEL_ECLIPSE_WORKSPACE_PATH` that points to the path with your Eclipse workspace you used in step 1.
4. Clone this repo alogside the main dbeaver/dbeaver repo. This must result in structure like the following:
```
some_root_folder_with_your_dbeaver_assets
    — dbeaver                  (a clone of dbeaver/dbeaver repo)
    — dbeaver-workspace-vscode (this repo)
```
5. Edit the `org.jkiss.dbeaver.tp.target` file so the location points to the same folder as `DBEAVER_DEVEL_ECLIPSE_PATH` variable.
6. Open VS Code. Install the following:
  - https://marketplace.visualstudio.com/items?itemName=vscjava.vscode-java-pack
  - https://marketplace.visualstudio.com/items?itemName=yaozheng.vscode-pde
7. Now you can open the workspace in VS Code and start debugging.

Happy hacking!
 
