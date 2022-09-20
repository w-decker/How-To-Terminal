# How-To

This is a private repository that stores instructions, notes and code on how to use GitHub using mac terminal.

# Git and Terminal

1. Install Homebrew using the code below

```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

2. Install git via brew

```
brew install git
```

# Cloning repositories directly onto computer

1. Click on repository you wish to clone.
2. Click on the green 'code' button
3. Click the https code
4. Use the following code to clone repository to computer

```
git clone https://github.com/w-decker/repository_name.git
```

# Making sure you're up to date with the repository

```
git checkout main
```

```
get fetch upstream
```

```
git merge upstream/main
```

```
git push origin main
```

# Pushing files to personal repositories

1. Add file into personal repository on computer
2. Use the following code to add all new files to repository.

```
git add -A
```

```
git commit -m "write message here"
```

```
git push origin branch_name
```

# Forking and using repositorys from another user

1. Fork the repo that you wish to work on
2. ``` cd``` into the directory in which you wish to store repo
3. clone the repo into desired location(using the same instructions stated earlier regarding cloning)
4. Use the following code to update the repo now located on your computer

```
cd ./repo_name
```

```
git remote add upstream https://github.com/repo_owner/repo_name.git
```

```
git remote set-url --push upstream Oops.no.push.to.upstream
```

```
git remote -v
```

You will see the following code in the output

```
origin https://github.com/yourname/repo_name.git (fetch)
origin https://github.com/yourname/repo_name.git (push)
upstream https://github.com/repo_owner/repo_name.git (fetch)
upstream	Oops.no.push.to.upstream (push)
```


# Removing .DS_Store files created by MACs

Use the following code to remove .DS_Store files created by macs

```
echo .DS_Store >> ~/.gitignore_global

git config --global core.excludesfile ~/.gitignore_global
```

# PAT

To connect Git to Github you have to provide authentication. It will ask for a username and then password, but no longer accepts these credentials. To create a PAT follow these instructions: https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token

When logging in, enter your username and PAT for the password.



