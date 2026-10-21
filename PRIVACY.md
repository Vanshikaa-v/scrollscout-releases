# ScrollScout privacy policy

Last updated: 21 October 2026

ScrollScout is a Mac app for researching Instagram Reels. It works on your Mac. We don't run any servers for it, there are no accounts, and we never receive your recordings, your notes or anything else you do in the app. There are no analytics, ads or trackers.

## What ScrollScout records

While you record a session:

- **Video:** still frames of the one Chrome window you choose, and only while it shows Instagram. Recording pauses when that window leaves Instagram.
- **Audio:** the sound from Chrome. macOS gives an app all of Chrome's sound, not one tab's. ScrollScout pauses its audio while another Chrome window shows it's playing sound, but it can't tell which background tab is playing, so a call or video in another tab could still be recorded. We suggest using Chrome only for Instagram while you record.
- **The address and title of Chrome's windows,** read through Chrome's scripting interface, to tell one Reel from the next. Only Instagram addresses are kept. Other windows' addresses and titles are neither saved nor logged.
- **Your marks, notes and research questions,** and your questions to the Companion.

## What ScrollScout makes from it

Transcripts (Apple's on-device speech recognition), on-screen text (Apple's on-device text recognition), summaries and Companion answers (Apple Intelligence on your Mac). These are made on your Mac.

## Where it's kept

Everything is in `~/Library/Application Support/ScrollScout` on your Mac, as plain files protected by your Mac login, and by FileVault if it's on. ScrollScout doesn't add its own encryption. Crash reports from macOS are kept in the same folder and are only shared if you export one and send it yourself.

## What can leave your Mac

Only these:

1. **Update check** (on by default, once a day; turn it off in Settings → General). ScrollScout asks GitHub for the latest version number. It sends nothing about you or your research. GitHub sees your IP address, as with any web request. [GitHub's privacy statement](https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement) applies.
2. **Claude** (available on request from vv@c4e.in; it needs your own Anthropic API key). If you use Claude for summaries or the Companion, the text of the Reels involved (transcripts, on-screen text, captions) goes to Anthropic, and so does your question to the Companion. Your notes and your sessions' research questions are never sent. Your key is stored in your Mac's Keychain. [Anthropic's privacy policy](https://www.anthropic.com/legal/privacy) applies.
3. **Speech model.** When you ask for one, macOS downloads a speech recognition model from Apple.

Every request ScrollScout itself makes is listed, before it's sent, in Settings → Privacy → Network activity.

## Permissions it asks for

- **Screen Recording,** to see the Chrome window you choose.
- **Automation for Chrome,** to read the address and title of Chrome's windows. It never runs anything inside the web page.
- **Speech Recognition,** to transcribe audio on your Mac.

## Your control

- Delete a session in the Library, and everything ScrollScout kept for it is removed. Deleting a single Reel removes its frames, text and audio clip, but the session's full audio recording stays until you delete the session.
- To remove everything, quit ScrollScout and delete the folder above.
- Turn the daily update check off in Settings → General, or remove your Claude key in Settings.
- Leave "scrollscout:// links" off in Settings → General. When it's on, a web page you visit can start a recording or ask the Companion a question.

## Other people's content

The Reels you record belong to their creators. ScrollScout is for your own research. Please respect Instagram's terms and the creators' rights.

## Children

ScrollScout isn't directed at children under 13.

## Changes

If this policy changes, the new version will be posted here with a new date.

## Contact

Questions: [vv@c4e.in](mailto:vv@c4e.in)
