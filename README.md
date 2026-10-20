# ScrollScout

ScrollScout is a Mac app for researching Instagram Reels. While you scroll Reels in Chrome, it notices each new Reel, keeps a few frames and the audio, and lets you mark the good ones. Afterwards it transcribes them, reads their on-screen text, makes them searchable, and lets you ask questions across everything you saved, with every answer linked to the moment it comes from.

Everything runs on your Mac. Nothing you capture leaves it.

## Download

Get the latest DMG from **[Releases](../../releases/latest)**.

## What you need

- A Mac with Apple Silicon, on macOS 26 or later
- Google Chrome, with Instagram open in a window of its own
- Apple Intelligence switched on, for summaries and questions (capture, transcripts and search work without it)

## Install

1. Open the DMG and drag ScrollScout into Applications.
2. Open it once. macOS will say it can't check the app, because this build isn't notarized yet.
3. Go to **System Settings → Privacy & Security** and click **Open Anyway**.
4. The welcome screen walks you through Screen Recording and Chrome Automation.

## Privacy

- Recording, transcripts, on-screen text, search and answers all stay on your Mac.
- ScrollScout records only a Chrome window that's showing Instagram, and pauses when that tab leaves Instagram.
- ScrollScout sends nothing over the network unless you turn something on. The update check (off by default) asks GitHub for the latest version number and nothing else. If you choose Claude for summaries in Settings, the text of the Reels you analyse goes to Anthropic. macOS downloads a speech model from Apple when you ask for one. Every request ScrollScout makes is listed in Settings → Privacy.

## Updates

ScrollScout → Check for Updates… tells you when a new version is here, and its Download button opens this page. Install the new DMG the same way.
