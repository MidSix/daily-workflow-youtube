# Daily Workflow: YouTube & TikTok add-on

A separate Android app that Daily Workflow downloads only when someone opens
YouTube or TikTok in it. It shows them in Firefox's engine (GeckoView), where
Google allows signing in, with Daily Workflow's filters:

- YouTube: the home page goes to the subscriptions, recommended videos are
  hidden, and Shorts don't scroll to the next one.
- TikTok: Home is the feed of the accounts one follows ("For You", Explore and
  LIVE never open), and a single video (one a friend sent, one of a profile or
  a search) can be watched with its comments but not swiped to the next one.
  The messages open in TikTok's version for computers, the only one that has
  them, fitted to the phone's screen.

It has no launcher icon, and only Daily Workflow can open it: its screens
require a permission granted only to apps signed with the same key. (The
repository and file names are from when it was only YouTube's.)

## Files (release v1.3)

Daily Workflow downloads the file for the phone's processor and installs it
only if its SHA-256 matches:

| File | Processor | Bytes | SHA-256 |
|---|---|---|---|
| `youtube-arm64-v8a.apk` | phones | 79482760 | `f8b57e2bbc73d2f3cbe8c00d0c9860d6923628be3b559762d64012fbf195e07e` |
| `youtube-x86_64.apk` | emulator | 83044840 | `421e91386a9bab427502d9774824998f23858e68918596cb591e152fa0543065` |

## Versions

- **v1.3**: the keyboard no longer covers what is typed (the page shrinks above it).
- **v1.2**: TikTok too (the accounts one follows; a single video, also one a friend sent, cannot be swiped to the next; the messages open in TikTok's version for computers, fitted to the phone's screen); windows a page opens (signing in with Google, Facebook…) work; and the comments of a YouTube Short scroll again (only the swipe to the next Short is stopped).
- **v1.1**: the "Sign in" button is shown again (v1.0 hid it, so one could not sign in).
- **v1.0**: first version.

## Third-party code

The APKs include GeckoView 130.0.20240913135723 by Mozilla, under the
[Mozilla Public License 2.0](https://mozilla.org/MPL/2.0/). Its source code is
at <https://github.com/mozilla/gecko-dev>.
