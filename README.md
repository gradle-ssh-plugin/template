Gradle SSH Plugin Template [![Build Status](https://travis-ci.org/gradle-ssh-plugin/template.svg?branch=master)](https://travis-ci.org/gradle-ssh-plugin/template) [![Gradle Status](https://gradleupdate.appspot.com/gradle-ssh-plugin/template/status.svg)](https://gradleupdate.appspot.com/gradle-ssh-plugin/template/status)
==========================

A template project with [Gradle SSH Plugin](https://github.com/int128/gradle-ssh-plugin).


Prerequisite
------------

Java 6 or later.


Try it now
----------

Clone the repository.

```bash
git clone https://github.com/gradle-ssh-plugin/template.git
cd template
```

Edit `build.gradle` and run Gradle.

```bash
./gradlew showPlatformVersion
```

We can dry run the script as follows:

```bash
./gradlew -PdryRun -i showPlatformVersion
```
