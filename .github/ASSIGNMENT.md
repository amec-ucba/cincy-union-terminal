# 📄 Cincinnati Union Terminal

## 🎯 Overview

Style a two-page guide to Cincinnati Union Terminal on your own, and show what you've learned
about CSS, typography, and media.

Union Terminal opened in 1933 as Cincinnati's train station. Its giant Art Deco arch and gold
rotunda make it one of the most recognizable buildings in the city, and today it's home to
Cincinnati Museum Center. The HTML for two pages is already written:

- **Home** (`index.html`), with a hero, the history of the building, a rotunda photo, and a
  1940s film clip
- **Visit** (`visit.html`), with hours, the museums inside, and how to get there

Your job is to finish three marked spots in the HTML, then write **all** of the CSS in
`css/styles.css` so both pages look like they belong to an Art Deco landmark.

This is an **independent** assignment. There is no follow-along video. After you submit, a
walkthrough video unlocks in Canvas so you can compare your work with mine.

### 🧠 What You'll Show

- Load a pair of Google Fonts and give every font a fallback
- Build a type scale in `rem`, with readable line height and line length
- Use the box model to space things consistently, and center a content column
- Put text over a `background-image` and keep it readable with an overlay
- Float an image so text wraps around it, and clear the float
- Serve the right size of image with `srcset` and `sizes`
- Add a video with a poster, more than one source, and captions

## 📋 Requirements

### HTML: the three TODOs

Change only the spots marked with a `TODO` comment. Don't change the rest of the HTML.

**Fonts** (both pages)

- [ ] In the `head` of both pages, add the Google Fonts `link` elements for your two fonts,
      **above** the link to `styles.css`

**Rotunda image** (`index.html`)

- [ ] An `img` of the rotunda, using `images/rotunda-800.webp` as its `src`
- [ ] A `srcset` that lists all four rotunda files with their widths (`480w`, `800w`, `1200w`,
      `1600w`)
- [ ] A `sizes` attribute. The photo fills the width of the screen on a phone, so `sizes="100vw"`
      works, as in the Week 6 lecture
- [ ] `width` and `height` attributes (the original is 1600 × 1200), `alt` text that describes
      the rotunda, and `loading="lazy"`

**Captioned video** (`index.html`)

- [ ] A `video` with `controls` and the poster `media/union-terminal-1940s-poster.webp`
- [ ] Two `source` elements: the `.webm` file first, then the `.mp4`, each with its `type`
- [ ] A `track` with `kind="captions"`, `src="media/union-terminal-1940s.vtt"`, `srclang="en"`,
      a `label`, and `default`
- [ ] Fallback text inside the `video` with a link to the `.mp4`
- [ ] The `video` is inside a `figure` with a `figcaption`

### Typography

- [ ] Two Google Fonts: an Art Deco **display** font for headings and the site name, and a
      readable **body** font for everything else
- [ ] Every `font-family` ends with a fallback, such as `serif` or `sans-serif`
- [ ] Font sizes use `rem`, with a clear scale from `h1` down to captions
- [ ] Body text has a `line-height` between 1.4 and 1.8
- [ ] Paragraphs are no wider than about 75 characters (`max-width` in `ch` or `rem`)

### Box model and layout

- [ ] The main content is a centered column with a `max-width` and `margin: 0 auto`
- [ ] Margins and padding are consistent from section to section
- [ ] Borders or `border-radius` are used to frame things like figures or the address
- [ ] Images and the video never overflow the column (`max-width: 100%`)
- [ ] The header, nav, and footer are styled, and the nav is no longer a bulleted list

### Background hero (`index.html`)

- [ ] The `.hero` section uses `images/hero.webp` as a `background-image`
- [ ] `background-size` and `background-position` keep the building in view at any width
- [ ] An overlay (for example a semi-transparent `linear-gradient` layered over the image)
      keeps the hero text readable
- [ ] The hero text passes a contrast check against the image

### Floated image (`visit.html`)

- [ ] The clock photo (`.float-image`) floats to one side, and the Hours text wraps around it
- [ ] It has a set width and margins so the text doesn't touch it
- [ ] The float is cleared, so the next section starts below it

### Stylesheet

- [ ] All of your CSS is in `css/styles.css`, and both pages use it
- [ ] No `style` attributes or `style` elements in the HTML
- [ ] The CSS passes the [W3C CSS Validator](https://jigsaw.w3.org/css-validator/#validate_by_input)
      with no errors

### ✅ Before You Submit

Check the following:

- [ ] No `TODO` comments are left in either page
- [ ] You did not rename or move any of the starter files
- [ ] Both pages pass the [W3C Markup Validator](https://validator.w3.org/#validate_by_input)
      with no errors
- [ ] On the **live site**, both pages use your fonts, and the hero, rotunda image, and floated
      clock look right on a computer and on your phone
- [ ] On the **live site**, the video plays and the captions show up
- [ ] In DevTools, the rotunda image loads a smaller file on a narrow screen
- [ ] You saved all of your files
- [ ] The site is live on GitHub Pages and the URL is in your pull request

## 📂 Starter Files

| File / Folder | Purpose |
| --- | --- |
| `index.html` | The Home page. Finish the TODOs for the fonts, the rotunda image, and the video. |
| `visit.html` | The Visit page. Finish the TODO for the fonts. |
| `css/styles.css` | Empty. Write all of your CSS here. |
| `images/` | `hero.webp` for the background, the rotunda in four widths, and the other photos already in the pages |
| `media/` | The film clip as `.webm` and `.mp4`, its poster image, and its captions file (`.vtt`) |

The HTML has only three classes: `.hero`, `.float-image`, and `.current` (the nav link for the
page you're on). Style everything else with element selectors like `header`, `nav`, `main`,
and `footer`.

## 🧮 Grading

| Criteria | What earns full credit | Points |
| --- | --- | --- |
| **Typography** | A Google Fonts display and body pairing with fallbacks; a consistent `rem` type scale; readable `line-height`; paragraphs limited to a readable line length. | 14 |
| **Box model and layout** | A centered content column; consistent margins and padding; borders or `border-radius` used with purpose; media stays inside the column; styled header, nav, and footer; the clock photo floats with wrapped text and the float is cleared. | 12 |
| **Media HTML** | The rotunda `img` has a correct `srcset` and `sizes`, `width`, `height`, `alt`, and lazy loading; the `video` has controls, a poster, two `source`s in the right order, a captions `track`, fallback text, and is in a `figure`. | 11 |
| **Background hero** | `hero.webp` fills the hero with `background-size` and `background-position`, and an overlay keeps the text readable. | 9 |
| **Stylesheet** | All CSS is in `css/styles.css`, shared by both pages, with no inline styles, and it passes the CSS validator. | 3 |
| **Published and submitted** | GitHub Pages site is live and loads correctly; pull request into `main` is open with the live URL in the description; PR URL submitted in Canvas. | 1 |
| **Total** |  | **50** |

## 📚 Resources

- Your CE4, CE5, and CE6 repos, which use every CSS property this assignment needs
- [Google Fonts](https://fonts.google.com/): try searching for Art Deco display fonts such as
  Limelight, Poiret One, or Federo
- [MDN: Fundamental text and font styling](https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/Text_styling/Fundamentals)
- [MDN: The box model](https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/Styling_basics/Box_model)
- [MDN: Backgrounds and borders](https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/Styling_basics/Backgrounds_and_borders)
- [MDN: Responsive images](https://developer.mozilla.org/en-US/docs/Web/HTML/Guides/Responsive_images)
- [MDN: Adding captions and subtitles to HTML video](https://developer.mozilla.org/en-US/docs/Web/Media/Guides/Audio_and_video_delivery/Adding_captions_and_subtitles_to_HTML5_video)
- [WebAIM Contrast Checker](https://webaim.org/resources/contrastchecker/)
- [W3C CSS Validation Service](https://jigsaw.w3.org/css-validator/#validate_by_input)

## 🆘 Getting Help

Ask during class or office hours, or post on the Canvas discussion board. Because this is an
independent assignment, I can point you to the right idea, but I won't write your CSS for you.

Before you ask, check these common problems:

- **None of your CSS works?** Check that you saved `css/styles.css`, and that you didn't rename
  or move it.
- **The hero image doesn't show?** The path in `url()` is relative to the **CSS file**, not
  the page. From `css/styles.css`, it's `url("../images/hero.webp")`.
- **Your Google Fonts don't load?** The Google Fonts `link` has to come **before** the link to
  `styles.css`, and the font name in `font-family` has to match Google's spelling exactly,
  in quotes.
- **The captions don't show when you open the page from your computer?** Some browsers block
  caption files on pages opened straight from a folder. Open the page with WebStorm's built-in
  preview, or check the live site.
- **The next section is squeezed beside the clock photo?** The float isn't cleared. Use
  `clear: both` on whatever should start below it.
- **The rotunda image always loads the biggest file?** Check that every file in `srcset` has its
  `w` width, and that `sizes` is there. Test in DevTools with the cache turned off.
- Did you save every file? Is every CSS rule closed with a `}` and every declaration ended with
  a `;`?

---

The AI policy and submission instructions are in the [README](../README.md).
