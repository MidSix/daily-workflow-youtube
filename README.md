# Daily Workflow: YouTube add-on

A separate Android app that Daily Workflow downloads only when someone opens
YouTube in it. It shows YouTube in Firefox's engine (GeckoView), where Google
allows signing in, with Daily Workflow's filter: the home page goes to the
subscriptions, recommended videos are hidden, and Shorts don't scroll to the
next one.

It has no launcher icon, and only Daily Workflow can open it: its screen
requires a permission granted only to apps signed with the same key.

## Files (release v1.1)

Daily Workflow downloads the file for the phone's processor and installs it
only if its SHA-256 matches:

| File | Processor | Bytes | SHA-256 |
|---|---|---|---|
| `youtube-arm64-v8a.apk` | phones | 79477286 | `70247a25f084442d7cfef2816d8bde348772e8c6dad32842ee12f2586025413d` |
| `youtube-x86_64.apk` | emulator | 83039362 | `53edb7bb1541fc52efdb4d6bf948c7b2615697fecba55183ae8f5e8e4e817ffd` |

## Versions

- **v1.1**: the "Sign in" button is shown again (v1.0 hid it, so one could not sign in).
- **v1.0**: first version.

## Third-party code

The APKs include GeckoView 130.0.20240913135723 by Mozilla, under the
[Mozilla Public License 2.0](https://mozilla.org/MPL/2.0/). Its source code is
at <https://github.com/mozilla/gecko-dev>.
