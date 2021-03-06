# WebRTC libraries for iOS

This repository provides built WebRTC libraries which is configured for [WebRTC SFU Sora](https://sora.shiguredo.jp) iOS SDK.

## Supperted WebRTC Version

M76 (commit position 3, `9863f3d246e2da7a2e1f42bbc5757f6af5ec5682`)

## How to Use

### Carthage

Add the following line to Cartfile.

```ruby
# Without version
github "shiguredo/sora-webrtc-ios"

# With Version
github "shiguredo/sora-webrtc-ios" "76.3.0"
```

### CocoaPods

To retrieve the binary using CocoaPods, you need to add a `source` line at the top of the default `source` in your `Podfile`, like this:

```ruby
# ADD THIS LINE
# Make sure to put it on top of the default CocoaPods specs to override "WebRTC" reference!
source 'https://github.com/shiguredo/sora-ios-sdk-specs.git'
# This is the default source line which refers the default CocoaPods specs
source 'https://github.com/CocoaPods/Specs.git'
```

Then you can add the following line to `Podfile` as follows:

```ruby
# Without version
pod 'WebRTC'

# With version
pod 'WebRTC', '= 76.3.0'
```

### Manual Download

Available from [releases](https://github.com/shiguredo/sora-webrtc-ios/releases) page of this repository.

## "Development" version (iOS)

Some releases are always comes with its "development" variants, for example `76.3.0` and `76.3.0-dev`. Development variants are smaller binaries, which:

- bitcode is stripped off and not available
- support arm64 only (no armv7)
