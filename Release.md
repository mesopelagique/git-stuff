# Release

Maybe you already know [git tag](https://git-scm.com/book/en/v2/Git-Basics-Tagging) to tag a specic commit in your history.

Typically, people use this functionality to mark release points. There is no release concept in git but in github you can assocciate a github release to a git tag.

Create a git tag with a version number like 0.0.1 (following [SemVer](https://semver.org/) rules)

Releases throught github help people to know about new stuff in your project.
- Someone that follow your project could register to notification and even receive mail with your release description.

Go to https://www.github.com/YourUserName/YourProject/releases to see [your release and create new one](https://help.github.com/en/github/administering-a-repository/managing-releases-in-a-repository)


Create the release and choose your tag. Add description (the change, the bug fix, etc...)

### Provide binary

You could attach binary to a release ie. You can attach a 4dz or a zip file, or any thing you want.

Providing binaries help to integrate your component quickly (Do not forget to describe in readme how to install it)

Edit you release and drag and drop the file.

You can provide a link to latest release :
- https://github.com/YourUserName/YourProject/releases/latest/download/YourProject.4DZ 

and add it to your install instruction.
- https://github.com/mesopelagique/CollectionUtils#installing


## Links

- [https://help.github.com/en/github/administering-a-repository/about-releases](https://help.github.com/en/github/administering-a-repository/about-releases)
- [https://help.github.com/en/github/administering-a-repository/managing-releases-in-a-repository](https://help.github.com/en/github/administering-a-repository/managing-releases-in-a-repository)
