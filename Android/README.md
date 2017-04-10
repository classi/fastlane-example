# fastlane Android example

This is setting to run fastlane for android.

# Requirements

## [Homebrew](https://brew.sh/)

```
$ brew install imagemagick
$ brew install graphicsmagick
```

## Environment Variables

```
ENV["CRASHLYTICS_API_TOKEN"] = "YOUR_CRASHLYTICS_TOKEN"
ENV["CRASHLYTICS_BUILD_SECRET"] = "YOUR_CRASHLYTICS_BUILD_SECRET"
ENV["CRASHLYTICS_GROUPS"] = "YOUR_CRASHLYTICS_GROUPS"
ENV["SLACK_URL"] = "YOUR_SLACK_WEBHOOK_URL"
ENV["SLACK_CHANNEL"] = "YOUR_SLACK_CHANNEL"
ENV["GITHUB_REPOSITORY"] = "classi/fastlane-example"
ENV["BETA_GRADLE_FLAVOR"] = "staging"
ENV["BETA_GRADLE_BUILD_TYPE"] = "debug"
ENV["PLAYSTORE_GRADLE_FLAVOR"] = "product"
ENV["PLAYSTORE_GRADLE_BUILD_TYPE"] = "release"
ENV["BADGE_GLOB"] = "/**/main/**/ic_launcher.{png,PNG}"
ENV["GOOGLE_PLAY_API_KEY_JSON"] = "{...}"
```

# Usage

## Upload to crashlytics beta

```
$ bundle exec fastlane beta
```

## Upload to Google Play Store

```
$ bundle exec fastlane playstore
```

### Create release branch

```
$ bundle exec fastlane release_branch version:2.0.0
```

