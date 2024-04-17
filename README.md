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
        per your requirements. You can access the Jenkins at the following url:
```bash
http://localhost:8080
```
        This is how the screen looks : 
        ![Alt text](/pythonProject1/img/jenkins_login_screen.png)

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
    The following command will authenticate you with your GitHub account.
    For this you will be asked a set of questions. Prefer to use the default
    values.
```bash
gh auth login

```
    The following command will Initialize the local directory as a Git repository. By default, the initial branch is called main.

```bash
git init -b main
```
   Add the files in your new local repository. This stages them for the first commit.

```bash
git add .
```

    Commit the files that you've staged in your local repository.
    (.venv) niladri@niladris-MacBook-Pro-2 pythonProject1 % gh repo create pythonProject1
    To get started with GitHub CLI, please run:  gh auth login
    Alternatively, populate the GH_TOKEN environment variable with a GitHub API authentication token.
    (.venv) niladri@niladris-MacBook-Pro-2 pythonProject1 % gh auth login
    ? What account do you want to log into? GitHub.com
    ? What is your preferred protocol for Git operations on this host? HTTPS
    ? Authenticate Git with your GitHub credentials? Yes
    ? How would you like to authenticate GitHub CLI? Login with a web browser
    
    ! First copy your one-time code: 7F0D-3F20
    Press Enter to open github.com in your browser... 
    ✓ Authentication complete.
    - gh config set -h github.com git_protocol https
    ✓ Configured git protocol
    ✓ Logged in as niladriforu
    (.venv) niladri@niladris-MacBook-Pro-2 pythonProject1 % 
    (.venv) niladri@niladris-MacBook-Pro-2 pythonProject1 % 

```bash
 git commit -m "First commit"
```

    In the Command prompt, add the URL for the remote repository where your local repository will be pushed.
```bash
git remote add origin remote repository URL
```

    In the Command prompt, push the changes in your local repository to GitHub.
```bash
git push -u origin main
```


