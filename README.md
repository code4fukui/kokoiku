# kokoiku

> 日本語のREADMEはこちらです: [README.ja.md](README.ja.md)

A simple web app to guide people to a specific location. "Kokoiku" (ココイク - "go here") generates a Google Maps directions link from the user's current location to a preset destination, making it easy to share location guidance via email, messaging, or on a website.

When a user opens a `kokoiku` link, the app gets their GPS location and creates a direct link to Google Maps with the route already calculated.

## Demo

[https://codeforfukui.github.io/kokoiku/](https://codeforfukui.github.io/kokoiku/)

*The default demo link directs you to the red pandas at Sabae's Nishiyama Park.*

## Features

*   **One-Click Directions:** Generates a direct link to Google Maps with the route calculated from the user's current location.
*   **Customizable Destination:** Easily set any destination by embedding its coordinates in the URL hash.
*   **Fallback Location:** If GPS is unavailable or permission is denied, it defaults to a fixed starting point (Sabae Station).
*   **Lightweight:** A single HTML file with no external library dependencies.

## How to Create Your Own Link

To create a "kokoiku" link for your own destination, simply append its latitude and longitude to the base URL using a hash (`#`).

**Format:** `https://codeforfukui.github.io/kokoiku/#LATITUDE,LONGITUDE`

### Example 1: Sharing a Link

Send this URL in an email or message to guide someone to the entrance of the Fukui College of Technology's engineering building:

```
https://codeforfukui.github.io/kokoiku/#35.937525,136.171508
```

### Example 2: Embedding on a Website

Add a link to your website to help visitors find a location:

```html
<a href="https://codeforfukui.github.io/kokoiku/#35.950908,136.180781" target="_blank">
  Come see the red pandas in Sabae!
</a>
```

## Attribution

Created by [Taisuke Fukuno](http://fukuno.jig.jp/784) (福野泰介).

## License

[CC BY 2.1 JP](https://creativecommons.org/licenses/by/2.1/jp/)