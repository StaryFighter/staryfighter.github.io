# zolomon-kaliser.com

Personal portfolio site for Zolomon Kaliser. Static HTML hosted on GitHub Pages.

## Structure

    index.html          Single-page portfolio (About, Education, Experience,
                        Research, Projects, Skills, Certifications, Contact)
    404.html            Not-found page
    portfolio.html      Redirect -> /   (old portfolio URL)
    research.html       Redirect -> /#research
    intake.html         Redirect -> /   (retired consulting page)
    legal.html          Redirect -> /   (retired consulting page)
    resume.pdf          Downloadable resume, linked from the nav and contact panel

    assets/site.css     Design tokens, layout, and every component
    assets/site.js      Nav shrink, mobile menu, scroll reveal, smooth anchors
    assets/headshot-zolomon.jpg
    assets/img/         Research project imagery
    assets/logos/       University and employer logos

    CNAME               Custom domain (zolomon-kaliser.com)
    .nojekyll           Serve files as-is on GitHub Pages
    favicon.*, apple-touch-icon.png, og-image.png

## Editing

Content is plain HTML in `index.html`, in document order matching the nav.
Colors, fonts, and spacing are CSS custom properties at the top of
`assets/site.css` — change a token there and it applies site-wide.

To add a work experience entry, copy an existing `.exp-item` block in the
`#experience` section. Use `<img>` inside `.exp-mark` when a logo exists,
or `<span class="initials">` as a fallback.

The site is fully readable with JavaScript disabled; GSAP only adds the
scroll-reveal animation.

## Deploying

Push to the default branch. GitHub Pages serves the site at the domain in
`CNAME`.
