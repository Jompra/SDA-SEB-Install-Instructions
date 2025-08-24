# Mac Software Install

## Step 1 Install Homebrew

1. Open Terminal.
2. (If prompted) install Apple’s Command Line Tools:

```bash
xcode-select --install
```

This might take a while depending on your OS and internet connection. If it takes more than 10 seconds, go and make a cup of tea then come back to make sure it works ok.

3. Install Homebrew

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

4. Add Brew to your PATH:

If you have Apple Silicon (M1/M2/M3) use the following commands:

  ```bash
  echo 'eval "$(/opt/homebrew/bin/brew shellenv)"' >> ~/.zprofile
  eval "$(/opt/homebrew/bin/brew shellenv)"
  ```

If you have an Intel Mac use the following commands:

  ```bash
  echo 'eval "$(/usr/local/bin/brew shellenv)"' >> ~/.zprofile
  eval "$(/usr/local/bin/brew shellenv)"
  ```

5. Verify:

```bash
brew --version
```

## Step 2 Install Python

1. Install:

Run the following commands in terminal one at a time:

```bash
brew update
brew install python
```

2. Verify:

```bash
python3 --version
pip3 --version
which python3
```

## Step 3 Install PostgreSQL

1. Install and start, run these one at a time:

```bash
brew install postgresql@17
brew services start postgresql@17
```

2. Verify server & client, run these one at a time:

```bash
psql -d postgres -c "SELECT version();"
psql --version
```

## Step 4 Install Node.js

Run the following commands:

```bash
brew install node
node --version
npm --version
```

This installs Node and npm in one go.

If you hit anything weird, `brew doctor` is your quick health check.


### Step 5 Check you are complete

| Step | Software / Platform | Completed |
|------|---------------------|-----------|
|1     | Homebrew            | - [] Done |
|2     | Python              | - [] Done |
|3     | PostgreSQL          | - [] Done |
|4     | Node.js             | - [] Done |
|5     | Check complete      | - [] Done |

If you have completed all 5 steps, let your instructors know and start on your pre reading. Well done! 👏 🥳.
