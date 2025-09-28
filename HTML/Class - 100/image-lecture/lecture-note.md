# Lecture Notes – HTML Media and File Paths

## 1. The `<img>` Tag (Images)

The `<img>` tag is used to display images on a webpage.
It is a **self-closing tag** (no closing tag needed).

### Common Attributes

* **`src`** → specifies the image file location.
* **`alt`** → alternative text shown if the image fails to load.
* **`width` and `height`** → set the size of the image.
* **`srcset` & `sizes`** → used for responsive images (different images for different screen sizes).

### Example:

```html
<img src="same-path-image.png" alt="An image of a television">
```

#### Image Types

* **JPEG / JPG** → good for photographs.
* **PNG** → supports transparency, good for graphics.
* **GIF** → supports animation.
* **SVG** → scalable vector graphics (logos, icons).
* **ICO** → used for favicons (browser tab icons).

#### Inline Nature of `<img>`

The `<img>` tag is **inline**, meaning it sits inside text or other elements without breaking the flow.

Example:

```html
<a> Click me 
   <span><img src="animated.gif" alt="Love"></span>
</a>
```

---

## 2. The `<video>` Tag (Videos)

The `<video>` tag embeds videos into webpages.

### Common Attributes

* **`controls`** → shows play/pause/volume buttons.
* **`autoplay`** → plays video automatically (not recommended without `muted`).
* **`muted`** → starts video without sound.
* **`loop`** → repeats the video.
* **`width` / `height`** → sets size of video player.

### Example:

```html
<video autoplay muted height="400" width="600" controls>
   <source src="video-1.mp4" type="video/mp4">
   <source src="video-1.ogg" type="video/ogg">
   Your browser does not support the video tag.
</video>
```

---

## 3. The `<audio>` Tag (Sounds & Music)

The `<audio>` tag is used to embed sound or music files.

### Common Attributes

* **`controls`** → displays play/pause/volume buttons.
* **`autoplay`** → plays audio automatically.
* **`muted`** → starts muted.
* **`loop`** → plays again when finished.

### Example:

```html
<audio controls muted autoplay>
   <source src="audio-1.mp3" type="audio/mpeg">
   <source src="audio-1.ogg" type="audio/ogg">
   Your browser does not support the audio element.
</audio>
```

---

## 4. The `<iframe>` Tag (Embedded Pages & Videos)

The `<iframe>` tag is used to embed another webpage or external content inside your webpage.
It is commonly used for **YouTube videos, Google Maps, and other sites**.

### Example:

```html
<iframe width="420" height="315"
   src="https://www.youtube.com/embed/d_F2qdjxm-I">
</iframe>
```

---

## 5. File Paths in HTML

When using `src` or `href`, you need to tell the browser **where the file is located**.

### Relative Path

* **No `/` at the beginning** → means file is in the same folder as your HTML file.

  ```html
  <img src="same-path-image.png">
  ```

* **`../`** → means "go up one folder."

  ```html
  <img src="../image-2.png">
  ```

* **`../../../`** → go up three folders.

  ```html
  <img src="../../../images/image-1.png">
  ```

### Absolute Path

* A full **URL** that includes `http://` or `https://`.

  ```html
  <img src="https://ng.jumia.is/product/television.jpg">
  ```

* Starting with `/` → means the file is located at the **root directory** of your project or server.

---

## 6. Background Images

You can also add images as **backgrounds in CSS**:

```html
<p style="
   background-image: url('images/image-1.png');
   height: 500px;
   background-repeat: no-repeat;
   background-size: cover;
   background-position: center;
   color: white;
   font-size: 50px;
">
   This is a paragraph with a background image.
</p>
```

---

# Summary

* Use `<img>` to add pictures (inline element).
* Use `<video>` to play videos, with multiple file formats for browser support.
* Use `<audio>` to embed music/sounds.
* Use `<iframe>` to embed other websites (like YouTube).
* Understand **relative paths (`../`)** vs **absolute paths (`/`, full URLs)** for locating files.