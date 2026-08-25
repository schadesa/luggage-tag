# luggage-tag

A single-page, mobile-first static website for a personal QR-code luggage tag.  
Hosted via GitHub Pages — no build tools required.

## Replacing the contact placeholders

Open `index.html` and replace the three placeholders (they appear twice each — once for the English card and once for the German card):

| Placeholder | Replace with |
|---|---|
| `+43XXXXXXXXX` in `href="tel:+43XXXXXXXXX"` | Your international phone number, e.g. `+43 699 12345678` |
| `43XXXXXXXXX` in `href="https://wa.me/43XXXXXXXXX"` | Your WhatsApp number **without** the leading `+` and without spaces, e.g. `436991234567` |
| `placeholder@example.com` in `href="mailto:placeholder@example.com"` | Your email address |

Search for the comment lines starting with `<!-- PLACEHOLDER:` to find every spot quickly.

## Previewing locally

```bash
# Python 3
python3 -m http.server 8080
# then open http://localhost:8080 in your browser
```

Or just open `index.html` directly in a browser (all assets are local — no server needed).

## Publishing with GitHub Pages

1. Push the repository to GitHub (`main` branch).
2. Go to **Settings → Pages** in the repository.
3. Under **Source**, select **Deploy from a branch**.
4. Choose branch `main` and folder `/ (root)`, then click **Save**.
5. After a minute or two the page will be live at:  
   `https://<your-github-username>.github.io/luggage-tag/`

## Updating the page

Edit `index.html` or `style.css`, commit, and push.  
GitHub Pages rebuilds automatically within a minute.
