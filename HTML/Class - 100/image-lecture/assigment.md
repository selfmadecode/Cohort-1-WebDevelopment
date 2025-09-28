# Practice Exercises – HTML Media & Paths

## 1. Image Practice

1. Create a simple webpage and display an image stored in the **same folder** as your HTML file.
   Example: `my-photo.jpg`

   ```html
   <img src="my-photo.jpg" alt="My Photo">
   ```

2. Add an image located **one folder up** using `../`.


3. Add an **online image** from any website using its full URL.


---

## 2. Background Image Practice

Create a `<div>` with a background image. Add some text inside it.
The backgound image should cover the entire div
The div height should be 500px, and the width should be the width of your device (fullscreen)
the font should be bold
use external css
Center the text horizontally and vertically inside the div using CSS.
Change the text color.
Add a border or a box-shadow around the div
Make the text change color when hovered
the background image to be stored in an images folder

---

## 3. Video Practice
### Do this for file stored locally and online

Center the video players on the page using CSS.
Add a background color to the page.
1. Insert a **local video** (saved in a `video` folder).

   ```html
   <video controls width="400">
      <source src="video/my-video.mp4" type="video/mp4">
   </video>
   ```

2. Make the video **autoplay without sound**.

   ```html
   <video controls autoplay muted width="400">
      <source src="video/my-video.mp4" type="video/mp4">
   </video>
   ```

---

## 4. Audio Practice
### Do this for file stored locally and online

Center the audio players on the page using CSS.
Add a background color to the page.
1. Add a **local mp3 file** called `song.mp3`.

   ```html
   <audio controls>
      <source src="audio/song.mp3" type="audio/mpeg">
   </audio>
   ```

2. Add a background music that plays automatically and loops:

   ```html
   <audio autoplay loop>
      <source src="audio/music.mp3" type="audio/mpeg">
   </audio>
   ```

---

## 5. Iframe Practice

1. Embed a YouTube video inside your page. (Use the **embed link**, not the share link).
   Example:

   ```html
   <iframe width="560" height="315"
      src="https://www.youtube.com/embed/d_F2qdjxm-I"
      frameborder="0" allowfullscreen>
   </iframe>
   ```

2. Embed **Google Maps** of Rumu-Okoro using an iframe.

   * Search your city on Google Maps.
   * Click **Share → Embed a map → Copy HTML**.
   * Paste it inside your HTML.

---

## 6. Path Navigation Practice

Create three folders:

* **project**

  * **images**

    * `add an image`
  * **videos**

    * `add an video`
  * **index.html**

Inside `index.html`:

1. Show the image from the **images folder**.
2. Play the video from the **videos folder**.
3. Add an online image from the internet.

---

# Challenge Task

Build a **mini portfolio webpage** with:

* A profile picture (`<img>`)
* A background image behind your name (`background-image`)
* An audio file playing your favorite song (`<audio>`)
* A short video introduction (`<video>`)
* A YouTube video you like (`<iframe>`)
