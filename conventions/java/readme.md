# Unnamed Team's Java Conventions

### Files and Folders

- Package names must only contain characters in the `[a-z]` range, package
names must be **singular** and have a single word *(for example: 'unnamedteam'
is bad, 'unnamed' is good)*.
- Classes, interfaces, enums, records and annotations names must be
**CamelCase**.
- Java files must have a license header.
- Tests must be in the same package as the class they test, but in a different
source folder (`test`).
- Tests names must be the same as the class they test, but with the `Test`
suffix.

### Build

- **Gradle over Maven:** Always prefer [Gradle](https://gradle.org/) over [Maven](https://maven.apache.org/).

### Structure

Java projects should have the following structure:

```
/<project-name>/
    |- /.github/                                  GitHub specific files (Optional)
         |- /workflows/
              |- build.yml
    |- /.idea/                                    IntelliJ IDEA specific files (Optional)
    |- /gradle/                                   Gradle files
         |- /wrapper/                             Gradle wrapper
              |- gradle-wrapper.jar               Gradle wrapper
              |- gradle-wrapper.properties        Gradle wrapper properties
    |- /docs/                                     Documentation (Optional)
    |- /<subproject-a>/                           Subproject A
    |- /<subproject-b>/                           Subproject B
    |- .editorconfig                              .editorconfig
    |- .gitignore                                 .gitignore
    |- gradle.properties                          Gradle properties (Should contain group, version and repositories)
    |- gradlew                                    Gradle wrapper script
    |- gradlew.bat                                Gradle wrapper script
    |- header.txt                                 License header
    |- license.txt                                License
    |- readme.md                                  Readme
    |- settings.gradle.kts                        Gradle settings
```
