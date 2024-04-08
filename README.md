# Setup


```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```
```bash
brew install jenkins-lts
```

Install the latest LTS version: 
```bash
brew install jenkins-lts
```
Start the Jenkins service: 
```bash
brew services start jenkins-lts
```

        The Jenkinse service got started. Once done, it is going to ask you
        to unlock the Jenkins. You can find the password in the following
        location:
```bash
cat /Users/username/.jenkins/secrets/initialAdminPassword
```
        Now you are the adminuser. You can create multiple users and assign 
        roles to them. You can also install plugins and configure Jenkins as
        per your requirements.

# Restart and other useful commands
Restart the Jenkins service: 
```bash
brew services restart jenkins-lts
```
Update the Jenkins version: 
```bash
brew upgrade jenkins-lts
```
Uninstall Jenkins: 
```bash
brew uninstall jenkins-lts
```
```bash
This is to install the GitHub CLI. This is a command-line tool that brings GitHub to your terminal.
```
```bash
brew install gh
```