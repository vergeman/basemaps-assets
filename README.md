# basemaps-assets
Fonts and sprites for [basemaps](https://github.com/protomaps/basemaps).

## Deploy Notes

Currently deployed on CF pages. Issue with syncing via git, so deploying via zip
file and direct upload

Make sure to exclude `.git`, `.github` directories.

## Directory Structure

* `fonts/`: Contains PBF glyphs generated by [font-maker](https://github.com/maplibre/font-maker)
  * Current fonts: `Noto Sans Regular`, `Noto Sans Medium`, `Noto Sans Italic`, `Font Awesome 6 Free Regular`
  * `Font Awesome 6 Free Regular` sources:
    * https://use.fontawesome.com/releases/v6.5.2/fontawesome-free-6.5.2-web.zip
    * send `webfonts/*.ttf` to [Font Maker App](https://maplibre.org/font-maker/) to generate pbfs.
 
* `sprites/v3`: Contains spritesheets generated by [spreet](https://github.com/flother/spreet), for each major version
  * `light@x.png` - light and dark themed spritesheets at 1x and 2x pixel densities

## Fonts

The typefaces and font variants hosted and downloadable here are limited to only those used by [basemaps](https://github.com/protomaps/basemaps) and a Noto Sans alternate. It is not meant to include all possible variations or other fonts. If you want to generate fonts for your own use, use the examples in `scripts` and maintain your own repository.

## Linking to Assets in Styles

```
glyphs:'https://<domain>/basemaps-assets/fonts/{fontstack}/{range}.pbf'
```

## Downloading Assets

Use the Downloads button on this repository page.

## License

The license for each group of assets is contained within that directory:

* `fonts/`: [SIL Open Font License](fonts/OFL.txt)
