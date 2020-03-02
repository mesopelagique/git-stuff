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

As you must know readme could be written using markdown.

You can be inspired from this template or any other project readme
https://gist.github.com/mesopelagique/4f9ca84088fbfcf7903ffb494e784a36

You must provide information about your project.
- how to use it (Getting Started, Usage)
- how to install/integrate/deploy it

You could add
- information about license, acknowledgments, authors
- how to contribute to your project (a link to a file CONTRIBUTING.md )

### Link to others documentations files

Maybe you create documentation for each public methods or class in Documentation folder

To be able to reach it easily, provide links in your README to some of them using markdown link

```markdown
[MyMethod](Documentation/Methods/MyMethod.md)
[MyClass](Documentation/Classes/MyClass.md)
```

### Badges

If look into the [provided template](https://gist.github.com/mesopelagique/4f9ca84088fbfcf7903ffb494e784a36) you could see under first header some "badges" ie. some images to show some summary information about your project

[![language-top][code-top]][code-url]

Github, Gitlab, Travis, etc.. provide some badge about Continous Integration (build, test, etc...) but a lot of badges come from https://shields.io/ website

### show top language

For instance to show top language in your project you could show this image

https://img.shields.io/github/languages/top/YourName/YourProject.svg

using markdown
```markdown
![language-top](https://img.shields.io/github/languages/top/YourName/YourProject.svg)
```

### Reference links

It allow to create variables in markdown for images & links

[https://www.markdownguide.org/basic-syntax/#reference-style-links](https://www.markdownguide.org/basic-syntax/#reference-style-links)

To display top language you could do like that

```markdown
[![language-top][code-top]][code-url]
```

and add at markdown bottom your links
```markdown
[code-top]: https://img.shields.io/github/languages/top/YourName/YourProject.svg
[code-url]: https://developer.4d.com/
```

You can copy all badges [from templates](https://gist.githubusercontent.com/mesopelagique/4f9ca84088fbfcf7903ffb494e784a36/raw/5e426af569daff9249fce2dabd01e33654ac11a0/README-Template.md)
and change the owner and project name

## Create a github pages

[GitHub Pages](GitHubPages.md)

## Release version

[Release](Release.md)

[code-top]: https://img.shields.io/github/languages/top/mesopelagique/CollectionUtils.svg
[code-url]: https://developer.4d.com/

