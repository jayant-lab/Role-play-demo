# Role Play: demo

A self-playing walkthrough of the Role Play voice-AI training use cases. A trainee plays the operator (OP) and practises calls with an AI agent that plays the customer.

- **Both use cases on one page:** Inbound (shareholder benefits help desk) and Outbound (internet / fiber sales). Each has its own walkthrough; the lower one starts when you scroll to it.
- **Six steps each:** choose a call, phone connects, live call (transcript and the trainee's notes typed during the call), call ends, the trainee's summary of how the practice call went plus a to-do list, saved to history.
- **Languages:** English and Japanese (switcher in the header). Light and dark theme.
- **Controls:** speed (0.6x / 1x / 1.8x), restart and pause apply to both walkthroughs; click any step to jump to it.
- **No backend, no microphone, no AI calls:** everything is scripted.

## Run locally

```bash
npx serve .
```

Static site: `index.html` only, no build step. Deploy on any static host (publish directory `.`).

## Edit the content

All text and the sample calls are in `index.html`:
- `UI` : interface text (English / Japanese)
- `DATA` : the sample transcript, notes, summary and to-dos for each use case
- `LOGS` : the activity-log entries
- `DUR` : how long each step lasts (ms)

`?lang=ja` opens the page in Japanese.
