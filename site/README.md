# Multiscapes Group Website

## Folder contents
- `index.html` — the whole website (one page)
- `images/` — every photo and the logo, named by what they show

## Updating content later
Open `index.html` in any text editor (VS Code, Notepad++, even Notepad). Search (Ctrl+F) for the
text you want to change — e.g. search "WhatsApp Us" or "0434 294 451" — and edit it directly.

## Swapping a photo
1. Drop your new photo into the `images/` folder.
2. In `index.html`, search for the filename of the photo you're replacing
   (e.g. "slide-gazebo-installation.jpg") and replace it with your new filename.
3. Keep photos under ~500KB each so the site stays fast — resize/export at "web quality"
   before adding them.

## Adding a new photo to the homepage slideshow
Find the `const SLIDES = [` block near the bottom of `index.html`. Add a new line like:
```
{src: "images/your-new-photo.jpg", label: "Your Caption Here"},
```

## Adding a new photo to the gallery section
Find the `const galleryItems = [` block. Add a new line like:
```
{src: SLIDES[N].src, label: SLIDES[N].label},
```
replacing N with the position of the photo in the SLIDES list above (counting from 0).
