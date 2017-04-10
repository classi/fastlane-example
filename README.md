# fastlane-example
fastlane example by Classi Corp.

Fastfile supports **both iOS and android**.

# Description

Fastfile is compatible with both iOS and android.  
For example, `bundle exec fastlane ios beta` or `bundle exec fastlane android playstore`.

iOS Directory contains samples of Matchfile and Appfile.  
Android Directory also includes Appfile and so on.

It will be a reference for the continuous delivery of iOS / Android.


# Usage

## iOS

Fastfile:

```
fastlane_version "2.19.2"

import_from_git(
  url: 'https://github.com/classi/fastlane-example',
  path: 'iOS/fastlane/Fastfile'
)
```

## Android

Fastfile:

```
fastlane_version "2.24.0"

import_from_git(
  url: 'https://github.com/classi/fastlane-example',
  path: 'Android/fastlane/Fastfile'
)
```

# Information for Japanese

[fastlane を利用した iOS 継続的デリバリーの実践 \| Classi株式会社's Blog](https://www.wantedly.com/companies/classi/post_articles/57007)

