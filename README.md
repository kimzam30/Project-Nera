# Project Nera

A single-file web page that delivers a personal letter as a retro terminal session — typewriter text, background music, and a timed image reveal. Built as a template: clone it, swap the words and media, send the link.

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/Vanilla_JS-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![No dependencies](https://img.shields.io/badge/dependencies-none-success?style=flat-square)

---

## What it is

One `index.html` — markup, styles, and logic in a single file, zero dependencies, no build step. Open it in a browser and it runs.

- **Terminal aesthetic** — phosphor-green monospace on black
- **Typewriter rendering** — text types out character by character on a timer
- **Audio** — background track fades in once the visitor interacts (browsers block autoplay until then)
- **Staged reveal** — two message passages, then an image with a heartbeat animation
- **Private by default** — the media files are gitignored, so forking the repo never exposes your photo or song

---

## Use it

### 1. Clone

```bash
git clone https://github.com/kimzam30/Project-Nera.git
cd Project-Nera
```

### 2. Add your media

The repository ships without media on purpose. Add two files to the project root:

| File | What |
|---|---|
| `song.mp3` | Background track |
| `us.jpg` | The image revealed at the end |

Both are listed in `.gitignore` — they will not be committed if you push your copy.

### 3. Write your letter

Open `index.html` and edit:

| What | Where |
|---|---|
| Message passages | The `myInsecurities` and `myReasons` arrays (~line 115) |
| Closing message | `finalP.innerHTML` (~line 182) |
| Pacing | The delay values in `runSequence()` — tune these to your track |

### 4. Preview

Open `index.html` in a browser. Audio needs a click first, so trigger the sequence rather than expecting sound on load.

---

## Deploying

Because the media is gitignored, **connecting this repo to Netlify or Vercel will deploy a version with no music and no image**. Deploy the local folder directly instead:

**Netlify drop** — go to [app.netlify.com/drop](https://app.netlify.com/drop) and drag your project folder (with `song.mp3` and `us.jpg` in it) onto the page. You get a live URL immediately.

**Vercel CLI**

```bash
npx vercel --prod
```

Run it from the folder containing your media — the CLI uploads local files rather than pulling from git.

---

## License

MIT — see [LICENSE](LICENSE). Use it, fork it, rewrite it for whoever you're writing to.
