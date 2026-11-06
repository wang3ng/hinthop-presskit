# Press assets

This folder is the drop zone for Hint Hop media. **No trailer, capsules, screenshots, or zip are in the repo yet.** Do not commit stand-in images. Add the real files, then link them from `../index.html` (a commented example sits in the Media section).

GitHub blocks files over 100 MB. If `hint-hop-press-assets.zip` is larger than that, host the zip somewhere else and paste that URL into the Media section instead of committing the file.

Suggested layout, using current Steamworks sizes ([store graphical assets](https://partner.steamgames.com/doc/store/assets/standard), [library assets](https://partner.steamgames.com/doc/store/assets/libraryassets)):

```
assets/
  trailer.mp4                         optional; a YouTube link is enough
  hint-hop-press-assets.zip           zip of the images below
  logo.png                            transparent logotype, if you have one
  capsules/
    header_920x430.png                required on Steam, 920×430
    small_462x174.png                 required on Steam, 462×174
    main_1232x706.png                 required on Steam, 1232×706
    vertical_748x896.png              required on Steam, 748×896
    page_background_1438x810.png      optional, 1438×810
  library/
    capsule_600x900.png               600×900
    header_920x430.png                920×430
    hero_3840x1240.png                3840×1240, no text
    logo.png                          transparent; 1280 px wide and/or 720 px tall
  screenshots/
    01-board.png                      1920×1080 or larger, 16:9
    02-hint.png
    03-lobby.png
```

PNG or JPG. Name screenshots so the order is obvious (`01-`, `02-`, …).

After the files exist, uncomment and edit the examples in `docs/presskit/index.html`:

```html
<p><a href="assets/hint-hop-press-assets.zip">Download all press assets (.zip)</a></p>
<video controls src="assets/trailer.mp4"></video>
<a href="assets/screenshots/01-board.png">
  <img src="assets/screenshots/01-board.png" alt="The two-axis word grid during a hint." width="960">
</a>
```

A public trailer can stay on YouTube instead of in git. The channel is <https://www.youtube.com/@PlayHintHop>. When a specific video is public, add its URL next to the trailer line on the press page.

The zip should contain the same capsules, library art, logo, and screenshots, with no extra executables.
