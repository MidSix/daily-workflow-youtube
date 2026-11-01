# Daily Workflow: YouTube add-on

A separate Android app that Daily Workflow downloads only when someone opens
YouTube in it. It shows YouTube in Firefox's engine (GeckoView), where Google
allows signing in, with Daily Workflow's filter: the home page goes to the
subscriptions, recommended videos are hidden, and Shorts don't scroll to the
next one.

It has no launcher icon, and only Daily Workflow can open it: its screen
requires a permission granted only to apps signed with the same key.

## Files (release v1.0)

Daily Workflow downloads the file for the phone's processor and installs it
only if its SHA-256 matches:

| File | Processor | Bytes | SHA-256 |
|---|---|---|---|
| `youtube-arm64-v8a.apk` | phones | 79477274 | `d3582fc2bc0fd859c8e6a95f1e338a04f958f5f0637933f366e258cdc963d6ce` |
| `youtube-x86_64.apk` | emulator | 83039354 | `f8000834c51b834b963045b3574f7ab279b082b7e59afa794fc785263484e6ba` |

## Third-party code

The APKs include GeckoView 130.0.20240913135723 by Mozilla, under the
[Mozilla Public License 2.0](https://mozilla.org/MPL/2.0/). Its source code is
at <https://github.com/mozilla/gecko-dev>.
