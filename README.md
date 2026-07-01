# G. Brock Williams — Personal Website

## Files

```
williams-site/
├── index.html          the page itself
├── css/
│   └── style.css       all visual styling
└── images/
    ├── williams.jpeg   your photo (intro section)
    ├── image_2.jpg     service card image
    └── SchoenbergZ.png grants card image
```

Copy your three images from the TTU server into the images/ folder.
Everything else is already here.

---

## How to edit

Open index.html in Emacs.  The HTML is divided into named sections with
comments like:

    <!-- RESEARCH CARD -->

Find the section you want, change the text between the tags, save.

To change your photo, replace images/williams.jpeg with a new file
(same name, or update the src="..." attribute in the HTML).

Open css/style.css to change colors, fonts, or spacing.  The color
palette is listed at the top of that file.

---

## How to put it on GitHub Pages (free hosting)

1. Install git if you don't have it:  https://git-scm.com

2. Create a free account at https://github.com

3. On GitHub, click the + button → New repository.
   Name it:  williams-website   (or anything you like)
   Set it to Public.  Click Create repository.

4. In your terminal, in this folder:

       git init
       git add .
       git commit -m "Initial version"
       git branch -M main
       git remote add origin https://github.com/YOUR_USERNAME/williams-website.git
       git push -u origin main

5. On GitHub, go to your repository → Settings → Pages.
   Under "Source," select:  Deploy from a branch → main → / (root)
   Click Save.

6. After about 60 seconds, your site is live at:
       https://YOUR_USERNAME.github.io/williams-website/

---

## How to update later

Make changes to index.html or style.css in Emacs, then:

    git add .
    git commit -m "brief description of what you changed"
    git push

GitHub Pages updates automatically within a minute or two.

---

## Optional: custom domain

If you want a URL like  brock-williams.com  instead of github.io:
  - Buy a domain at namecheap.com or porkbun.com (~$10/year)
  - GitHub Pages lets you point any custom domain to your site for free
  - Instructions: https://docs.github.com/pages/configuring-a-custom-domain-for-your-github-pages-site
