# Role Play: visual demo

A self-playing, **simulated** walkthrough of the Role Play voice-AI training use case, for prospects who want to *see* the product before a contract. It is not a working product.

- **What it shows:** a trainee plays the operator (OP) and practises one call with an AI agent that plays the customer, in six steps: choose a call, phone connects, live call (transcript and the trainee's notes typed during the call), call ends, the trainee's summary of how the practice call went plus a to-do list, saved to history.
- **Two use cases:** Inbound (shareholder benefits help desk) and Outbound (internet / fiber sales). Switch between them at the top.
- **Languages:** English and Japanese (switcher in the header).
- **Controls:** speed (0.6x / 1x / 1.8x), restart, pause, and click any step in the list to jump to it. Light / dark theme.
- **No backend, no microphone, no AI calls.** Everything is scripted sample data. Nothing here is a real call.

The full working project (live AI voice customers, the client's own scripts and use cases) is built after contract.

## Run locally

```bash
npx serve .
```

Static site: `index.html` only, no build step. Deploy it on any static host (publish directory `.`).

## Edit the content

All text and the sample call are in `index.html`:
- `UI` : interface text (English / Japanese)
- `DATA` : the sample transcript, notes, summary and to-dos for each use case
- `LOGS` : the activity-log entries
- `DUR` : how long each step lasts (ms)

Query parameters: `?lang=ja` and `?uc=outbound` open the demo in Japanese or on the outbound use case.
