# Casey Glick — personal site

A plain static website. No build step, no framework, no database — just HTML and
one CSS file. That means it's fast, it can't really be "hacked" in the way people
worry about (there's no server-side code to exploit), and you can host it free on
GitHub Pages.

---

## What's here

```
index.html            About / bio (home page)
cv.html               Curriculum vitae  (+ link to a CV PDF)
publications.html     Publications, patents, thesis (+ PDF links)
blog.html             "Writing" index — lists your posts
posts/                Individual blog posts (one HTML file each)
music.html            Compositions — UNLISTED (noindex, not in the nav)
creative-writing.html Poetry/prose — UNLISTED (noindex, not in the nav)
assets/styles.css     All the styling, in one file
files/                Put PDFs, audio, etc. here to host them
robots.txt, 404.html, .nojekyll   Housekeeping — leave them alone
```

The two unlisted pages are the "hobby" areas. They carry a `noindex` tag and are
not linked from any public page, so they won't appear when someone googles your
name — but anyone you hand the direct link to sees them instantly. That's the
"not front-and-center" you wanted; it is *not* a password, and it isn't meant to
be one.

---

## Publishing it (no Git commands)

1. Make a free account at **github.com** if you don't have one.
2. Create a new repository named **`yourusername.github.io`** (use your actual
   GitHub username). Make it **Public**. Don't add a README when prompted.
3. On the new repo's page, click **“uploading an existing file.”**
4. Drag **the contents of this folder** (all the files and the `posts/`,
   `assets/`, `files/` folders) into the browser window. Wait for them to finish.
5. Scroll down, click **“Commit changes.”**
6. Your site is live in a minute or two at **`https://yourusername.github.io`**.

To update it later: go to the repo, open the file you want to change, click the
pencil ✏️ icon, edit, and click **Commit changes.** Or drag a new version of a
file in the same way. You never touch the command line.

> Why this is safe: GitHub only serves these files as-is. Protect your **GitHub
> account** (turn on two-factor authentication) — that's the real front door.

### A custom domain (optional)
If you buy a domain (e.g. `caseyglick.com`), GitHub Pages → repo **Settings →
Pages → Custom domain** walks you through it. Not required; the
`github.io` address works fine.

---

## Editing content — the common tasks

**Change text (bio, CV, etc.):** open the `.html` file, find the words, change
them. The comments marked `<!-- EDIT ... -->` point out the spots most worth
customizing (your email, current role, etc.).

**Host your CV or thesis PDF:** put the PDF in the `files/` folder. The CV page
already links to `files/Glick_Casey_CV.pdf` and the publications page to
`files/Glick_thesis_2017.pdf` — name your files to match, or change the link.

**Add a blog post:** copy `posts/2026-01-15-example-post.html` to a new file,
edit the title/date/body, then add one line linking to it near the top of the
list in `blog.html`.

**Add a composition or poem:** edit `music.html` / `creative-writing.html`. Each
has commented examples for linking out (MuseScore, Bandcamp), embedding a player,
or hosting an audio/PDF file directly from `files/`.

**The resiliency amendments (later):** when they're ready, the simplest path is a
new `resiliency.html` — copy any existing page as a template. Decide then whether
it's public (add it to the nav) or unlisted (copy the `noindex` line from
`music.html` and leave it out of the nav), same mechanism as the hobby pages.

---

## One honest note on hosting papers

- **Your thesis:** you almost certainly own the copyright to your own
  dissertation — host it freely.
- **Journal papers:** the publisher usually holds copyright to the *final typeset
  PDF*, but nearly all publishers explicitly let you host the **preprint** or the
  **accepted manuscript** (your own formatted version, pre-typesetting). That's
  what academics post, and it's fully allowed. Check a journal's policy in
  ~30 seconds at **Sherpa Romeo** (open-access.network/sherpa-romeo). Posting the
  accepted manuscript gets you the same result as the publisher PDF with none of
  the risk — so there's rarely a reason to post the publisher's version.
- Conference proceedings and patents: patents are public record; proceedings vary,
  but the preprint rule above is the safe default.

I'm not a lawyer — but the preprint/accepted-manuscript route is the standard,
low-friction way to do this legitimately.
