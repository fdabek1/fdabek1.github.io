# filipdabek.me — personal resume site

Static site migrated from a private server to GitHub Pages (free hosting).

## Deploy
1. Create a repo named **fdabek1.github.io** on GitHub.
2. Upload all files in this folder to the repo root (the `CNAME` file sets the custom domain automatically).
3. In repo Settings → Pages, confirm the custom domain is `filipdabek.me` and turn on **Enforce HTTPS**.
4. At your domain registrar, point DNS at GitHub Pages:
   - Apex (`filipdabek.me`): A records → 185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153
   - `www`: CNAME → fdabek1.github.io

## Notes
- `.nojekyll` is required: the `_layout/` folder starts with an underscore and GitHub Pages would otherwise ignore it (breaking all CSS/JS).
- The contact form is a placeholder (`action="javascript:alert('success!');"`) — it never sent mail anywhere, so nothing is lost in the move.
- `prizetv` link returns HTTP 500 on the old server too — pre-existing broken link, left as-is.
