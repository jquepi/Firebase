#  [DEPRECATED] This Repository is no Longer Maintained

This was an experimental project. Firebase team has already started to work on carthage support in their main repository. 
For more information please refer to [Firebase-iOS-Carthage](https://github.com/firebase/firebase-ios-sdk/blob/master/Carthage.md).


# Firebase-Carthage
[![Carthage compatible](https://img.shields.io/badge/Carthage-compatible-4BC51D.svg?style=flat)](https://github.com/Carthage/Carthage)

#### Unofficial Carthage support for Firebase.

If you are looking for open source Firebase repository you may refer to [Firebase-iOS-SDK](https://github.com/firebase/firebase-ios-sdk).

----

## Usage
The iOS Example file is a sample of using core firebase (analytics). 

You need to add <b>GoogleService info plist</b> to your main project. (iOS Example project also needs Googleservice info plist)

## Installation

### Carthage

[Carthage](https://github.com/Carthage/Carthage) is a decentralized dependency manager that builds your dependencies and provides you with binary frameworks.

You can install Carthage with [Homebrew](http://brew.sh/) using the following command:

```bash
$ brew update
$ brew install carthage
```

To integrate Firebase into your Xcode project using Carthage, specify it in your `Cartfile`:

```ogdl
github "soheilbm/Firebase" 
```

Run `carthage update` to build the framework and drag the built `Firebase.framework` into your Xcode project.

- Add the -ObjC flag to "Other Linker Settings"
- Turn on ALWAYS_EMBED_SWIFT_STANDARD_LIBRARIES in your build settings.
- Drag each framework from the directory named after the SDK into the Project
   Navigator pane. Note that there may be no additional frameworks, in which
   case this directory will be empty. For instance, if you want the Database
   SDK, look in the Database folder for the required frameworks. In the dialog
   box that appears, make sure the target you want this framework to be added to
   has a checkmark next to it, and that you've selected "Copy items if needed.


"(~> X)" below means that the SDK requires all of the frameworks from X. You
should make sure to include all of the frameworks from X when including the SDK.
Add the following Framework to your project with [carthage copy-framework](https://github.com/Carthage/Carthage#getting-started) method.


#### Analytics
  - FirebaseAnalytics.framework
  - FirebaseNanoPB.framework
  - FirebaseCoreDiagnostics.framework
  - FirebaseCore.framework
  - FirebaseInstanceID.framework
  - GoogleToolboxForMac.framework
  - nanopb.framework

#### ABTesting (~> Analytics)
  - FirebaseABTesting.framework
  - Protobuf.framework

#### AdMob (~> Analytics)
  - GoogleMobileAds.framework

#### Auth (~> Analytics)
  - FirebaseAuth.framework
  - GTMSessionFetcher.framework

#### Crash (~> Analytics)
  - FirebaseCrash.framework
  - Protobuf.framework

#### Database (~> Analytics)
  - FirebaseDatabase.framework
  - leveldb-library.framework

#### DynamicLinks (~> Analytics)
  - FirebaseDynamicLinks.framework

#### Firestore (~> Analytics)
  - BoringSSL.framework
  - FirebaseFirestore.framework
  - Protobuf.framework
  - gRPC.framework
  - gRPC-Core.framework
  - gRPC-ProtoRPC.framework
  - gRPC-RxLibrary.framework
  - leveldb-library.framework

  You'll also need to add the resources in the
  Resources directory into your target's main
  bundle.

#### Invites (~> Analytics)
  - FirebaseDynamicLinks.framework
  - FirebaseInvites.framework
  - GTMOAuth2.framework
  - GTMSessionFetcher.framework
  - GoogleAPIClientForREST.framework
  - GoogleSignIn.framework
  - Protobuf.framework

  You'll also need to add the resources in the
  Resources directory into your target's main
  bundle.

#### Messaging (~> Analytics)
  - FirebaseMessaging.framework
  - Protobuf.framework

#### Performance (~> Analytics)
  - FirebasePerformance.framework
  - FirebaseSwizzlingUtilities.framework
  - GTMSessionFetcher.framework
  - Protobuf.framework

#### RemoteConfig (~> Analytics)
  - FirebaseABTesting.framework
  - FirebaseRemoteConfig.framework
  - Protobuf.framework

#### Storage (~> Analytics)
  - FirebaseStorage.framework
  - GTMSessionFetcher.framework

# Samples

You can get samples for Firebase from https://github.com/firebase/quickstart-ios:

git clone https://github.com/firebase/quickstart-ios

Note that several of the samples depend on SDKs that are not included with
this archive; for example, FirebaseUI. For the samples that depend on SDKs not
included in this archive, you'll need to use CocoaPods.

# Versions

The frameworks in this directory map to these versions of the Firebase SDKs in
Carthage.

|           Carthage           | Version |
----------------------------- | ------- |
| BoringSSL                     | 9.2 |
| Firebase                      | 4.10.0 |
| FirebaseABTesting             | 1.0.0 |
| FirebaseAnalytics             | 4.1.0 |
| FirebaseAuth                  | 4.4.4 |
| FirebaseCore                  | 4.0.16 |
| FirebaseCrash                 | 2.0.2 |
| FirebaseDatabase              | 4.1.5 |
| FirebaseDynamicLinks          | 2.3.2 |
| FirebaseFirestore             | 0.10.2 |
| FirebaseInstanceID            | 2.0.9 |
| FirebaseInvites               | 2.0.2 |
| FirebaseMessaging             | 2.1.1 |
| FirebasePerformance           | 1.1.2 |
| FirebaseRemoteConfig          | 2.1.2 |
| FirebaseStorage               | 2.1.3 |
| FirebaseSwizzlingUtilities    | 1.0.0 |
| GTMOAuth2                     | 1.1.6 |
| GTMSessionFetcher             | 1.1.14 |
| Google-Mobile-Ads-SDK         | 7.29.0 |
| GoogleAPIClientForREST        | 1.3.2 |
| GoogleSignIn                  | 4.1.2 |
| GoogleToolboxForMac           | 2.1.3 |
| Protobuf                      | 3.5.0 |
| gRPC                          | 1.9.1 |
| gRPC-Core                     | 1.9.1 |
| gRPC-ProtoRPC                 | 1.9.1 |
| gRPC-RxLibrary                | 1.9.1 |
| leveldb-library               | 1.20 |
| nanopb                        | 0.3.8 |

## Author

Soheil B.Marvasti


## License
I do not own this project. This is just a simple repository to bring Carthage compatibility to Firebase. 
