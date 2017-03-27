# fastlane-example
fastlane example by Classi Corp.

# Requirements

## [Homebrew](https://brew.sh/)

```
$ brew install imagemagick
$ brew install graphicsmagick
```

## Environment Variables

```
ENV["DANGER_GITHUB_API_TOKEN"] = "YOUR_GITHUB_API_TOKEN"
ENV["FASTLANE_USER"] = "YOUR_APPLE_ID"
ENV["FASTLANE_PASSWORD"] = "YOUR_APPLE_PASSWORD"
ENV["DELIVER_PASSWORD"] = "YOUR_ITUNES_CONNECT_PASSWORD"
ENV["MATCH_PASSWORD"] = "YOUR_MATCH_PASSWORD"
ENV["CRASHLYTICS_API_TOKEN"] = "YOUR_CRASHLYTICS_TOKEN"
ENV["CRASHLYTICS_BUILD_SECRET"] = "YOUR_CRASHLYTICS_BUILD_SECRET"
ENV["SLACK_URL"] = "YOUR_SLACK_WEBHOOK_URL"
```

# Usage

## Test

```
$ bundle exec fastlane test
```

## Upload to crashlytics beta

```
$ bundle exec fastlane beta
```

## Upload to iTunes Connect

```
$ bundle exec fastlane release
```

## Create release branch

```
$ bundle exec fastlane release_branch version:2.0.0
```

# Information for Japanese

TODO: Wantedly URL.

