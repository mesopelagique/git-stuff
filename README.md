# git-stuff

Have you a project ready for prime time? Want to share it to the community

First of all, one git project by 4d project/component

I recommand to use a software like sourcetree https://www.sourcetreeapp.com

If you already know how to use git, and want to know just how to present your project on github go to [github section](#github)

## Create a git project

### using command line

On mac and linux sing a terminal go to your 4d project root folder and write

```
git init .
```

This will create a .git folder (so if there is alread a .git folder, nothing to do)

### using a soft like sourcetree (recommanded)

Just drag and drop the project folder to sourcetree. It will ask you to create a github project.

## Commit your project

First of all your files must be commited.

### select the files to commit

Using command line to add all
```
$ git add .
```

On sourcetree just select it

#### Ignore some files

Do not push DerivedData, and userPreferences
Use .gitignore mecanism

On sourcetree right click on file, choose to ignore a file, and select the rules according yo your need

or manually create a .gitignore files in project root, or edit the global file
or use command line

https://www.atlassian.com/git/tutorials/saving-changes/gitignore

### commit

#### command line

provide a commit message and its done

```
git commit -c "Initial commit message" 
```

#### using sourcetree

https://fr.coursera.org/lecture/version-control-with-git/command-line-commit-to-a-local-repository-zBlSu

# Github

## Create the github project

Log into your github account or create one

Click the Plus button near the avatar (top right) and choose new repository. (or click [here](https://github.com/new))

Choose a relevant name and validate.

Github will provide a list of command lines to use. Keep the page open it could help later.

### Create or not the README.md file?

If you have already a project on your disk, keep empty the remote project. You will push a readme file by yourself or create one online after first push.

# Link Git and GitHub

## Link your local git project to github project

### Using command line

Again go to your project root using a terminal and type.
You could see this command line on github page and we will use it

```
$ git remote add origin https://github.com/user/repo.git
```
https://help.github.com/en/github/using-git/adding-a-remote

ps: origin is just a shortcut name for the remote url you use. You could do `git remote add github https://...` if you want. But remember this shortcut name for later to push files for instance

#### already attached?

to know if your project is already attached to a remote git server you can type 

```
$ git remote -v 
```

You could be attached to multiple remote server

```
$ git remote -v
github	https://mesopelagique@github.com/4d-for-ios/4D-Mobile-App-Server.git (fetch)
github	https://mesopelagique@github.com/4d-for-ios/4D-Mobile-App-Server.git (push)
gitlab	https://gitlab.4d.fr/qmobile/4d-mobile-app-server.git (fetch)
gitlab	https://gitlab.4d.fr/qmobile/4d-mobile-app-server.git (push)
```

### Using sourcetree

Go to project setting, choose remote tab, add a new remote
choose name origin (or github) and paste the remote url (the github url with .git)

https://confluence.atlassian.com/sourcetreekb/changing-remote-repository-path-on-sourcetree-using-git-or-mercurial-785616227.html

## push your files on github

If you have commited already locally your files

### using command line 

```
git push origin
```

### using sourcetree

Just press push button

when commiting you can also check the box : "push change immediatly to", and make commit push one operation

## Have a good readme!

It is very important to have a good readme. It is your landing page for your project.
You will find on following link good pratices of writing such a file - with a few examples, and a ready to use template.

[Good Readme](GoodReadme.md)

## Create a github pages

Generate a website for your project easily.

[GitHub Pages](GitHubPages.md)

## Release version

Notify followers about new stuff and bug fixes. Provide binaries.

[Release](Release.md)
