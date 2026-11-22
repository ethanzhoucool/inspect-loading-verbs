# inspect-loading-verbs

Ramp's coding agent, Inspect, says "Thinking…" while it works. This makes it say "Reconciling…" instead. Or "Depreciating gracefully…", or "Whatchamacalliting…".

It's one HTML file that mocks up the Inspect chat. Type a prompt, hit Enter, and it thinks forever.

```bash
python3 -m http.server 5178
```

Type `/` to search the verbs. The buttons in the bottom right switch between Before and After and blur the rest of the screen. To add your own verbs, edit `VERBS` at the top of the script.

Fan project, not affiliated with Ramp. Layout based on the screenshot in [Modal's post about Inspect](https://modal.com/blog/how-ramp-built-a-full-context-background-coding-agent-on-modal). MIT license.
