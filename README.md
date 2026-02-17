[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/MUEW8x3O)
# ITCS333: Internet Software Development - GitHub Tutorial

This tutorial outlines the necessary steps to set up your development environment and submit your first task using GitHub and Visual Studio Code.

## Version Control

### What is Version Control?
Version Control (VC) is a system that records changes to a file or set of files over time so that you can recall specific versions later. It allows multiple people to work on a single project simultaneously without overwriting each other's changes.
* [Wikipedia: Version Control](https://en.wikipedia.org/wiki/Version_control)

### What is Git?
Git is a free and open-source distributed version control system designed to handle everything from small to very large projects with speed and efficiency. It is the tool running locally on your machine that tracks the history of your code.
* [Wikipedia: Git](https://en.wikipedia.org/wiki/Git)
* [Official Website: Git](https://git-scm.com/)

### What is GitHub?
GitHub is a developer platform that allows developers to create, store, manage, and share their code. It provides a web-based hosting service for Git repositories, adding features like access control, bug tracking, software feature requests, task management, and continuous integration.
* [Wikipedia: GitHub](https://en.wikipedia.org/wiki/GitHub)
* [Official Website: GitHub](https://github.com/)

### Why We Use Them
* **Collaboration:** Multiple developers can work on the same codebase simultaneously.
* **History and Backup:** Every change is tracked. You can revert to previous versions if a bug is introduced.
* **Branching:** You can work on new features in isolated environments (branches) without affecting the main code.

---

## Task 1: Create a GitHub Account

1.  **Navigate to GitHub:** Open your web browser and go to [https://github.com/](https://github.com/).
2.  **Initiate Sign Up:** Click the "Sign up" button located in the top-right corner of the page.
3.  **Enter Credentials:** Follow the prompts to enter your email address, create a strong password, and select a unique username.
    * **Note:** Select a professional username, as you may use this profile for job applications in the future.
4.  **Verify Account:** Complete the CAPTCHA puzzle and enter the launch code sent to your email address to verify your account.
5.  **Complete Setup:** You may complete the personalization questions or skip them to access your main dashboard.

---

## Task 2: Download and Install Git

### Windows
1.  **Download:** Navigate to the official Git website at [https://git-scm.com/download/win](https://git-scm.com/download/win). The download should start automatically.
2.  **Run Installer:** Open the downloaded `.exe` file.
3.  **Installation:** Follow the installation wizard.
    * **Note:** You can safely accept the default settings for all steps. Ensure "Git Bash" is selected if you prefer a Unix-style command line.

### macOS
Git is often pre-installed on macOS.
1.  **Check Installation:** Open the Terminal and type `git --version`.
2.  **Install (if missing):** If Git is not installed, the system will prompt you to install the Xcode Command Line Tools. Follow the on-screen instructions.
3.  **Alternative:** You may also use the installer from [https://git-scm.com/download/mac](https://git-scm.com/download/mac).

### Linux
Git is usually pre-installed on most Linux distributions.
1.  **Check Installation:** Open your terminal and type `git --version`.
2.  **Install (if missing):** Use your distribution's package manager.
    * **Debian/Ubuntu:** `sudo apt-get install git`
    * **Fedora:** `sudo dnf install git`

### Verification
After installation is complete, verify it by opening your command prompt (Terminal or PowerShell) and running:
```bash
git --version

```

You should see the installed version number as output.

---

## Task 3: Download and Install VS Code

1. **Download:** Navigate to the official Visual Studio Code website at [https://code.visualstudio.com/](https://code.visualstudio.com/).
2. **Install:** Download the installer for your operating system (Windows, macOS, or Linux) and follow the installation wizard.
* **Note:** During installation, ensure the "Add to PATH" option is checked.



### Verify Git Installation in VS Code

1. Open Visual Studio Code.
2. Open the Integrated Terminal by pressing `Ctrl + ~` (tilde) or selecting **Terminal > New Terminal** from the menu.
3. Type the following command and press Enter:
```bash
git --version

```


4. If installed correctly, the terminal will display the Git version.

### Configure Git

Configure your global Git settings to associate your commits with your identity. Run the following commands in the VS Code terminal, replacing the text in quotes with your actual information:

```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"

```

---

## Task 4: Clone this repository Using VS Code

1. **Copy Repository URL:** On the main page of this GitHub repository, click the green **Code** button and copy the HTTPS URL.
2. **Open VS Code:** Launch Visual Studio Code.
3. **Open Command Palette:** Press `Ctrl + Shift + P` (Windows/Linux) or `Cmd + Shift + P` (macOS).
4. **Run Clone Command:** Type `Git: Clone` and press **Enter**.
5. **Paste URL:** Paste the repository URL you copied in Step 1 and press **Enter**.
6. **Select Location:** Choose a folder on your local machine where you want to save the project.
7. **Open Repository:** Once the cloning process finishes, a notification will appear in the bottom-right corner. Click **Open** to load the repository in VS Code.

Refer to this video:

[![Clone Repos from VS Code](https://img.youtube.com/vi/bz1KauFlbQI/0.jpg)](https://www.youtube.com/watch?v=bz1KauFlbQI)

---

## Task 5: Modify the file studentinfo.txt

1. **Locate File:** In the VS Code **Explorer** pane (left side), locate the file named `studentinfo.txt`.
2. **Edit File:** Click the file to open it.
3. **Enter Details:** Fill in your specific details next to the provided labels.

**Example Content:**

```text
Name: Abdulla Ebrahim
UOB ID: 20001000
GitHub Username: aebrahim

```

---

## Task 6: Commit and Push using VS Code

1. **Open Source Control:** Click the **Source Control** icon in the left sidebar (or press `Ctrl + Shift + G`).
2. **Stage Changes:** You will see `studentinfo.txt` listed under **Changes**. Hover over the file name and click the **+ (Plus)** icon to stage the changes.
3. **Commit Message:** In the text box labeled "Message", type a descriptive message (e.g., "Updated student information").
4. **Commit:** Click the **Commit** button (or press `Ctrl + Enter`).
5. **Push Changes:** Click the **Sync Changes** button (or **Push**) to upload your commit to the remote GitHub repository.
