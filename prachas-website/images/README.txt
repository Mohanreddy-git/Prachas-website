IMAGES FOLDER
=============

The site currently uses CSS gradients and inline SVG icons so it is fully
self-contained (no external image downloads required).

To use the real Prachas branding and photography, drop the asset files here
and reference them in the HTML. Suggested files:

  logo.png / logo.svg   -> replace the "P" gradient logo in the header/footer
  hero.jpg              -> background or side image for the home hero
  about.jpg            -> image for the About page "split" media block
  og-image.jpg         -> social share preview (1200x630)
  favicon.ico          -> browser tab icon

Example — replacing the header logo (in each .html file):

  <a href="index.html" class="brand">
    <img src="images/logo.svg" alt="Prachas Technologies" height="40">
  </a>

Example — adding a favicon (inside <head> of each page):

  <link rel="icon" href="images/favicon.ico">

You can grab the original images from the live site (prachas.com) by saving
them from the page, or export them from the GoDaddy editor's media library.
