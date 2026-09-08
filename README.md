# pixelfishing.io

The website for [Pixel Fishing](https://github.com/Pixel-Fishing/pixel-fishing-app),
a Discord fishing game. Plain HTML and one stylesheet: no build step, nothing to
install, nothing to break.

Pushing to `main` publishes it. GitHub Pages serves the repository as-is.

    index.html     the landing page
    privacy.html   required by Discord before the app can be listed
    terms.html     likewise
    style.css      shared by all three
    img/           listing images — see img/README.md
    CNAME          the custom domain; do not delete it

## Images

Drop a file in `img/` and it is live at `https://pixelfishing.io/img/<filename>`
as soon as it is pushed. That URL is what Top.gg's description needs; Discord's
App Directory takes uploads directly and does not.

## The policy pages

`privacy.html` and `terms.html` were written against what the bot actually
stores, and they need to stay true to it. If the schema gains a column that
holds something about a player, the privacy page needs a line about it.
