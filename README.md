# drlafave.github.io

Personal academic website for Dan LaFave (Colby College), served by GitHub Pages at https://drlafave.github.io.

Plain HTML, no build step:

- `index.html` – home page (bio, recent papers)
- `research.html` – working papers and publications
- `teaching.html` – courses and syllabi
- `style.css` – all styling (light and dark mode)
- `files/` – paper and syllabus PDFs
- `.github/workflows/deploy.yml` – publishes the site; pulls the CV from Dropbox on every push and once a day
- `images/` – headshot

To add a paper, copy an existing `<li>` block in `research.html`, edit it, drop the PDF in `files/`, then commit and push. The site updates within a minute or two.

## CV

The CV lives in Dropbox (`CV_lafave.pdf`). The deploy workflow downloads it and serves it from `files/CV_lafave.pdf`, so browsers open it normally. After updating the CV in Dropbox, it appears on the site within a day, or immediately if you click **Actions → Deploy site → Run workflow** on GitHub (or run `gh workflow run deploy.yml`).
