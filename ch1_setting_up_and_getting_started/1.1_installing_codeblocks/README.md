## What is Code::Blocks? 🤔

**Code::Blocks** is a highly extensible, configurable, and open-source IDE for C, C++, and Fortran. It's designed to be cross-platform, meaning it runs seamlessly on Windows, macOS, and Linux. Code::Blocks includes a compiler (like MinGW for Windows), a debugger, and many other features that streamline the coding process, making it an excellent choice for beginners.

---

## Installation Guides 💻

Follow the instructions below for your specific operating system.

### 🪟 Windows

1. **Download the Installer:**
   * Go to the official Code::Blocks downloads page: [https://www.codeblocks.org/downloads/binaries/](https://www.codeblocks.org/downloads/binaries/)
   * Under "Windows XP / Vista / 7 / 8.x / 10", click on **"Download the binary release"**.
   * Look for the installer that includes the MinGW compiler. It will typically be named something like `codeblocks-XX.XXmingw-setup.exe` (e.g., `codeblocks-25.03mingw-setup.exe`). This version includes the GCC/G++ compiler and GDB debugger, so you don't need to install them separately.
   * Download the file from SourceForge.net.

2. **Run the Installer:**
   * Locate the downloaded `.exe` file and double-click it to start the installation wizard.
   * Click **"Next"** on the welcome screen.
   * Read and **"I Agree"** to the license agreement.
   * For "Choose Components," select **"Full"** installation to ensure all necessary plugins and features are included. Click **"Next"**.
   * Choose your installation directory (the default is usually fine). Click **"Install"**.
   * The installation process will take a few minutes.
   * Once complete, you can choose to run Code::Blocks immediately or click **"Finish"**.

3. **Initial Setup (First Launch):**
   * When you first open Code::Blocks, it should auto-detect the **"GNU GCC Compiler"**. Select it and click **"Set as default"**, then **"OK"**.
   * If prompted to associate Code::Blocks with C/C++ file types, select **"Yes, associate Code::Blocks with C/C++ file types"** and click **"OK"**.

---

### 🍎 macOS

1. **Install Xcode Command Line Tools (Prerequisite):**
   * Code::Blocks on macOS often relies on the Xcode distribution for its compiler. If you don't have Xcode or its command-line tools installed, open your Terminal and run:
     ```bash
     xcode-select --install
     ```
   * Follow the prompts to install the tools.

2. **Download the Disk Image:**
   * Go to the official Code::Blocks downloads page: [https://www.codeblocks.org/downloads/binaries/](https://www.codeblocks.org/downloads/binaries/)
   * Under "Mac OS X", click on **"Download the binary release"**.
   * Download the `.dmg` file (e.g., `CodeBlocks-XX.XX_macOS-YY.Y_x64-wx3.X.X.dmg`).

3. **Install Code::Blocks:**
   * Double-click the downloaded `.dmg` file to open it.
   * Drag the **Code::Blocks** application icon into your **Applications** folder.
   * Close the `.dmg` window and eject the disk image.

4. **Open Code::Blocks (First Launch):**
   * Navigate to your Applications folder and double-click the Code::Blocks icon.
   * You might encounter a security warning about the app being downloaded from the internet. If so, go to **System Settings/Preferences > Security & Privacy > General**, and click **"Open Anyway"** next to the Code::Blocks entry.
   * When Code::Blocks launches for the first time, it should auto-detect the **"GNU GCC Compiler"**. Select it and click **"Set as default"**, then **"OK"**.
   * You might also need to configure the terminal for console programs. Go to **Settings > Environment** and change the "Terminal to launch console programs" to:
     ```
     osascript -e 'tell app "Terminal"' -e 'activate' -e 'do script "$SCRIPT"' -e 'end tell'
     ```

---

### 🐧 Ubuntu Linux

The easiest and recommended way to install Code::Blocks on Ubuntu is via the terminal using `apt`.

1. **Open Terminal:**
   * You can usually open the terminal by pressing `Ctrl + Alt + T` or by searching for "Terminal" in your applications menu.

2. **Update Package List:**
   * It's always a good practice to update your package list before installing new software. Run the following command:
     ```bash
     sudo apt update
     ```
   * Enter your password when prompted.

3. **Install Code::Blocks and Contrib Plugins:**
   * Now, install Code::Blocks along with the `codeblocks-contrib` package, which provides additional plugins and features:
     ```bash
     sudo apt install codeblocks codeblocks-contrib
     ```
   * If prompted, type `Y` and press Enter to confirm the installation.

4. **Launch Code::Blocks:**
   * Once the installation is complete, you can launch Code::Blocks from your applications menu or by typing:
     ```bash
     codeblocks
     ```
     in the terminal.
   * On the first launch, it should auto-detect the **"GNU GCC Compiler"**. Select it and click **"Set as default"**, then **"OK"**.
