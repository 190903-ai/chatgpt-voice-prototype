# ChatGPT Voice: Live Transcript Prototype

A working prototype from my product case study on increasing voice input in the ChatGPT mobile app. It shows the idea I picked: **show the user's words on screen while they speak**.

**Live prototype:** https://voice-prototype-live.vercel.app/

## The problem
Students know ChatGPT Voice exists, but they still type. In my survey, people said voice feels rushed, the AI interrupts them, and it misunderstands them. They also could not see what they had said.

## The idea
Live transcripts while speaking, in both the mic button and Voice mode. I scored five ideas with RICE and this one came first (score 16.20).

## What you can try
Use the buttons at the top of the page.
- **Demo mode:** plays a sample conversation so you can see the feature without a microphone.
- **Baseline (no transcript):** how it works today, with no words shown.
- **Reply captions:** shows live captions with the transcript. Words that may still change are grey, and they turn black once they are final.
- **Reset first-run** and **Clear chat:** start over.
- **Live mic:** speak and watch your words appear. This uses the browser's Web Speech API, so use Chrome or Edge and allow the microphone.

## Run it yourself
It is one file with no build step and no keys.
1. Download or clone this repo.
2. Serve the folder, for example with `python -m http.server 8000`, then open http://localhost:8000. The microphone needs `localhost` or `https`.

## Files
- `index.html` is the whole prototype.

## Notes
- This is a student case-study prototype. It is not made by or connected to OpenAI. ChatGPT is a trademark of OpenAI.
- It does not send your voice or text anywhere. It makes no network calls.
- Success metric I proposed: voice sessions per user.
