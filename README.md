# inspect-loading-verbs

What if Ramp's Inspect said "Reconciling…" instead of "Thinking…"?

Inspect is Ramp's coding agent. While it works, it shows a plain "Thinking…". This is a one-page mockup of the Inspect chat where that line cycles through finance verbs like "Depreciating gracefully…" and "Flagging an out-of-policy latte…", plus a few whimsical ones like "Whatchamacalliting…".

```bash
python3 -m http.server 5178
```

Type a prompt and hit Enter. It runs a few fake tool steps, then thinks forever. Type `/` to search every verb, and use the buttons in the bottom right to compare Before and After. To add your own verbs, edit `VERBS` in `index.html`.

Fan project, not affiliated with Ramp. MIT.
