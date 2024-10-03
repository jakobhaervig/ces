# Conference for Energy Students (CES) at Aalborg University

This site is based on the [jekyll-theme-conference](https://github.com/DigitaleGesellschaft/jekyll-theme-conference) template. At this link you may find much more in-depth information about how to modify and update it.

## Notes to self for working locally with the website

### Step 1: Install Windows for Linux (WSL)
- First, follow the [official guide](https://learn.microsoft.com/en-gb/windows/wsl/install) to install WSL.
- Go to Microsoft Store and install Ubuntu.
- Open the Ubuntu App and go through the installation process, e.g. choose WSL Ubuntu username and password.

### Step 2: Install Visual Studio Code (VS Code)
- Download and install [VS Code](https://code.visualstudio.com/).

### Step 3: Install a git mangemenent software
- Install your preferred git management software such as [GitHub Desktop](https://desktop.github.com/download/) or [GitKraken](https://www.gitkraken.com/).

### Step 4: Setting up and installing prerequisites
- Open your git management software and clone https://github.com/jakobhaervig/ces.
- Open VS Code and open the *ces* folder you just cloned.
- Open a WSL terminal.

### Step 5:
Copy/paste the following commands one-by-one into the WSL terminal to install prerequisite:
```
sudo apt-get install ruby-full build-essential zlib1g-dev
```

Change default home for gems:
```
echo '# Install Ruby Gems to ~/gems' >> ~/.bashrc
echo 'export GEM_HOME="$HOME/gems"' >> ~/.bashrc
echo 'export PATH="$HOME/gems/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc
```

Install Jekyll and bundler:
```
gem install jekyll bundler
```

Install git lfs support:
```
sudo apt install git-lfs
git lfs install
```

Serve website locally:
```
bundle exec jekyll serve
```

, which will serve the website locally. Navigate to [http://127.0.0.1:4000/](http://127.0.0.1:4000/) to view the website.