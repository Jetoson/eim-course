# eim-course

## Github config
## 1. ⚙️ Initial Setup: Git and GitHub

Before starting, ensure you have **Git** installed on your Windows machine and configured. Also, make sure you have an account on **GitHub**.

### 1.1 Create the Repository on GitHub

1.  Go to **GitHub** and log in.
2.  Click the **'+'** icon in the top right corner and select **'New repository'**.
3.  For **Repository name**, enter your desired name, e.g., **"x"**.
4.  Optionally, provide a **Description**.
5.  Choose whether you want the repository to be **Public** or **Private**.
6.  Crucially, check the boxes to **'Add a README file'**, **'Add .gitignore'** (select **Android** from the template dropdown), and **'Choose a license'**.
7.  Click **'Create repository'**.


## 2. 💻 Project Creation and Cloning in Android Studio

Now, you'll use Android Studio to create a local project and link it to the remote GitHub repository.

### 2.1 Clone the Remote Repository

Instead of creating a new project locally first, it's easier to **clone** the existing GitHub repo ("x") into your desired workspace. This downloads the README, .gitignore, and License files.

1.  Open **Android Studio**.
2.  On the welcome screen, select **'Get from VCS'**.
3.  In the dialog box:
    * Select **'Git'** as the Version Control.
    * Enter the **URL** of your new GitHub repository "x" (you can copy this from the green **'Code'** button on your GitHub repo page).
    * Choose the **Directory** where you want to store the project on your Windows computer.
4.  Click **'Clone'**.

### 2.2 Create an Android Studio Project within the Cloned Directory

Since you just cloned an empty-ish folder, you now need to create your actual Android project *inside* that folder.

1.  In Android Studio, go to **File > New > New Project**.
2.  Select your desired **Template** (e.g., **'Empty Views Activity'**).
3.  In the **New Project** dialog:
    * For **Name**, use the same name as your repo, **"x"**.
    * For **Save location**, **browse to and select the *cloned folder*** named "x" you created in the previous step. **This is critical**—it ensures your project files are within the existing Git repository.
    * Configure the remaining options (Package name, Language, Minimum SDK) as needed.
4.  Click **'Finish'**.

Android Studio will now create the entire project structure inside the folder that is already a Git repository, automatically adding the new project files (like `app`, `gradle`, etc.) for tracking.

---

## 3. 🚀 Pushing Changes to GitHub

Your project files are now created locally within the repository. The final step is to commit these new files and push them up to GitHub.

### 3.1 Commit the New Project Files

1.  In Android Studio, go to **Git > Commit...** (or press $Ctrl + K$).
2.  In the **Commit** window, you will see a list of all the new files that are **untracked** (your entire Android project structure).
3.  Enter a descriptive **Commit Message** (e.g., "**Initial commit of project structure**").
4.  Click **'Commit'**.



### 3.2 Push the Changes to the Remote Repo

1.  Go to **Git > Push...** (or press $Ctrl + Shift + K$).
2.  Verify the details (it should show your local branch and the remote branch).
3.  Click **'Push'**.

Your entire Android Studio project, including all its files and folders, will now be uploaded and visible on your remote GitHub repository "x".
