AKOREDE Favicon Pack - transparent background
================================================

Background fully removed (true alpha transparency, verified against a
checkerboard test) -- just the chrome "A" mark, no black square.

Files:
- favicon.ico                       -> site root (16/32 multi-res)
- favicon-16x16.png
- favicon-32x32.png
- apple-touch-icon.png (180x180)
- android-chrome-192x192.png
- android-chrome-512x512.png
- site.webmanifest

<head> snippet:

<link rel="icon" type="image/x-icon" href="/favicon.ico">
<link rel="icon" type="image/png" sizes="32x32" href="/favicon-32x32.png">
<link rel="icon" type="image/png" sizes="16x16" href="/favicon-16x16.png">
<link rel="apple-touch-icon" sizes="180x180" href="/apple-touch-icon.png">
<link rel="manifest" href="/site.webmanifest">

Note: browsers still render a light backdrop behind transparent favicons in
light-theme tab bars -- that's normal browser chrome, not a black square
baked into the image.
