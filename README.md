# Liu Xuan'ang's Academic Homepage — Source

The `main` branch contains the published GitHub Pages site. This `hexo-source` branch contains the Hexo project used to build it.

## Build

Requirements: Node.js and npm.

```powershell
npm ci
npm run build
```

Hexo writes the generated site to `public/`. The homepage content is in `source/_posts/academic-home.md`; shared styles are in `source/css/academia-overrides.css`.

## Update profile assets

- Add a portrait at `source/images/avatar.jpg` and set `avatar: /images/avatar.jpg` in `themes/academia/_config.yml`.
- The public site links to `attaches/CV.pdf` on `main`. The CV is omitted from this source snapshot; for a local build, copy it to `source/attaches/CV.pdf`.
- The public contact email is omitted from this source snapshot. Add a contact link to `themes/academia/_config.yml` and `source/_posts/academic-home.md` if you want it in a local build.

To publish the generated site, configure GitHub SSH access for this computer and run `npm run deploy`. Hexo deploys the generated `public/` contents to the `main` branch.