## iOS 11 Camera Permissions Plugin for Apache Cordova

**NSCameraUsageDescription, NSPhotoLibraryUsageDescription, NSPhotoLibraryAddUsageDescription, NSMicrophoneUsageDescription and NSCalendarsUsageDescription in iOS 11 by adding a declaration to the Info.plist file**

## Install

#### Latest published version on npm (with Cordova CLI >= 5.0.0)

```
cordova plugin add cordova-plugin-ios-permissions --save
```

#### Latest version from GitHub

```
cordova plugin add https://github.com/brramos/cordova-plugin-ios-permissions.git --save
```

#### Customising the message prompts

On installation you can customise the prompts shown by setting the following variables on installation.

- CAMERA_USAGE_DESCRIPTION for NSCameraUsageDescription
- CALENDARS_USAGE_DESCRIPTION for NSCalendarsUsageDescription
- MICROPHONE_USAGE_DESCRIPTION for NSMicrophoneUsageDescription
- PHOTOLIBRARY_ADD_USAGE_DESCRIPTION for NSPhotoLibraryAddUsageDescription (write-access only, iOS 11 only)
- PHOTOLIBRARY_USAGE_DESCRIPTION for NSPhotoLibraryUsageDescription (read/write access)

For example:
```
cordova plugin add cordova-plugin-ios-camera-permissions --variable CAMERA_USAGE_DESCRIPTION="your usage message" --variable MICROPHONE_USAGE_DESCRIPTION="your microphone usage message here" --variable PHOTOLIBRARY_ADD_USAGE_DESCRIPTION="your photo library usage message here" --variable PHOTOLIBRARY_USAGE_DESCRIPTION="your photo library usage message here" --save
```

## Usage

For the changes to `plugin.xml` to take effect, you must refresh the `ios.json` file (inside the `/plugin` folder):
```
$ cordova platform rm ios
$ cordova platform add ios
```

## Platforms

Applies to iOS 10/11 only.

## License

[MIT License]
