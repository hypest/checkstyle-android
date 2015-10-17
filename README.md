# checkstyle-android

A [gradle checkstyle](https://docs.gradle.org/current/userguide/checkstyle_plugin.html) configuration that most closely matches the [Android Code Style Guidelines for Contributors](https://source.android.com/source/code-style.html).

## Usage

Add this repo as a git submodule in your repo root
```
git submodule add git@github.com:hypest/checkstyle-android.git
```
Add it in your project's `build.gradle` like this:
```
apply from: 'checkstyle-android/checkstyle.gradle
```
You can now run the checks at the command line:
```
./gradlew checkstyle
```
Xml and html reports will be created in `<project build dir>/reports/checkstyle/`
You may opt to have the build fail if checkstyle reports issues. You can enable that by adding to build.gradle:
```
preBuild.dependsOn('checkstyle')
```

Alternatively, you can just grab the rules file and use it with your own checkstyle setup.
## Prerequisities

Things you will need:

* gradle and/or AndroidStudio

## Running the tests

* 

## Contributing

Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct and the process for contributing!

## History

**v0.1**: Initial repo setup

## Authors

**Stefanos Togoulidis** - [hypest](https://github.com/hypest)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details

## Acknowledgments

*
