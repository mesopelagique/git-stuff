# Have a good readme!

## Format

As you must know readme could be written using markdown. Edit it on github or on your favorite markdown editor (such as visual studio code, etc...)

## Template

You can be inspired from this [template](https://gist.github.com/mesopelagique/4f9ca84088fbfcf7903ffb494e784a36) or any other project readme

Juste edit or visualize RAW version to see markdown and copy it.

## Readme content

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

If you look into the [provided template](https://gist.github.com/mesopelagique/4f9ca84088fbfcf7903ffb494e784a36) you could see under first header some "badges" ie. some images to show some summary information about your project

[![language-top][code-top]][code-url]

Github, Gitlab, Travis, etc.. provide some badge about Continous Integration (build, test, etc...) but a lot of badges come from https://shields.io/ website

You can show last released version, the language, the license and more.

### ex: show top language

For instance to show top language in your project you could show this image

https://img.shields.io/github/languages/top/YourName/YourProject.svg

using markdown
```markdown
![language-top](https://img.shields.io/github/languages/top/YourName/YourProject.svg)
```

### Reference links (link as variable, easier to copy paste and edit)

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


[code-top]: https://img.shields.io/github/languages/top/mesopelagique/CollectionUtils.svg
[code-url]: https://developer.4d.com/

## Big readme file

If your file contains a lot of lines, create a Table of Content using markdown links

For instance here [https://github.com/phimage/Prephirences#contents](https://github.com/phimage/Prephirences#contents)

