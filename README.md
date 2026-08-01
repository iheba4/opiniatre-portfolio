# Opiniâtre portfolio

The portfolio site for Opiniâtre, a poster series I design and sell. Seventeen works, each with a full resolution plate, a mid size view, a mockup in a room, and a thumbnail.

## Why it is built this way

There is no framework and no build step. The whole site is one HTML file, one JSON file, and a folder of images. Open `index.html` and it works, from a local disk or from any static host.

That is a deliberate choice rather than a limitation. A portfolio has to still work in three years when I have forgotten how it was made, and the fastest way to guarantee that is to have nothing that can rot. There is no dependency to update and no toolchain to reinstall.

## Adding a work

Everything the gallery renders comes from `works.json`. Each entry carries the title, the year, the description and the paths to its four image sizes. Add the images, add the entry, reload. No rebuild.

The four sizes exist because they do different jobs. Thumbnails load the grid fast. The mid size is what you see when you open a piece. The full plate is what a print buyer wants to look at closely. The mockup is what makes someone imagine it on their own wall, which is the one that actually sells.

## Layout

    index.html        the whole site
    works.json        the catalogue the gallery is built from
    assets/posters/   full resolution plates
    assets/mid/       mid size views
    assets/mockups/   framed in a room
    assets/thumbs/    grid thumbnails
    assets/meta.json  per work metadata

## The work itself

The posters are typographic and mostly monochrome, built around a single idea per plate. Opiniâtre means stubborn, which is roughly the working method.

All poster artwork in this repository is my own and is not licensed for reuse. The MIT licence covers the site code.
