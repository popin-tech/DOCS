# Popin media spec

Reference: www.vogue.co.uk
**Images used in Rogue**

## Tech

* Lovell\Sharp - image editing capabilities \ resizing
* DigitalOcean\AWS - SDK for uploading

## Manipulation:

* Exif orientation
* Resizing on upload

## Size

* 200
* 400
* 600
* 900
* 1200

## Orientation:

* Square
* Landscape
* Portrait
* Thumbnail

## Naming Conventions

**Popin**
_Images uploaded by us (Popin) have multiple sizes_
`/image/{uniqueId}/crop/{size}/{orientation}`

**Space**
`/image/{uniqueId}/crop/{size}/{orientation}`

`/video360/{uniqueId}`

`/video/`

**Brand**
_Images uploaded by Brands will be fixed to the prefixes below_
`/image/{uniqueId}/crop/200/thumbnail.jpg`

`/image/{uniqueId}/crop/600/square.jpg`

**TODO:**

* Generation of uniqueIds

## Models Using Images:

* Spaces
  * Avatar (Thumbnails)
  * Shop Front
* Brand
  * Avatar (Thumbnails)
* Areas
  * Images
* Products
  * Images

## Examples

VOGUE (_preferred choice_)

* _Square example_

```
<img src="https://vg-images.condecdn.net/image/YBYYjlvnA8m/crop/200/square"
    data-src="https://vg-images.condecdn.net/image/YBYYjlvnA8m/crop/200/square"
    data-srcset="https://vg-images.condecdn.net/image/YBYYjlvnA8m/crop/200/square 200w,
                 https://vg-images.condecdn.net/image/YBYYjlvnA8m/crop/300/square 300w,
                 https://vg-images.condecdn.net/image/YBYYjlvnA8m/crop/400/square 400w,
                 https://vg-images.condecdn.net/image/YBYYjlvnA8m/crop/600/square 600w,
                 https://vg-images.condecdn.net/image/YBYYjlvnA8m/crop/900/square 900w"
    data-sizes="auto"
    class="global__image lazyautosizes img-lazyload--loaded"
    sizes="330px"
    srcset="https://vg-images.condecdn.net/image/YBYYjlvnA8m/crop/200/square 200w,
            https://vg-images.condecdn.net/image/YBYYjlvnA8m/crop/300/square 300w,
            https://vg-images.condecdn.net/image/YBYYjlvnA8m/crop/400/square 400w,
            https://vg-images.condecdn.net/image/YBYYjlvnA8m/crop/600/square 600w,
            https://vg-images.condecdn.net/image/YBYYjlvnA8m/crop/900/square 900w">
```

* _Landscape example_

```
<img src="https://vg-images.condecdn.net/image/eyqqb7oJPWd/crop/405/landscape"
    data-src="https://vg-images.condecdn.net/image/eyqqb7oJPWd/crop/405/landscape"
    data-srcset="https://vg-images.condecdn.net/image/eyqqb7oJPWd/crop/405/landscape 405w,
                 https://vg-images.condecdn.net/image/eyqqb7oJPWd/crop/810/landscape 810w,
                 https://vg-images.condecdn.net/image/eyqqb7oJPWd/crop/1020/landscape 1020w,
                 https://vg-images.condecdn.net/image/eyqqb7oJPWd/crop/1440/landscape 1440w,
                 https://vg-images.condecdn.net/image/eyqqb7oJPWd/crop/1620/landscape 1620w" data-sizes="auto" class="global__image lazyautosizes img-lazyload--loaded"
    sizes="1440px"
    srcset="https://vg-images.condecdn.net/image/eyqqb7oJPWd/crop/405/landscape 405w,
            https://vg-images.condecdn.net/image/eyqqb7oJPWd/crop/810/landscape 810w,
            https://vg-images.condecdn.net/image/eyqqb7oJPWd/crop/1020/landscape 1020w,
            https://vg-images.condecdn.net/image/eyqqb7oJPWd/crop/1440/landscape 1440w,
            https://vg-images.condecdn.net/image/eyqqb7oJPWd/crop/1620/landscape 1620w">
```

_INSTAGRAM_

```
<img class="_2di5p" style="" sizes="614px"
    srcset="https://scontent-lht6-1.cdninstagram.com/t51.2885-15/e35/25009010_201324713772933_4663507461733351424_n.jpg 640w,
            https://scontent-lht6-1.cdninstagram.com/t51.2885-15/e35/25009010_201324713772933_4663507461733351424_n.jpg 750w,
            https://scontent-lht6-1.cdninstagram.com/t51.2885-15/e35/25009010_201324713772933_4663507461733351424_n.jpg 1080w"
    src="https://scontent-lht6-1.cdninstagram.com/t51.2885-15/e35/25009010_201324713772933_4663507461733351424_n.jpg">
```

_GUARDIAN_

```
<picture>
    <!--[if IE 9]><video style="display: none;"><![endif]-->
    <source media="(min-width: 980px) and (-webkit-min-device-pixel-ratio: 1.25), (min-width: 980px) and (min-resolution: 120dpi)"
        sizes="220px"
        srcset="https://i.guim.co.uk/img/media/fb8d0e1b7ccfd6927271947cd34e1e8a6319784f/226_246_1342_804/master/1342.jpg?w=220&amp;q=20&amp;auto=format&amp;usm=12&amp;fit=max&amp;dpr=2&amp;s=d79b39c0ca64c63cecf06c27cb71c266 440w">
    <source media="(min-width: 980px)"
        sizes="220px"
        srcset="https://i.guim.co.uk/img/media/fb8d0e1b7ccfd6927271947cd34e1e8a6319784f/226_246_1342_804/master/1342.jpg?w=220&amp;q=55&amp;auto=format&amp;usm=12&amp;fit=max&amp;s=fc69956e73dba77458761bddff356068 220w">
    <source media="(min-width: 740px) and (-webkit-min-device-pixel-ratio: 1.25), (min-width: 740px) and (min-resolution: 120dpi)"
        sizes="160px"
        srcset="https://i.guim.co.uk/img/media/fb8d0e1b7ccfd6927271947cd34e1e8a6319784f/226_246_1342_804/master/1342.jpg?w=160&amp;q=20&amp;auto=format&amp;usm=12&amp;fit=max&amp;dpr=2&amp;s=24d52826af4eca1c0917cd126bc76c6c 320w">
    <source media="(min-width: 740px)"
        sizes="160px"
        srcset="https://i.guim.co.uk/img/media/fb8d0e1b7ccfd6927271947cd34e1e8a6319784f/226_246_1342_804/master/1342.jpg?w=160&amp;q=55&amp;auto=format&amp;usm=12&amp;fit=max&amp;s=699c2503922b3efada1820fc6bf19594 160w">
    <source media="(min-width: 0px) and (-webkit-min-device-pixel-ratio: 1.25), (min-width: 0px) and (min-resolution: 120dpi)"
        sizes="127px"
        srcset="https://i.guim.co.uk/img/media/fb8d0e1b7ccfd6927271947cd34e1e8a6319784f/226_246_1342_804/master/1342.jpg?w=127&amp;q=20&amp;auto=format&amp;usm=12&amp;fit=max&amp;dpr=2&amp;s=bee46483364974ad19e2ad647249b7c3 254w">
    <source media="(min-width: 0px)"
        sizes="127px"
        srcset="https://i.guim.co.uk/img/media/fb8d0e1b7ccfd6927271947cd34e1e8a6319784f/226_246_1342_804/master/1342.jpg?w=127&amp;q=55&amp;auto=format&amp;usm=12&amp;fit=max&amp;s=9531cb9b625808422b6a7ac17be898be 127w">
    <!--[if IE 9]></video><![endif]-->
    <img class="responsive-img" alt="" src="https://i.guim.co.uk/img/media/fb8d0e1b7ccfd6927271947cd34e1e8a6319784f/226_246_1342_804/master/1342.jpg?w=300&amp;q=55&amp;auto=format&amp;usm=12&amp;fit=max&amp;s=aa6821d747a8c4f29bcf24215c0706f0">
</picture>
```
