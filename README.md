# CLAIRIFY.CA — Static Site

This folder is a complete, ready-to-deploy static website: two HTML pages, one shared
stylesheet, and two images. No build step, no dependencies, no backend.

## Structure

```
index.html          Home page
about.html           About page
css/styles.css        Shared styles for both pages
images/logo.jpg        Nav wordmark
images/headshot.jpg     Claire's headshot (About page)
```

## Local preview

Just open index.html in a browser. Everything is relative paths, so it works
straight off disk with no server needed for a quick look.

## Deploying with GitHub + Cloudflare Pages

See the setup walkthrough provided separately for full step-by-step instructions.
Short version:

1. Push this folder to a new GitHub repository.
2. In Cloudflare Pages, create a project connected to that repo.
   Framework preset: None. Build command: (leave blank). Output directory: /
3. Deploy. Cloudflare gives you a *.pages.dev URL immediately.
4. Point clairify.ca at Cloudflare (nameservers or CNAME), then attach the
   custom domain to the Pages project.
