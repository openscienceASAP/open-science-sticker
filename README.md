Open Science Goodies
====================

Repository with "blue prints" for Open Science goodies.

License
-------

[CC BY 4.0 International](http://creativecommons.org/licenses/by/4.0/)

Used Software
-------------

-   [Inkscape](https://inkscape.org/)

    Used to create the SVG files.
-   [ImageMagick](http://imagemagick.org/)

    Used to convert the SVG files to bitmaps formats
    (**not stored in the Git repository**).

Used Content
------------

-   [okfn.org Webarchive](http://www.google.de/imgres?imgurl=http%3A%2F%2Fwebarchive.okfn.org%2Fokfn.org%2F201404%2Fwp-content%2Fuploads%2F2013%2F11%2Fopenscience-sticker.png&imgrefurl=http%3A%2F%2Fwebarchive.okfn.org%2Fokfn.org%2F201404%2Fmedia%2F&h=72&w=329&tbnid=ucA4njWK5xtSzM%3A&zoom=1&docid=-ThchW7j-sAwnM&ei=NmyZVJLJLIzEPPeLgZgJ&tbm=isch&client=ubuntu&iact=rc&uact=3&dur=208&page=1&start=0&ndsp=48&ved=0CG0QrQMwFg)

    Open Science sticker ([pdf](http://webarchive.okfn.org/okfn.org/201404/assets.okfn.org/p/okfn/media/open-science.pdf)) under [CC BY 3.0 unported](http://creativecommons.org/licenses/by/3.0/)
-   [okfn Google Driver](https://drive.google.com/?tab=mo&pli=1&authuser=0#folders/0ByBC-sFwdwtJU3BObG9UX1V4alk)

    New Logos.

Structure
---------

-   [README.md](README.md)

    Overview of repository.
-   `raw/`

    The raw archive provide by OKF or third party if not in SVG.
-   `svg/`

    SVG files used to create the bitmaps. **Is your start point if you want to
    customize some goodie.**
-   [svg2bitmap](svg2bitmap)

    Shell script to convert the SVG into bitmap.

SVG Files
---------

**This files are a very good start point for you create your stickers.**

-   [badge.svg](badge.svg)

    Badge that you can use in the footnote of your website.
-   [badge-sticker.svg](badge-sticker.svg)

    Badge to be print as stickers.
-   [graphic.svg](graphic.svg)

    The symbol of the OKF Open Science Working Group.
-   [icon.svg](icon.svg)

    The icon of the OKF Open Science Working Group.
-   [icon-sticker.svg](icon-sticker.svg)

    The icon to be print as 5x5 stickers.
-   [icon-black.svg](icon-black.svg)

    The black version of the icon.
-   [icon-white.svg](icon-white.svg)

    The white version of the icon.
-   [logo.svg](logo.svg)

    The logo of the OKF Open Science Working Group.
-   [logo-black.svg](logo-black.svg)

    The black version of the logo.
-   [logo-white.svg](logo-white.svg)

    The white version of the logo.

FAQ
---

-   How can I change the background of JPG files?

    Replace

    ~~~
    INPUT_OPTIONS="-background none"
    ~~~

    with

    ~~~
    INPUT_OPTIONS="-background color"
    ~~~

    at [svg2bitmap](svg2bitmap), where `color` is the name of the color you want
    (e.g. `white`).
-   How can I set the width of the PNG/JPG files?

    **You should avoid this because the output will have bad quality.**

    Replace

    ~~~
    OUTPUT_OPTIONS=""
    ~~~

    with

    ~~~
    OUTPUT_OPTIONS="-resize 100"
    ~~~

    at [svg2bitmap](svg2bitmap), where `100` is the width that you want.
-   How can I set the height of the PNG/JPG files?

    **You should avoid this because the output will have bad quality.**

    Replace

    ~~~
    OUTPUT_OPTIONS=""
    ~~~

    with

    ~~~
    OUTPUT_OPTIONS="-resize x100"
    ~~~

    at [svg2bitmap](svg2bitmap), where `100` is the height that you want.
