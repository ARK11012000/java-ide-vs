
# Java IDE Pack

In pursuit of the best Java tooling in VS Code.

As of Feb 2018 VS Code has become more than editor. 
For Java it has debug, JUnit support.
The developmnet is lead by (developers of) companies: Red Hat, Microsoft, Pivotal. And there are many diverse extentions available for other languages and general in nature. 

This extention pack is to help to bootstrap VS Code for Java development. Comment via issues on GitHub,
but note that feature contribution is done by particular extention listed below and you should use respective resource to learn and give (issues, changes).  All GitHub links are given below.

The pack is to give compatible set, of extensions that complement each other. Requirements are those that satisfy all extensions.

### Requirements

- VS Code 1.19+
- JDK 8. `java`, `javac` on path
- Maven, `mvn` on path

## Install

Open VS Code Extension view (press `Ctrl + Shift + X`), type `java-ide-pack`.

Or launch VS Code Quick Open (`Ctrl + P`), paste the following command, and press enter.
```bash
ext install java-ide-pack
```

### Included

See `extensionDependencies` section in `package.json`:

    "extensionDependencies": [ 
        "redhat.java",
        "vscjava.vscode-maven",
        "vscjava.vscode-java-debug",
        "vscjava.vscode-java-test",
        "vscjava.vscode-spring-initializr"
        "Pivotal.vscode-boot-java", 
        "Pivotal.vscode-boot-properties",
        "ithildir.java-properties",
        "dgileadi.java-decompiler", 
        "robertohuertasm.vscode-icons"
    ]

List as `displayName`, `publisher`.`name` (aka Unique Identifier), GitHub URL
[, "description", notes]:

- Java Language Support `redhat.java`  
https://github.com/redhat-developer/vscode-java
- Maven Project Explorer `vscjava.vscode-maven`  
https://github.com/Microsoft/vscode-maven
- Debugger for Java `vscjava.vscode-java-debug`  
https://github.com/Microsoft/vscode-java-debug
- Java Test Runner `vscjava.vscode-java-test`  
https://github.com/Microsoft/vscode-java-test
- Spring Initializr Java Support `vscjava.vscode-spring-initializr`  
https://github.com/Microsoft/vscode-spring-initializr

- Spring Boot Java Support `Pivotal.vscode-boot-java`  
https://github.com/spring-projects/sts4/tree/master/vscode-extensions
- Spring Boot Application Properties Support `Pivotal.vscode-boot-properties`  
https://github.com/spring-projects/sts4/tree/master/vscode-extensions
- Java Properties `ithildir.java-properties`  
https://github.com/ithildir/vscode-java-properties
"A port of the TextMate Java Properties (`.properties`) syntax highlighting for Visual Studio Code."
- Java Decompiler `dgileadi.java-decompiler`  
https://github.com/dgileadi/vscode-java-decompiler
- vscode-icons `robertohuertasm.vscode-icons`  
https://github.com/vscode-icons/vscode-icons

### Not included

- SonarLint `SonarSource.sonarlint-vscode`    
SonarLint does not yet have [support for Java
#13](https://github.com/SonarSource/sonarlint-vscode/pull/13)
- jsh
`joshuansu.jshell`  
https://github.com/joshuansu0897/Extension-Jshell-Code
Java 9+ Shell (JShell) support
- Java Language Support
`georgewfraser.vscode-javac`  
https://github.com/georgewfraser/vscode-javac
"Java support using the Java Compiler API" is alternative to using language server
- Java Debug
`DSnake.java-debug`  
https://github.com/go-bin/vscode-java-debug
(Last commit Jan 2017)
- Java Snippets
`tushortz.java-snippets`  
https://github.com/tushortz/vscode-Java-Snippets
Only one release, all completions are in one 10MB `java_complete.json`
- Java Imports Snippets
`tushortz.java-imports-snippets`  
https://github.com/tushortz/vscode-Java-Imports
Only one release. Entering import starts with typing `_`
- Java Linter
`faustinoaq.javac-linter`  
https://github.com/faustinoaq/vscode-javac-linter
"A simple Java linter for Visual Studio Code using the the language server protocol."
- Spring Boot Support `ecmel.vscode-spring-boot`  
https://github.com/ecmel/vscode-spring-boot
- Java Server Pages (JSP) `pthorsson.vscode-jsp`  
Let template engine support stay optional.

## Feedback

- [GitHub issues](https://github.com/paulvi/vscode-java-ide-pack/issues)

## Developing

- https://github.com/paulvi/vscode-java-ide-pack

### Links and docs

- https://code.visualstudio.com/docs/extensions/publish-extension
