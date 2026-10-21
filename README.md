# ScrollScout

ScrollScout is a Mac app for researching Instagram Reels. While you scroll Reels in Chrome, it notices each new Reel, keeps a few frames and the audio, and lets you mark the good ones. Afterwards it transcribes them, reads their on-screen text, makes them searchable, and lets you ask questions across everything you saved, with every answer linked to the moment it comes from.

Everything runs on your Mac. Nothing you capture leaves it.

## Download

Get the latest DMG from **[Releases](../../releases/latest)**.

## What you need

- A Mac with Apple Silicon, on macOS 26 or later
- Google Chrome, with Instagram open in a window of its own
- Permission to record the screen and to control Chrome. ScrollScout needs both to record: reading Chrome's address is how it confirms the window is Instagram. The welcome screen asks for them.
- Apple Intelligence switched on, for summaries and questions (capture, transcripts and search work without it)

## Install

1. Open the DMG and drag ScrollScout into Applications.
2. Open it. The welcome screen walks you through Screen Recording and Chrome Automation.

ScrollScout is signed with a Developer ID and notarized by Apple, so it opens like any other Mac app.

## Privacy

- Recording, transcripts, on-screen text, search and answers all stay on your Mac.
- Video comes only from the Chrome window you choose, and only while it shows Instagram. Recording pauses when that tab leaves Instagram.
- Audio comes from all of Chrome. While you record, we suggest using Chrome only for Instagram: a call or video playing in another Chrome tab or window would be recorded and transcribed too.
- ScrollScout sends nothing over the network unless you turn something on. The update check (off by default) asks GitHub for the latest version number and nothing else. If you choose Claude for summaries in Settings, the text of the Reels you analyse goes to Anthropic. macOS downloads a speech model from Apple when you ask for one. Every request ScrollScout makes is listed in Settings → Privacy.
- Settings → General has an option for `scrollscout://` links, which is off by default. Leave it off: when it's on, a web page you visit can start a recording or ask the Companion a question.

## Where your research is kept

Everything ScrollScout saves is in `~/Library/Application Support/ScrollScout` on your Mac:

- `library.sqlite`: transcripts, on-screen text, captions, your notes and Companion chats
- `keyframes/`: still frames of the Reels you scrolled
- `audio/` and `journal/`: the recorded audio
- `diagnostics/`: crash reports, which stay on your Mac unless you export one

These are plain files on your disk, protected by your Mac login (and FileVault, if it's on), like most apps' data. To remove something, delete the session or Reel in the Library. To remove everything, quit ScrollScout and delete that folder.

## Updates

ScrollScout → Check for Updates… tells you when a new version is here, and its Download button opens this page. Install the new DMG the same way.
