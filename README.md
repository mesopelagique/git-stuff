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

# github

## Have a good readme

As you must know readme could be written using markdown

You can be inspired from this template or any other project readme
https://gist.github.com/mesopelagique/4f9ca84088fbfcf7903ffb494e784a36

### Link to other documentation

Maybe you create documentation for each public methods in Documentation folder

To be able to reach it easily, provide in your README links to some of them using markdown link

```markdown
[MyMethod](Documents/MyMethod.md)
```

## Create a github pages

For instance https://mesopelagique.github.io/formula_compose/

Go to Settings, go down to Github Pages section and choose to active github pages.

You can choose the root, and your README will be the first page. (If you not want you could also select docs/)

The link to your github page will be written but if not the link is https://user.github.io/repo

#### Customize

You can choose a theme just in the same section where you activate the page.

The theme will be used at next site generation (you can edit readme to force publish a new website)

#### Provide the link in page description

Copy the page link and edit project description. Here at the right you can paste the link and save.

## Release version

Maybe you already know git tag. Tag allow to have a time point in your git comit history. You could create a tag with a version number (following SemVer)

Releases throught github help people to know about new stuff in your project and they are associated to a tag.
Someone that follow your project could register to notification and even receive mail with your release description.

Go to https://www.github.com/YourUserName/YourProject/releases

### Provide binary

You could attach binary to a release ie. You can attach a 4dz file or any thing you want.
Providing binaries help to integrate your component quickly (Do not forget to describe in readme how to install it)

Edit you release and drag and drop the file

You can provide a link to latest release by removing release name/version and add latest before "download" in download link

