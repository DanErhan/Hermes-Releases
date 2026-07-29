# HERMES

**An AI trading desk that runs on your own machine.**

Hermes connects to your broker, journals every trade you make automatically, and
tells you what actually drives your results — in plain language, by voice.

It is an assistant, not a bot that trades for you. Autonomous trading ships
**off**, behind a switch you have to arm deliberately, and it stays off until
you do.

---

## Download

**[→ Latest release](../../releases/latest)**

| Your computer | File |
|---|---|
| Mac with Apple Silicon (M1–M4) | `Hermes-<version>-mac-arm64.dmg` |
| Windows 10 / 11, 64-bit | `Hermes-<version>-win-x64.exe` |

**Intel Macs are not supported yet.** Check first: Apple menu → About This Mac.
If it says *Apple M1/M2/M3/M4* you're fine. If it says *Intel*, this build will
not open at all — an Intel version is coming, and it's worth the ten seconds to
check rather than wonder why nothing happens.

---

## Installing

The beta is **not code-signed yet**, so both operating systems will warn you the
first time. The warning means "we don't recognise this publisher" — not "we
found something wrong". Here is how to get past it.

### Windows

1. Run the `.exe`.
2. Windows says **"Windows protected your PC"**.
   Click **More info** → **Run anyway**.
3. Follow the installer and launch Hermes from the Start menu.

### macOS

1. Open the `.dmg` and drag **Hermes** to Applications.
2. **First launch only:** open Applications, **right-click** Hermes → **Open** →
   **Open** again.
   (Double-clicking will just be refused. Right-click → Open is how you tell
   macOS you trust it. You do this once.)

First start takes a minute while it prepares its data files. That is normal.

---

## Starting your 30 days

Enter your email on the first screen. You may be emailed a 6-digit code to
confirm the address — type it in, and you're in. That's it: 30 days, nothing
charged, no card asked for.

Your licence is tied to that computer, and you can run it on two (a desktop and
a laptop, say). One trial per machine, and the 30 days count from the moment
you sign up.

---

## What you'll need

- **A broker account — use a demo.** cTrader is the best-tested path (free demo
  in two minutes at your broker or ctrader.com). MT4, MT5 and OANDA are also
  supported. This is beta software: do not point it at money you care about.
- **Optional: your own AI and voice keys** (Anthropic, OpenAI, Google,
  ElevenLabs). Hermes uses *your* accounts, never anyone else's, and the keys
  are encrypted on your machine. Skip them and it still works — system voice,
  and answers computed from your own trade data.

---

## What it does on first run

A short setup: create a local profile, connect cTrader, import your history.
Then, before you configure anything, it shows you a real analysis of your own
trading. That's the part worth waiting for.

To talk to it, hold **Ctrl** and speak:

> "What's my worst hour of the day?"
> "How did I do on gold this month?"
> "Short gold, one percent risk, forty pip stop."

It will read an order back to you before anything is sent, and it will tell you
plainly when something did *not* happen. It never claims a trade was placed
unless the broker confirmed it.

---

## Your data

Everything lives on your machine. Broker credentials and API keys are encrypted
with a key from your OS keychain. Nothing about your hardware is transmitted —
licensing uses a one-way fingerprint, never a serial number.

Uninstalling removes the app; your data lives separately, so it survives an
update and can be deleted on its own.

---

## Something wrong?

Open an [issue](../../issues) — include your **Installation ID** (bottom of the
activation screen; it's a hash, it identifies nothing about you) and what you
were doing. Bug reports from the beta are the entire point of the beta.

---

## Known limits, honestly

- **Not code-signed yet**, hence the warnings above.
- **Apple Silicon only on macOS.** An Intel build needs a build machine we don't
  currently have; the file here will not open on an Intel Mac.
- **cTrader is the path that has been tested properly.** MT4, MT5 and OANDA are
  in this build and are newer — if you use one, expect rough edges and please
  report them.
- The beta is 30 days. Extensions are a message away.
- This repository holds **releases only** — no source. Hermes is not open source.

---

© 2026 Dan Erhan. Beta software, provided as is, for evaluation.
