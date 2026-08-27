# LENS Lab

Website for the LENS Lab (Light-based Exploration of Neural Systems), Kravis Department of Integrated Sciences, Claremont McKenna College.

## Files

- `index.html` — the entire site: markup, styles, and scripts in one file
- `images/` — all photographs and figures

## Published with GitHub Pages

Settings → Pages → Deploy from a branch → `main` → `/ (root)`

## Making changes

**Text** — open `index.html`, click the pencil icon, edit, commit. The live site updates in about a minute.

**Replacing a photo** — upload the new file to `images/` using the same filename it replaces. No change to `index.html` is needed.

**Adding a photo** — upload it to `images/`, then reference it in `index.html` as `images/your-file.jpg`.

## Image reference

| File | Used for |
| --- | --- |
| `invivo-imaging.gif` | *in vivo* imaging card (animated, 13 frames) |
| `behavior-frogs.jpg` | Behavior tracking card |
| `plasticity-diagram.jpg` | Experience-dependent plasticity card |
| `xenopus-tadpole.jpg` | Xenopus organism panel |
| `ranitomeya-adult.jpg`, `ranitomeya-pair.jpg`, `ranitomeya-tadpole.jpg` | Ranitomeya organism panel |
| `team-*.jpg` | Team headshots |


## Adding an alumni section later

The alumni styles are still in `index.html` (search for `.alumni-`), but the markup was removed since there are no alumni to list yet. To bring the collapsible section back, paste this inside the `#team` section, just before its closing `</section>` tag, and edit the entries:

```html
<div class="team-subsection alumni-section" id="alumni">
  <button class="alumni-toggle" onclick="this.closest('.alumni-section').classList.toggle('open')">
    <span>Lab alumni</span>
    <svg class="alumni-chevron" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" xmlns="http://www.w3.org/2000/svg">
      <polyline points="6 9 12 15 18 9"/>
    </svg>
  </button>
  <div class="alumni-panel">
    <div class="alumni-grid">
      <div class="alumni-entry">
        <div class="alumni-name">Name</div>
        <div class="alumni-detail">Research assistant &middot; 2024-26</div>
        <div class="alumni-next">Where they went next.</div>
      </div>
    </div>
  </div>
</div>
```

Repeat the `alumni-entry` block for each person.
