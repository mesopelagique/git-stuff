# git-stuff

Have you a project ready for prime time? Want to share it to the community

First of all, one git project by 4d project/component

I recommand to use a software like sourcetree https://www.sourcetreeapp.com

If you already know how to use git, and want to know just how to present your project on github go to [github section](#github)


## Create a git project

### using command line

Using a terminal go to your project root and type

```
git init .
```

This will create a .git folder (so if there is alread a .git folder, nothing to do)

### using a soft like sourcetree (recommanded)

Just drag and drop the project folder to sourcetree. It will ask you to create a github project

## Create the github project

Log into github, Click the Plus button near the avatar (top right) and choose new repository

Choose a relevant name and validate.

Github will provide a list of command line to use. Keep the page open.

## Link your local git project to github project

### Using command line

Again go to your project root using a terminal and type.
You could see this command line on github page

```
$ git remote add origin https://github.com/user/repo.git
```
https://help.github.com/en/github/using-git/adding-a-remote

to know if alread attached to a remote you can type 

```
$ git remote -v 
```

### Using sourcetree

Go to project setting, choose remote tab, add a new remote
choose name origin (or github) and paste the remote url (the github url with .git)

https://confluence.atlassian.com/sourcetreekb/changing-remote-repository-path-on-sourcetree-using-git-or-mercurial-785616227.html

## Push your project

It's time to push your local code to github

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
git commit -c "Initial commit" 
```

#### using sourcetree

https://fr.coursera.org/lecture/version-control-with-git/command-line-commit-to-a-local-repository-zBlSu

### push

#### using command line 

```
git push origin
```

#### using sourcetree

press push button
when commiting you can also check the box : "push change immediatly to", and make commit push one operation

# Github

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
