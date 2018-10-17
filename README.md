# WebRTC libraries for iOS

This repository provides built WebRTC libraries which is configured for [WebRTC SFU Sora](https://sora.shiguredo.jp) iOS SDK.

## Supperted WebRTC Version

M70 (commit position 17)

## How to Use

### Carthage

Add the following line to Cartfile.

```ruby
# Without version
github "shiguredo/sora-webrtc-ios"

# With Version
github "shiguredo/sora-webrtc-ios" "70.17.0"
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
pod 'WebRTC', '= 70.17.0'
```

### Manual Download

Available from [releases](https://github.com/shiguredo/sora-webrtc-ios/releases) page of this repository.

## "Development" version

Some releases are always comes with its "development" variants, for example `70.17.0` and `70.17.0-dev`. Development variants are smaller binaries, which:

- bitcode is stripped off and not available
- support arm64 only (no armv7)
