# iOS Ads Support
Copy of the [ioS Ads Support Unity Plugin](https://github.com/Unity-Technologies/com.unity.ads.ios-support).

**Assembly:**\
com.unity.ads.ios-support

**Namespace:**\
Unity.Advertisement.IosSupport

**ASMDEF File:**\
Unity.Advertisement.IosSupport

**Scripting Define Symbol:**\
EXT_ADS_IOS_SUPPORT

# Using this package

This package supports Apple's SKAdNetwork and AppTrackingTransparency frameworks for your made-with-Unity iOS application, by aggregating proper ad network IDs and providing access to relevant Apple developer APIs.

For more information about iOS 14 technical integration, including this package's support functionality, please see the full [iOS 14 technical documentation](https://unityads.unity3d.com/help/monetization/ios14).

## Apple developer API extensions

This package provides access to the following Apple developer APIs:

```
public static void SkAdNetworkUpdateConversionValue(int conversionValue)
```
This method allows you to [update the attribution conversion value](https://developer.apple.com/documentation/storekit/skadnetwork/3566697-updateconversionvalue?language=objc).

```
SkAdNetworkRegisterAppForNetworkAttribution()
```
This method allows you to [register for attribution](https://developer.apple.com/documentation/storekit/skadnetwork/2943654-registerappforadnetworkattributi?language=objc).

```
public static void RequestAuthorizationTracking()
```
This method allows you to [request the user permission dialogue](https://developer.apple.com/documentation/apptrackingtransparency/attrackingmanager/3547037-requesttrackingauthorization).

```
public static AuthorizationTrackingStatus GetAuthorizationTrackingStatus()
```
This method allows you to check the app tracking transparency (ATT) [authorization status](https://developer.apple.com/documentation/apptrackingtransparency/attrackingmanager/3547038-trackingauthorizationstatus).

## Sample Project

The SampleProject~ folder included here is a complete Unity project, compatible with Unity 2018.4.33f1 and up. This project contains an example of a context screen you could use to give context to users before showing the native App Tracking Transparency dialog.

------------------------------
INSTALLATION INSTRUCTIONS
------------------------------
- Open your unity package manager manifest (YourProject/Packages/manifest.json)

- Add a new entry...\
  "com.unity.ads.ios-support": "https://github.com/BrandXR/com.unity.ads.ios-support.git?path=com.unity.ads.ios-support",

- If you want to keep up to date with this repo, then you're done.
- If you want a specific version, add #v1.0.0 to the end of the URL (replace with the released version you want)

- Check the [Unity manual](https://docs.unity3d.com/Manual/upm-git.html#subfolder) on installing plugins from the subfolder of a Git repo for more info.
