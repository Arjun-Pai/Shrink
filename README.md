# Shrink

Shrink is a browser-based collection and launcher for small web games/experiences built for Hack Club.

## Included games

- `Obby.html` – 2D obstacle jumper
- `Reaction_tester.html` – reaction speed tester
- `Retro_Synthesizer.html` – playable mini synth
- `Voice_Changer.html` – simple voice effect player
- `Canvas.html` – quick sketch/drawing canvas

## Run locally

Because this project is static HTML/CSS/JS, you can run it with any static server.

### Option 1: Python

```bash
cd /home/runner/work/Shrink/Shrink
python3 -m http.server 8000
```

Then open `http://localhost:8000/`.

### Option 2: Node (`serve`)

```bash
cd /home/runner/work/Shrink/Shrink
npx serve .
```

Then open the URL printed in your terminal.

## Launcher and game organization

- `index.html` is the main launcher page.
- Game files are standalone `.html` files at the repository root.
- The launcher tries to discover `*.html` game files from directory listings when available and also includes a fallback list of known games so it works on static hosts like GitHub Pages.
- To add a game, add a new standalone HTML file and update the fallback game list in `index.html` if your host does not expose directory listings.

## Contributing

Contributions are welcome. Keep games standalone, dependency-free where possible, and avoid breaking existing game files.

## License

No license file is currently present in this repository. If you want open-source reuse terms, add a `LICENSE` file.
