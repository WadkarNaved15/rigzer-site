RIGZER SITE: how to put it on your domain
==========================================

WHAT THIS IS
A plain static website. No build step, no database, no server code.
  index.html      the page (open this first; it must be the home page of your domain)
  playshelf.html  the Game Shelf, shown inside the page
  radio.html      Rigzer Radio, shown inside the page
  rd/             images and short looping videos used by the Radio
  *.webp / *.mp4  pictures and the hero video used by the page itself

HOW TO PUBLISH
1. Upload the CONTENTS of this folder (not the folder itself) to the root of your hosting,
   so that  yourdomain.com/index.html  and  yourdomain.com/rd/seq-1.mp4  both work.
   - Shared hosting / cPanel: File Manager -> public_html -> upload and extract the zip there.
   - Netlify / Cloudflare Pages / Vercel / GitHub Pages: drag this folder in (or connect the repo)
     and point your domain at it in the project's "Domains" settings.
2. Point the domain at the host (the host shows you the exact DNS records; usually an A record or a CNAME).
3. Turn on HTTPS (free on every host listed above).

KEEP THESE FILES TOGETHER
All paths are relative, so the files must stay in the same folders as they are here.
The page also loads two fonts from Google Fonts, so visitors need an internet connection (normal).

OPTIONAL, FOR SPEED
Ask the host to cache images and videos for a long time and to serve with gzip/brotli (most do by default).
