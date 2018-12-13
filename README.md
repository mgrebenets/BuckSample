# BuckSample
This is a sample to show how to use Buck to build an iOS project with mixed languages (Swift & Objective C).

To explain how we use Buck, we have setup this repo as a demo.

[![Build Status](https://travis-ci.com/airbnb/BuckSample.svg?branch=master)](https://travis-ci.com/airbnb/BuckSample)

### To Install

```sh
# Install Buck
brew tap facebook/fb
brew install buck
```

### Running Tests
Press `Cmd + U` to run the unit tests for the `ExampleApp` target inside Xcode.

Or, from the terminal you can run `make test`.

<img src="https://github.com/airbnb/BuckSample/raw/master/Docs/CommandLineTests.png" width=500 />

### Viewing Targets
You may run `make targets` to see a list of Buck targets available to build/test/etc.

<img src="https://github.com/airbnb/BuckSample/raw/master/Docs/BuckTargets.png" width=500 />

### Generating an Xcode Project
To generate the project from the terminal, just run `make project`. You can then run in the simulator or press `Cmd + U` to run the tests.

You may also use breakpoints, just like normal when using the generated Xcode project.

<img src="https://github.com/airbnb/BuckSample/raw/master/Docs/Breakpoint.png" width=500 />


### References
1. https://github.com/airbnb/BuckSample/blob/master/Pods/BUCK gives a few examples on how we build CocoaPods with Buck
2. https://github.com/airbnb/BuckSample/tree/master/src/ImportObjC/BUCK shows how to config a mixed language build rule
3. https://github.com/airbnb/BuckSample/blob/master/src/ImportFromAnotherLibrary/BUCK shows how to import from another mixed language build rule
4. https://github.com/airbnb/BuckSample/blob/master/App/BUCK is the main build file which shows how we setup resources/assets and build the final binary/ipa file.

Buck Build channel https://buckbuild.slack.com.
