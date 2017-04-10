# fastlane iOS example

This is the environment setting necessary to run fastlane ios.

# Requirements

## [Homebrew](https://brew.sh/)

### iOS

```
$ brew install imagemagick
$ brew install graphicsmagick
```

## Environment Variables

### iOS

```
ENV["DANGER_GITHUB_API_TOKEN"] = "YOUR_GITHUB_API_TOKEN"
ENV["FASTLANE_USER"] = "YOUR_APPLE_ID"
ENV["FASTLANE_PASSWORD"] = "YOUR_APPLE_PASSWORD"
ENV["DELIVER_PASSWORD"] = "YOUR_ITUNES_CONNECT_PASSWORD"
ENV["MATCH_PASSWORD"] = "YOUR_MATCH_PASSWORD"
ENV["BETA_MATCH_TYPE"] = "development or ad-hoc"
ENV["CRASHLYTICS_API_TOKEN"] = "YOUR_CRASHLYTICS_TOKEN"
ENV["CRASHLYTICS_BUILD_SECRET"] = "YOUR_CRASHLYTICS_BUILD_SECRET"
ENV["CRASHLYTICS_GROUPS"] = "YOUR_CRASHLYTICS_GROUPS"
ENV["SLACK_URL"] = "YOUR_SLACK_WEBHOOK_URL"
ENV["XCOV_WORKSPACE"] = "classi.xcworkspace"
ENV["XCOV_SCHEME"] = "ClassiTests"
ENV["XCOV_EXCLUDE_TARGETS"] = "GoogleToolboxForMac.framework,Rswift.framework"
ENV["SLACK_CHANNEL"] = "YOUR_SLACK_CHANNEL"
ENV["RELEASE_GYM_SCHEME"] = "YOUR_RELEASE_SCHEME"
ENV["XCODEPROJ"] = "classi.xcodeproj"
ENV["GITHUB_REPOSITORY"] = "classi/fastlane-example"
```

# Usage

## iOS

### Test

```
$ bundle exec fastlane test
```

### Upload to crashlytics beta

```
$ bundle exec fastlane beta
```

### Upload to iTunes Connect

```
$ bundle exec fastlane release
```

### Create release branch

```
$ bundle exec fastlane release_branch version:2.0.0
```

