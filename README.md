# ScrollScout

ScrollScout is a Mac app for researching Instagram Reels. While you scroll Reels in Chrome, it notices each new Reel, keeps a few frames and the audio, and lets you mark the good ones. Afterwards it transcribes them, reads their on-screen text, makes them searchable, and lets you ask questions across everything you saved, with every answer linked to the moment it comes from.

Everything runs on your Mac. Nothing you capture leaves it.

## Download

Get the latest DMG from **[Releases](../../releases/latest)**.

## What you need

- A Mac with Apple Silicon, on macOS 26 or later
- Google Chrome, with Instagram open in a window of its own
- Permission to record the screen and to control Chrome. ScrollScout needs both to record: reading Chrome's address is how it confirms the window is Instagram. Setup asks for them.
- Apple Intelligence switched on, for summaries and questions (capture, transcripts and search work without it)

## Install

1. Open the DMG and drag ScrollScout into Applications.
2. Open it. A short setup on the first screen walks you through Screen Recording and Chrome, and your first recording. You can skip it and bring it back any time from Help → Set Up ScrollScout.

ScrollScout is signed with a Developer ID and notarized by Apple, so it opens like any other Mac app.

## Privacy

The full [privacy policy](PRIVACY.md) covers everything below in more detail.

- Recording, transcripts, on-screen text, search and answers all stay on your Mac.
- Video comes only from the Chrome window you choose, and only while it shows Instagram. Recording pauses when that tab leaves Instagram.
- Audio comes from all of Chrome. ScrollScout pauses its audio while another Chrome window shows it's playing sound, but it can't hear which background tab is playing. So while you record, we suggest using Chrome only for Instagram.
- Once a day ScrollScout asks GitHub whether there's a newer version. It sends nothing about you or your research, and you can turn it off in Settings → General. Nothing else leaves your Mac unless you ask for it: macOS downloads a speech model from Apple when you ask for one, and Claude (for summaries and the Companion) is available on request from vv@c4e.in. If you use it, the text of the Reels involved goes to Anthropic. Every request ScrollScout makes is listed in Settings → Privacy.
- Settings → General has an option for `scrollscout://` links, which is off by default. Leave it off: when it's on, a web page you visit can start a recording or ask the Companion a question.

## Where your research is kept

Everything ScrollScout saves is in `~/Library/Application Support/ScrollScout` on your Mac:

- `library.sqlite`: transcripts, on-screen text, captions, your notes and Companion chats
- `keyframes/`: still frames of the Reels you scrolled
- `audio/` and `journal/`: the recorded audio
- `diagnostics/`: crash reports, which stay on your Mac unless you export one

These are plain files on your disk, protected by your Mac login (and FileVault, if it's on), like most apps' data. To remove something, delete the session or Reel in the Library. To remove everything, quit ScrollScout and delete that folder.

## Updates

ScrollScout checks for a new version once a day (you can turn this off) and tells you when one is here. ScrollScout → Check for Updates… checks right away. Its Download button opens this page; install the new DMG the same way.
