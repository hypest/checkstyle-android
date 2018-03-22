# checkstyle-android

A [gradle checkstyle](https://docs.gradle.org/current/userguide/checkstyle_plugin.html) configuration that most closely matches the [Android Code Style Guidelines for Contributors](https://source.android.com/source/code-style.html). Many Android projects chose to follow those guidelines and this checkstyle configuration helps enforce them on your code.

This is still Work-In-Progress! Only a few rules have been implemented so far. Check the #Contributing section below on how to contrbute ;)

## Usage

You can just grab [the rules file](config/checkstyle.xml) and use it with your own checkstyle setup or you can add this repo as a git submodule:
```
git submodule add git@github.com:hypest/checkstyle-android.git
```
Add it in your project's `build.gradle` like this:
```
apply from: 'checkstyle-android/checkstyle.gradle'
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
## Prerequisities

You will need gradle or AndroidStudio.

## Contributing

Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct and how you can contribute to this project!

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
