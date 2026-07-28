# He Jian — Personal Homepage

Minimal personal page for OpenReview registration. Hosted free on GitHub Pages.

Final URL (after publishing): **https://hejian0818.github.io**

---

## ✏️ How to edit

Before publishing, you must set your real email (OpenReview requires the page
to show your name + email). Open `index.html` and find this line:

```html
<li><span class="label">Email</span> <a href="mailto:hejian@example.com">hejian@example.com</a></li>
```

Replace `hejian@example.com` (both the `mailto:` link and the visible text)
with the email you registered with on OpenReview.

---

## 🚀 How to publish (one-time, ~2 minutes)

You need a GitHub repo **named exactly** `hejian0818.github.io` (your username +
`.github.io`). Then any file pushed to it becomes live at the URL above.

### Option A — from the terminal (if you have `gh` CLI)

```bash
cd /Users/hejian/Desktop/openReview

git init
git add .
git commit -m "Initial personal homepage"

gh repo create hejian0818.github.io --public --source=. --push
```

If you don't have `gh`, install it: `brew install gh && gh auth login`.
(If `hejian0818.github.io` is taken on GitHub, use another username — the site URL
must match `<username>.github.io`.)

### Option B — from the browser

1. Go to https://github.com/new
2. Repository name: `hejian0818.github.io`
3. Set to **Public**, then **Create repository**
4. Upload `index.html` (drag it in), commit
5. Wait ~30s, open **https://hejian0818.github.io**

---

## 🔗 Fill into OpenReview

On OpenReview's "Personal Links" step, put the published URL in the
**Homepage URL** field:

```
https://hejian0818.github.io
```

Make sure it starts with `https://` (it does). The page shows your name
("He Jian") and your email, which satisfies OpenReview's verification.

---

## 📝 Expanding later (optional)

This is intentionally minimal. To add more later, edit `index.html`:

- Add a `<li>` under `.meta` for Institution / Scholar / ORCID / etc.
- Add sections (Bio, Research, Publications) with `<h2>` + `<p>`.
- Add a profile photo: drop a file like `photo.jpg` next to `index.html`
  and reference it with `<img src="photo.jpg" alt="He Jian" />`.
