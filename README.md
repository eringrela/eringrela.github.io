# Academic website — James-style layout, without divider lines

This is a simple standalone HTML/CSS website with the key features of James Okun's public academic website: a fixed left sidebar containing your name, headshot, short bio, and links; research sections on the right; blue paper-title links; and expandable abstracts. **All horizontal rules and borders between papers/sections have been omitted.** The HTML/CSS was written independently, so you do **not** need to fork or download his GitHub repository.

## Look at it

Double-click `index.html` to open the website in your browser. No installation required.

## Replace before publishing

1. In `index.html`, replace **Your Name**, the placeholder intro, and the email. Edit the `<title>` and description in the `<head>`.
2. Add a real headshot to `assets/`, e.g. `headshot.jpg`. Replace `assets/portrait-placeholder.svg` with `assets/headshot.jpg` in `index.html` and change the alt text.
3. Add your CV as `files/cv.pdf` (create `files/` if needed). Change the CV placeholder `<span>` into `<a href="files/cv.pdf">CV</a>`.
4. Change the Google Scholar / GitHub placeholder links to your own URLs. Remove any links you don't want.
5. Edit all paper titles, descriptions, and abstracts. They're illustrative working-title examples, **not** verified publication titles or official abstracts. Add your real publications in place of the sample entry.
6. Add PDFs by placing them in a `files/` folder. Turn any paper title into a link, e.g. `<a href="files/my-paper.pdf">My Paper Title</a>`.
7. To change the blue accent subtly, edit `--link` in `styles.css`. To change space between papers, edit `.paper { margin: ... }`.

## Publish without a fork

1. Create a new public repository on GitHub named `YOUR-USERNAME.github.io`.
2. Upload **the contents of this folder** (not the parent folder) to the repository root.
3. In the repository, choose **Settings → Pages → Build and deployment → Deploy from a branch**, select `main` and `/(root)`, then Save.
4. The published site will be at `https://YOUR-USERNAME.github.io` after deployment.
5. Optionally add a custom domain later in Settings → Pages and configure the registrar's DNS.

Guide: https://docs.github.com/en/pages/quickstart

## Optional Claude Code prompt

> Use this existing starter site. Keep the James Okun-style two-column layout: fixed left column for photo, name, bio, links; right column for research, normal-weight headings, compact paper entries, blue links, and expandable abstracts. Do not add horizontal rules, lines, cards, background blocks, or section borders. Customize the content using only the data I supply. Do not fabricate publications, coauthors, statuses, or PDFs. Preserve mobile responsiveness.
