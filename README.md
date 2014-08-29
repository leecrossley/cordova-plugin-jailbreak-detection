## Native Transitions Plugin for Apache Cordova

Use this plugin to add an extra layer of security for your app, by detecting if the device running the app is jailbroken.

Unfortunately, there are 10s of millions of jailbroken iOS devices, so preventing your app from running on a jailbroken device could lead to a limited userbase and/or bad App Store reviews.

**I recommend you use this plugin to block certain features in your app rather than prevent it from running entirely.**

## Install

### Locally

```
cordova plugin add https://github.com/leecrossley/cordova-plugin-jailbreak-detection.git
```

You **do not** need to reference any JavaScript, the Cordova plugin architecture will add a `jailbreakdetection` object to your root automatically when you build.

## Usage

### isJailbroken

```js
jailbreakdetection.isJailbroken(successCallback, failureCallback);
```

- => `successCallback` is called with true if the device is Jailbroken, otherwise false
- => `failureCallback` is called if there was an error determining if the device is Jailbroken

## Platform Support

iOS only.

## License

[MIT License](http://ilee.mit-license.org)
