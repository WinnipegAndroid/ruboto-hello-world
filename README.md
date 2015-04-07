# Ruboto Hello World

Check out the  [Ruboto project](https://github.com/ruboto/ruboto) for more information! Also, the API is [here](http://www.rubydoc.info/gems/ruboto/).

## Setup

### Prerequisites

- rbenv
- Java JDK
- Android SDK
- Apache ANT

### Shell

Add the following to your environment variables:
`export ANDROID_HOME=~/Documents/Android/SDK`
`export PATH=${PATH}:$ANDROID_HOME/tools:$ANDROID_HOME/platform-tools`

### Installation

1. `$ rbenv install jruby-1.7.9`
2. `$ rbenv shell jruby-1.7.9`
3. `$ gem install ruboto`
4. `$ gem install jruby-jars`
5. `$ ruboto setup` (May fail, use setup to verify prerequisites are detected)
6. `$ ruboto gen app --package com.ruboto.hello --name RubotoHelloWorld --target 16 --min-sdk 16 --activity Hello`
(Make sure you have the SDK for API level 16 for this step)
7. Connect your Android device/emulator
8. `$ rake install start`
9. :tada:

Note: You will need the Ruboto core app on your device! Once you launch your app, it will provide a link to download the Ruboto core app from the Google Play store. The Ruboto core app is also available for manual installation  [here](http://ruboto.org/downloads/).
