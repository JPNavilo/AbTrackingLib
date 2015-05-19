# AbTrackingLib

[![CI Status](http://img.shields.io/travis/Laura Orán/AbTrackingLib.svg?style=flat)](https://travis-ci.org/Laura Orán/AbTrackingLib)
[![Version](https://img.shields.io/cocoapods/v/AbTrackingLib.svg?style=flat)](http://cocoapods.org/pods/AbTrackingLib)
[![License](https://img.shields.io/cocoapods/l/AbTrackingLib.svg?style=flat)](http://cocoapods.org/pods/AbTrackingLib)
[![Platform](https://img.shields.io/cocoapods/p/AbTrackingLib.svg?style=flat)](http://cocoapods.org/pods/AbTrackingLib)

## Usage

To run the example project, clone the repo, and run `pod install` from the Example directory first.

## Requirements

## Installation

AbTrackingLib is available through [CocoaPods](http://cocoapods.org). To install
it, simply add the following line to your Podfile:

```ruby
pod "AbTrackingLib"
```
To trigger the event, in your application delegate import the library:
```
#import <AbTrackingLib/ABTracker.h>
```

and add the following code in didFinishLaunchingWithOptions:
```
NSString *bundleId = [[NSBundle mainBundle] bundleIdentifier];
NSString *appVersion = [[NSBundle mainBundle] objectForInfoDictionaryKey:(NSString *)kCFBundleVersionKey];
[ABTracker trackOpenEventVersion:appVersion andBundle:bundleId];
```

In order to send your bundle ID and your App Version to abtrckr.com

## Author

Laura Orán, laura.oran@navilo.es

## License

AbTrackingLib is available under the MIT license. See the LICENSE file for more info.
