# Windows Installations

## Step 1 Install Git & Git Bash on Windows

### 1.1 Check your Windows version

If you are using windows 7 please inform your instructors and then skip to **Step 2 Install Node.js**

### 1.2 Download Git for Windows

Go to the official download page and grab the current x64 installer. As of **Aug 24, 2025**, the latest is **2.51.0** (released **Aug 19, 2025**).

### 1.3 Run the installer

When the Setup wizard opens, you can safely accept defaults unless you prefer the alternatives noted below.

### 1.4 Open Git Bash

Start → search **“Git Bash”** → open it. Git bash will allow you to use all of the same commands that we use in class regardless of if you're on Windows, or Mac.

### 1.5 Verify the installation

In **Git Bash** type in the following command **exactly** as shown below:

```bash
git --version
```

You should see something like `git version 2.51.0.windows.x`. Don't worry about the specific numbers.

### 1.6 Identify yourself for commits

type the following commands one at a time into git bash **Be extremely careful and type it exactly as you see here:

Change `Your Name` and `you@example.com` to your name and email address. Use the same email address that you used to sign up to github and github enterprise.

```bash
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
```

For example if i were to complete this I would put:

```bash
git config --global user.name "George Jones"
git config --global user.email "george.jones@generalassemb.ly"
```

### 1.7 CHange your default branch to main

Your default branch will probably be called `master` we no longer use this terminology so we need to use the following command.

```bash
git config --global init.defaultBranch main
```

## Step 2 Install Node.js

Node.js is what we will use to run javascript on our computer

### 2.1 Download the LTS installer

Go to [https://nodejs.org/en/download/][1]

Scroll down, ensure that the options look like this and click `Windows Installer (.msi)`

![Windows installer node](./images/Screenshot%202025-08-24%20at%2016.01.43.png)

### 2.2 Run the installer

Double-click the downloaded `.msi` file, accept the license, keep the defaults, and finish. This installs **Node.js** and **npm** and adds them to your PATH.

### 2.3 Verify the install

Open a **new** Git Bash and run:

```bash
node --version
npm --version
```

You should see version numbers for both.

If you seesomething like `command not found` contact your instructors.

## Step 3 Install Python

### 3.1 Download the installer**

Go to the official [Python downloads page][2] and grab the latest **Python 3.x Windows installer (64-bit)**. The latest release is highlighted at the top.

### 3.2 **Run the installer**

* Double-click the `.exe` installer.
* **Important**: On the first screen, **check the box** that says **“Add Python 3.x to PATH”**.
* Click **Install Now** (the follwing defaults are fine).

### 3.3 **Verify the install**

Open a new git bash and run:

```bash
python --version
pip --version
```

You should see a Python 3.x version and a pip version.

## Step 4 Install PostgreSQL on Windows

### 4.1 Download the installer

Go to the official [PostgreSQL Windows downloads page][3].

Choose the latest stable version Windows x86-64. 17.6

### 4.2 Run the installer

Double-click the `.exe` you downloaded.
*Step through the wizard (defaults are fine):

**Installation directory** → leave default
**Components** → keep PostgreSQL Server, pgAdmin, Command Line Tools
**Password** → set a strong but memorable password for the default `postgres` user (make a note of it. No really, don't forget it!)
**Port** → default is 5432 (DO Not Change This!)
Click **Next** until installation starts.

### 4.3 Verify the install

   Open **Git Bash** and run:

```bash
psql --version
```

You should see something like `psql (PostgreSQL) 17.x`.

### Step 5 Check you are complete

| Step | Software / Platform | Completed |
|------|---------------------|-----------|
|1     | Git and Gitbash     | - [] Done |
|2     | Node.js             | - [] Done |
|3     | Python              | - [] Done |
|4     | PostgreSQL          | - [] Done |
|5     | Check complete      | - [] Done |

If you have completed all 5 steps, let your instructors know and start on your pre reading. Well done! 👏 🥳.

[1]: https://nodejs.org/en/download/
[2]: https://www.python.org/downloads/windows/
[3]: https://www.enterprisedb.com/downloads/postgres-postgresql-downloads
