# Inspect loading verbs

A small concept: what if [Inspect](https://inspect.com), Ramp's background coding agent, swapped its generic `Thinking…` line for verbs that sound like Ramp?

> Reconciling… · Receipt-wrangling… · Flagging an out-of-policy latte… · Depreciating gracefully… · Net-thirtying…

It's a single HTML file that recreates the Inspect chat view. Type a prompt and press Enter. Inspect runs a few tool steps, then thinks forever, cycling through the verbs.

## Try it

Open `index.html` in a browser, or serve the folder:

```bash
python3 -m http.server 5178
```

Then go to http://localhost:5178.

- **Enter** sends a prompt.
- **/** opens a searchable list of every verb. Use the arrow keys to move and Esc to close.
- **Before / After** (bottom right) switches between plain `Thinking…` and the Ramp verbs.
- **Focus** blurs everything except the thinking line while Inspect works.

## Make it yours

Everything you'd want to change is at the top of the `<script>` block:

| Setting | What it does |
|---|---|
| `VERBS` | The verb list |
| `VERB_INTERVAL_MS` | How long each verb stays on screen |
| `TOOL_STEPS` | How many tool lines appear before it settles into thinking |
| `BEFORE` | What the Before button shows |
| `MODEL` | The model name shown in the composer and sidebar |

## Credits

The layout is based on a public screenshot of Inspect in [Modal's write-up on how Ramp built it](https://modal.com/blog/how-ramp-built-a-full-context-background-coding-agent-on-modal).

This is a fan concept by Ethan Zhou and isn't affiliated with or endorsed by Ramp. "Inspect" and "Ramp" are their respective owners' trademarks.

## License

MIT
