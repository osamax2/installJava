# How to Install Java and IntelliJ IDEA Community Edition

## 1. Install Java

### Windows
1. **Download Java JDK:**
   - Visit the [Oracle Java Downloads page](https://www.oracle.com/java/technologies/javase-downloads.html).
   - Choose the latest JDK version for Windows and download the installer.

2. **Run the Installer:**
   - Double-click the downloaded `.exe` file.
   - Follow the installation wizard and accept the default settings.

3. **Set JAVA_HOME Environment Variable:**
   - Open the Start Menu and search for "Environment Variables."
   - Click on "Edit the system environment variables."
   - In the System Properties window, click on "Environment Variables."
   - Under "System Variables," click "New" and add:
     - **Variable Name:** `JAVA_HOME`
     - **Variable Value:** Path to your JDK installation (e.g., `C:\Program Files\Java\jdk-XX.X.X`).
   - Click "OK" to save.

4. **Update Path Variable:**
   - In the same "Environment Variables" window, locate the "Path" variable under "System Variables."
   - Click "Edit" and add the path to `bin` inside your JDK installation (e.g., `C:\Program Files\Java\jdk-XX.X.X\bin`).
   - Click "OK" to save.

5. **Verify Installation:**
   - Open Command Prompt and run: `java -version`
   - The output should display the installed JDK version.

---

### macOS
1. **Install Homebrew (Optional):**
   - If Homebrew is not installed, open Terminal and run:
     ```sh
     /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
     ```

2. **Install Java JDK:**
   - Run the following command:
     ```sh
     brew install --cask temurin
     ```
     This installs the latest OpenJDK.

3. **Verify Installation:**
   - Run the following in Terminal:
     ```sh
     java -version
     ```
   - The output should display the installed JDK version.

---

### Linux
1. **Update Package List:**
   - Open Terminal and run:
     ```sh
     sudo apt update
     ```

2. **Install OpenJDK:**
   - Run:
     ```sh
     sudo apt install openjdk-17-jdk
     ```
     Replace `17` with the desired version.

3. **Set JAVA_HOME Environment Variable:**
   - Open the `~/.bashrc` or `~/.zshrc` file and add:
     ```sh
     export JAVA_HOME=/usr/lib/jvm/java-17-openjdk-amd64
     export PATH=$JAVA_HOME/bin:$PATH
     ```
     Replace `java-17-openjdk-amd64` with your installed version's path.
   - Run:
     ```sh
     source ~/.bashrc
     ```

4. **Verify Installation:**
   - Run:
     ```sh
     java -version
     ```
   - The output should display the installed JDK version.

---

## 2. Install IntelliJ IDEA Community Edition

### Windows
1. **Download IntelliJ IDEA:**
   - Visit the [IntelliJ IDEA download page](https://www.jetbrains.com/idea/download/).
   - Download the Community Edition for Windows.

2. **Run the Installer:**
   - Double-click the downloaded `.exe` file.
   - Follow the installation wizard and select the desired options.

3. **Launch IntelliJ IDEA:**
   - After installation, launch IntelliJ IDEA and configure as needed.

---

### macOS
1. **Download IntelliJ IDEA:**
   - Visit the [IntelliJ IDEA download page](https://www.jetbrains.com/idea/download/).
   - Download the Community Edition for macOS.

2. **Install IntelliJ IDEA:**
   - Open the downloaded `.dmg` file.
   - Drag and drop IntelliJ IDEA into the Applications folder.

3. **Launch IntelliJ IDEA:**
   - Open IntelliJ IDEA from the Applications folder and configure as needed.

---

### Linux
1. **Download IntelliJ IDEA:**
   - Visit the [IntelliJ IDEA download page](https://www.jetbrains.com/idea/download/).
   - Download the tar.gz file for Linux.

2. **Extract the Archive:**
   - Open Terminal and navigate to the download directory. Run:
     ```sh
     tar -xzf ideaIC-*.tar.gz
     ```

3. **Run IntelliJ IDEA:**
   - Navigate to the `bin` directory inside the extracted folder. Run:
     ```sh
     ./idea.sh
     ```

4. **Create Desktop Entry (Optional):**
   - In IntelliJ IDEA, go to **Tools > Create Desktop Entry** to add a shortcut.

---

You're now ready to use Java and IntelliJ IDEA Community Edition on your system!
