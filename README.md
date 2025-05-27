# Osu Background Nuker

Title is self explanatory.

Python script that fetches all of the beatmaps in your Osu! song folder, then deletes all of the background images in order to save space.

The background images are immediately deleted, not moved to the recycle bin.

## How to run

### Windows

Either download the latest release on the [Releases](https://github.com/AmineLeCepe/OsuBackgroundNuker/releases) tab, or:

- Download and install the latest [Python](https://www.python.org/downloads/) release
- Clone this repository (using git or by downloading the source code)
- Open either Powershell or CMD and write the following command inside of the source code directory:
  
```
python3 main.py
```

  - If you wish to specify a custom song folder, use the **--path** flag either this way:
    
    ```
    python3 main.py --path <Path to your osu! song folder>
    ```
    or this way:
    
    ```
    OsuBackgroundNuker.exe --path "<Path to your osu! song folder>" (DONT FORGET THE QUOTES PLS)
    ```
    
    depending on your installation method.
    Passing an invalid directory will result in a crash and will not delete anything.

### Linux

- Download **Python** and **Git** (Check your distro's documentation on how to do it)
- Enter the following commands:
  
```
git clone https://github.com/AmineLeCepe/OsuBackgroundNuker/
cd OsuBackgroundNuker
python main.py
```

  - If you wish to specify a custom song folder, use the **--path** flag:
    
    ```
    python main.py --path <Path to your osu! song folder>
    ```
    
## How to use
- If you specify an invalid path, the program will exit immediately.
- You will be prompted to enter the word **"CONFIRM"** in **all uppercase** to execute the program, entering any other string will end up in the program exiting.
- By entering "CONFIRM", the program will run and all of the background images/videos will be **PERMANENTLY DELETED**
- The program can hypothetically be used for any subfolder containing .jpeg, .jpg, .png, .mp4 files within a parent folder
