# How-To

This is a private repository that stores instructions, notes and code surrounding how to use GitHub using mac terminal.

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


