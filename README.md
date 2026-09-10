# Mareo — legal documents

The published Privacy Policy and Terms of Service for **Mareo**, a reminder and tracking app for
iOS. These are the pages the App Store listing points at.

They are served with GitHub Pages:

- https://minemuso.github.io/mareo-legal/privacy.html
- https://minemuso.github.io/mareo-legal/terms.html

## These files are generated — do not hand-edit them

`privacy.html` and `terms.html` are produced from the app's own copy by
`scripts/build-legal-mirrors.ts` in the application repository, and a test there fails if the
published text drifts from what the app shows on screen.

That indirection exists because of a real failure: the two were once maintained by hand, and while
the in-app policy was being rewritten the published one still carried months-old text. Editing a
file here would recreate exactly that gap — the app would say one thing and this page another, with
nothing to catch it.

So a change starts in the app, is regenerated there, and is copied here.

## Why this repository is separate

The application source is private. GitHub Pages will not serve a private repository on a free plan,
and these three files are meant to be public anyway — a privacy policy that cannot be read is not
serving its purpose. Nothing in this repository is secret: it contains no source code, no keys, and
no configuration.
