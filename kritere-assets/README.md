# KriTere theme images

Upload these files to Blogger, then in `kritere-blogger-theme.xml` replace each
`REPLACE_IMG_<name>` with the URL Blogger gives you for that file.

| Placeholder in the theme        | File                      | What it is |
|---------------------------------|---------------------------|------------|
| `REPLACE_IMG_kt-logo`           | `kt-logo.png`             | KT logo, also the mascot with moving eyes |
| `REPLACE_IMG_kritere-share`     | `kritere-share.jpg`       | 1200x630 picture shown when the site is shared on social networks |
| `REPLACE_IMG_dgm-icon`          | `dgm-icon.webp`           | Don't Get Mad! app icon |
| `REPLACE_IMG_dgm-trailer`       | `dgm-trailer.webp`        | Picture shown on the Don't Get Mad! trailer before it plays |
| `REPLACE_IMG_dgm-shot-1` ... `4`| `dgm-shot-1.webp` ... `4` | Don't Get Mad! posters |
| `REPLACE_IMG_dgm-marble`        | `dgm-marble.webp`         | White marble background of the Don't Get Mad! section |
| `REPLACE_IMG_kaj-icon`          | `kaj-icon.webp`           | Kris Ann's Journey app icon |
| `REPLACE_IMG_kaj-trailer`       | `kaj-trailer.webp`        | Picture shown on the Kris Ann's Journey trailer before it plays |
| `REPLACE_IMG_kaj-shot-1` ... `4`| `kaj-shot-1.webp` ... `4` | Kris Ann's Journey posters |
| `REPLACE_IMG_family-game-night` | `family-game-night.webp`  | Family photo from the Kris Ann's Journey trailer (Parents' corner) |

## Getting image URLs from Blogger

1. In Blogger, create a new post (keep it as a draft, never publish it).
2. Insert all the images above into it.
3. Switch the post editor to **HTML view** and copy each image's `src` URL
   (it starts with `https://blogger.googleusercontent.com/`).
4. Paste each URL over its placeholder in the theme.

If Blogger refuses a `.webp` file, convert it to `.jpg` first and upload that.

## The other placeholders

- `REPLACE_DGM_YOUTUBE_ID`, `REPLACE_KAJ_YOUTUBE_ID`: upload the two trailer videos to
  YouTube and paste the video id (the part after `watch?v=`).
- `REPLACE_DGM_WEB_URL`, `REPLACE_DGM_MS_STORE_URL`, `REPLACE_DGM_PLAY_STORE_URL` and the
  same three for `KAJ`: the web game, Microsoft Store and Google Play links.
- `REPLACE_YOUTUBE_URL`, `REPLACE_TIKTOK_URL`, `REPLACE_INSTAGRAM_URL`,
  `REPLACE_FACEBOOK_URL`, `REPLACE_THREADS_URL`, `REPLACE_X_URL`: your social profiles.

`kritere-preview.html` (next to this folder) shows the page with these images, so you can
open it in a browser to see the design before installing the theme.
