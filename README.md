# JDK-Setup

### Windows:

1. **Download JDK:**
   - Visit the [Oracle JDK Downloads](https://www.oracle.com/java/technologies/javase-downloads.html) page.
   - Choose the desired JDK version and download the Windows installer (`.exe` file).
   - Accept the license agreement during the download.

2. **Install JDK:**
   - Run the downloaded installer.
   - Follow the on-screen instructions to complete the installation.
   - Note the installation directory (e.g., `C:\Program Files\Java\jdk-<version>`).

3. **Set Environment Variables:**
   - Set the `JAVA_HOME` system environment variable to the JDK installation directory.
   - Add the `bin` directory of the JDK to the system `PATH` variable.

4. **Verify Installation:**
   - Open a Command Prompt and run:
     ```bash
     java -version
     javac -version
     ```

### macOS:

1. **Download JDK:**
   - Visit the [Oracle JDK Downloads](https://www.oracle.com/java/technologies/javase-downloads.html) page.
   - Choose the desired JDK version and download the macOS installer (`.dmg` file).
   - Accept the license agreement during the download.

2. **Install JDK:**
   - Open the downloaded `.dmg` file.
   - Drag the JDK package to the Applications folder.
   - Note the installation directory (e.g., `/Library/Java/JavaVirtualMachines/jdk-<version>.jdk/Contents/Home`).

3. **Set Environment Variables (optional):**
   - macOS usually sets the required environment variables automatically.
   - If necessary, you can add the following to your shell profile (e.g., `~/.bash_profile` or `~/.zshrc`):
     ```bash
     export JAVA_HOME=/Library/Java/JavaVirtualMachines/jdk-<version>.jdk/Contents/Home
     export PATH=$PATH:$JAVA_HOME/bin
     ```

4. **Verify Installation:**
   - Open a Terminal and run:
     ```bash
     java -version
     javac -version
     ```

### Linux (Ubuntu as an example):

1. **Install OpenJDK via Package Manager:**
   - Open a Terminal.
   - Run the following commands:
     ```bash
     sudo apt update
     sudo apt install default-jdk
     ```

2. **Set Environment Variables (optional):**
   - Open your shell profile (e.g., `~/.bashrc` or `~/.zshrc`).
   - Add the following lines:
     ```bash
     export JAVA_HOME=/usr/lib/jvm/default-java
     export PATH=$PATH:$JAVA_HOME/bin
     ```

3. **Verify Installation:**
   - Run:
     ```bash
     java -version
     javac -version
     ```

These instructions should help you set up the Java Development Kit (JDK) on Windows, macOS, and Linux. Adjust the paths and commands as needed for specific versions and system configurations.
