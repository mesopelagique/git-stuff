# git-stuff

Have you a project ready for prime time? Want to share it to the community

## Create a git project

### using command line

### using a soft like sourcetree (recommanded)


## Create the github project

## Link your local git project to github project

### Using command line

### Using sourcetree


## Push your project

It's time to push your local code to github

First your file must be commited

Do not push DerivedData, and userPreferences
Use .gitignore mecanisum

On sourcetree right click on file, choose to ignore a file, and select the rules according yo your need

# github

## Have a good readme

As you must know readme could be written using markdown

You can be inspired from this template or any
https://gist.github.com/mesopelagique/4f9ca84088fbfcf7903ffb494e784a36

### Link to other documentation

Maybe you create documentation for each public method in Documentation folder

To be able to reach it easily, provide in your README links to some of them using markdown link

MyMethod(Documents/MyMethod.md)

## Create a github pages

Go to settings, general, and choose to active github pages.
The link to your github page will be written. (yourname.gitpage.io/yourproject)

You can choose the root, and your README will be the first page. (If you not want you could 

#### Customize

You can choose a theme just near where you activate the page.

The theme will be used at next site generation (you can edit readme to force publish a new website)

#### Provide the link

Then you copy the page link and edit project description. Here at the right you can paste the link and save.

## Release version

Maybe you already know git tag. Tag allow to have a time point in your git comit history. You could create a tag with a version number (following SemVer)

Releases throught github help people to know about new stuff in your project and they are associated to a tag.
Someone that follow your project could register to notification and even receive mail with your release description.

Go to https://www.github.com/YourUserName/YourProject/releases

### Provide binary

You could attach binary to a release ie. You can attach a 4dz file or any thing you want.
Providing binaries help to integrate your component quickly (Do not forget to describe in readme how to install it)
