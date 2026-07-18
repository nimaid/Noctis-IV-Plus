# How To Compile Noctis IV Plus
No DeLorean needed for this trip through time. You will however need a computer capable of running DOSBox-X.

## Preparing The DOSBox-X Build Environment
Before moving onto the following steps, [download DOSBox-X from here](https://dosbox-x.com/) and install it to it's default location. All the default settings should be good.

### Setup A DOSBox-X `C:` Drive Folder
1. Make a new folder in your root directory named `DOS_C`.
    - On `Windows`, the root directory is `C:`, so your DOS `C:` drive directory should be `C:\DOS_C\`.
    - On `*nix`, the root directory is `/`, so your DOS `C:` drive directory should be `/DOS_C/`.
2. Open DOSBox-X. From the toolbar, select `Main > Configuration tool`.
3. Click the `AUTOEXEC.BAT` button on the popup window.
4. Enter the following into the text box window, replacing `{DOS_C}` with your DOS `C:` drive directory:
```
mount C {DOS_C}
c:
```
5. Click `OK`.
6. Click `Save...`, and then click `Save` again on the popup.
7. Click `Close` and then close DOSBox-X.

### Install Borland C++ 3.1 for DOS
1. Download Borland C++ 3.1 for DOS here: [BCPP31.ZIP](https://archive.org/download/bcpp31/BCPP31.ZIP).
2. Make a new folder on your DOS `C:` drive named `bc.31`.
3. Extract the contents of the `BCPP31.ZIP` file to the `bc.31` folder to finish the install.

### Copy The Noctis Folder
Make a copy of the `Noctis-IV-Plus` folder in the root of your DOS `C:` drive.

## Compiling
1. Open DOSBox-X.
2. Run the command `cd Noctis-IV-Plus\source` in order to switch to the source code directory.
3. Run the command `compile.bat`.
    - If the build failed, it will let you know and prompt you to press a key to exit.
    - If the build succeeded, it will prompt you to press a key to run the newly compiled Noctis IV Plus.

The compiled binary is automatically copied over to the `modules` folder inside the main `Noctis-IV-Plus` folder.