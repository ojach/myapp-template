# My App Template

An easy, single-file HTML template that brings your favorite web pages together in a mobile app-style launcher.

**OJapp Free** is already included in `index.html`. Publish the page and add it to your home screen to launch it like an app.

## How to use

### 1. Open the HTML file

Open `index.html` in a text editor.

### 2. Edit four sections

Search the HTML for `[EDIT` to find every section you need to customize.

1. **App name, description, and home screen icon**
2. **Colors and appearance**
3. **Header text**
4. **Apps to display**

Edit each app inside the `MY_APPS` list:

```js
{
  name: "Shop",
  url: "https://example.com/shop/",
  icon: "🛍️",
  color: "#fff0f4"
}
```

- `name`: Label shown below the icon
- `url`: URL to open
- `icon`: Emoji or image URL
- `color`: Icon background color

Copy a `{ ... }` block to add as many apps as you like.

### 3. Publish it online

Upload the edited HTML file to an HTTPS-enabled web server.

Rename the file to `index.html` if you want it to open directly from the folder URL.

### 4. Add it to your home screen

Open the published page on your phone.

- **iPhone:** Safari Share button → **Add to Home Screen**
- **Android:** Chrome menu → **Add to Home screen** or **Install app**

The add-to-home-screen tip is automatically hidden when the page is launched as an app.

## Home screen icon

Replace the URL below with the URL of your own square image:

```html
<meta name="ojapp:icon" content="https://example.com/icon.webp">
```

A **512×512px WebP** image is recommended. Make sure the image URL can be opened directly in a browser.

## OJapp Free

This template uses one line of OJapp Free to turn the page into a home screen app:

```html
<script src="https://ojapp.app/js/ojapp.js"></script>
```

[Learn more about OJapp Free](https://ojapp.app/one-page-one-app/en)
