# splunk-seed-app

## What is it?
splunk-seed-app is a seed for a [Splunk](http://splunk.com/) application.  The idea is you should clone this repository, delete the .git directory and rename the directory.  You then have the basics of an application.

## Directory layout

    splunk-seed-app
    |--source                     # source directory: Gets bundled as a tgz into target
    |  |--appserver
    |  |  \--static
    |  |--bin
    |  |--default
    |  |  \--data
    |  |     \--views
    |  |        \--nav
    |  \--meta
    |--target                     # output directory (ignored)
    \--tests                      # test: any tests go here

## Installation

```PowerShell
git clone https://github.com/oxo42/splunk-seed-app.git my-app
cd my-app
rm -Recurse -Force .git
git init
git add -A
git commit -m "Initial Import"
```

## Build

I haven't decided on the build system yet.  The options are:
* [Gradle](http://gradle.org/)
* [Maven](https://maven.apache.org/)
* [PyBuilder](http://pybuilder.github.io/)
* [Python Setuptools](https://pythonhosted.org/setuptools/)
