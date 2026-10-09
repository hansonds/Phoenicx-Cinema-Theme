<div align="center">

# 🎬 PHOENICX CINEMA

### Signature Edition · v2.0

**A cinematic, modern, dark interface for Jellyfin.**

*Smooth movie cards · Frosted-glass surfaces · Lavender accents · Media Bar styling*

![Jellyfin](https://img.shields.io/badge/Jellyfin-Custom_CSS-9469e2?style=for-the-badge&logo=jellyfin&logoColor=white)
![Version](https://img.shields.io/badge/Version-2.0-8e85fa?style=for-the-badge)
![Theme](https://img.shields.io/badge/Theme-Dark-151925?style=for-the-badge)

</div>

---

## ✨ Overview

**PHOENICX CINEMA** gives the Jellyfin web interface a refined, cinema-inspired look. It brings together rounded media cards, a dark palette, soft shadows, a glass-like navigation bar, and styling for a home-screen Media Bar slideshow.

The theme is distributed as **one combined CSS file**, so you do **not** need to import other theme stylesheets from a CDN.

> [!NOTE]
> The CSS styles the Media Bar, but it does **not** install or replace the Media Bar plugin. You need a compatible plugin if you want the slideshow itself.

## 🖼️ Preview

*Add your own screenshots to the `screenshots/` folder to show how the theme looks on your Jellyfin server.*

<!-- Uncomment after adding screenshots:
![PHOENICX CINEMA home screen](screenshots/home.png)
![Movie details](screenshots/details.png)
-->

## 🌟 Features

| Feature | What it changes |
| --- | --- |
| 🎞️ Cinematic home screen | Gradient overlays and slideshow presentation styles |
| 🪟 Frosted-glass UI | Header, menus, dialogs, and floating panels |
| 🍿 Movie & series cards | Rounded artwork, shadows, and desktop hover emphasis |
| 💜 Signature accent | Lavender highlights, buttons, outlines, and progress bars |
| 🔤 Readable typography | Nunito-based custom styling with theme typography fallbacks |
| ▶️ Playback actions | Rounded buttons and prominent play controls |
| 📱 Responsive styling | Adjustments for smaller screens and portrait layouts |
| ♿ Accessibility touches | Visible focus states and reduced-motion support |
| 📦 All-in-one CSS | No external **theme stylesheet** imports required |

## 🚀 Installation

### Option A — Paste into Jellyfin (recommended)

1. Download **[`PHOENICX_CINEMA_SIGNATURE_v2_CLEAN.css`](PHOENICX_CINEMA_SIGNATURE_v2_CLEAN.css)** from this repository.
2. Open Jellyfin in your browser with an administrator account.
3. Go to **Dashboard → General → Custom CSS** (the location may vary by Jellyfin version).
4. **Back up your existing Custom CSS**, then replace it with the complete contents of the downloaded file.
5. Save your changes.
6. Hard-refresh the web interface with **Ctrl + Shift + R** (or clear its cached site assets).

> [!IMPORTANT]
> Do not paste a second theme on top of this stylesheet. Competing styles can create layout issues or override your settings.

### Option B — Host your own CSS

You can host the CSS file yourself and import it from Jellyfin's Custom CSS field:

```css
@import url("https://YOUR-DOMAIN.example/path/PHOENICX_CINEMA_SIGNATURE_v2_CLEAN.css");
```

Replace the example URL with a real URL that serves the CSS file. This option **does** depend on your own hosted file being accessible.

## 🎛️ Customize the look

The combined stylesheet includes a **PHOENICX CINEMA** design-variable section. You can change the core colors and rounding to suit your taste:

```css
:root {
  --px-background: #090b12;
  --px-surface: #151925;
  --px-accent: #a69cff;
  --px-accent-light: #cbc4ff;
  --px-text: #f7f7fc;
  --px-card-radius: 15px;
  --px-panel-radius: 20px;
}
```

If you want to override values **without editing the main file**, place your overrides *after* the main stylesheet, in the same Custom CSS field.

## 🧩 Compatibility & requirements

- **Jellyfin Web:** intended for the modern Jellyfin web interface, with Jellyfin 12 layout adaptations included.
- **Media Bar:** styling is included; slideshow operation requires a compatible Media Bar plugin and configuration.
- **Browsers:** modern Chromium-based browsers are a sensible starting point. Other browsers and TV clients may behave differently.
- **Native apps:** Custom CSS only affects clients that render and accept the Jellyfin web CSS; it cannot be assumed to restyle every native app.
- **Network:** the theme CSS is self-contained with respect to other *themes*, but it references Google Fonts / font assets, which may require internet connectivity unless self-hosted.

**Compatibility is not guaranteed across all Jellyfin releases, plugins, or devices.** Test after upgrades.

## 🛠️ Troubleshooting

| Issue | What to try |
| --- | --- |
| Old design is still visible | Hard-refresh the browser and clear cached assets |
| Cards or menus look broken | Remove any older Custom CSS or competing theme overrides |
| Slideshow doesn't appear | Check that your Media Bar plugin is installed, compatible, and configured |
| Fonts look different | Check connectivity to Google Fonts; fallback fonts may be used |
| Mobile / TV layout is awkward | Test in Jellyfin Web first; client support varies |

To revert, remove the theme from **Custom CSS**, restore your backup if needed, save, and refresh.


## 🙌 Credits & third-party notices

PHOENICX CINEMA's standalone stylesheet incorporates and customizes existing Jellyfin theme work, including:

- **ElegantFin** by **lscambo13**
- **Media Bar Plugin Support** add-on by **lscambo13**
- **ElegantFin for Jellyfin 12 Modern** by **mihaif7** ([upstream repository](https://github.com/mihaif7/elegantfin-jf12))

See **[`PHOENICX_CINEMA_THIRD_PARTY_NOTICES.txt`](PHOENICX_CINEMA_THIRD_PARTY_NOTICES.txt)** for additional attribution. The original authors retain their rights; all applicable upstream license requirements continue to apply. Before publishing the combined CSS, make sure the complete relevant licenses and notices are included as required.

## 💜 PHOENICX CINEMA

<div align="center">

**Your library. Your screen. Your cinema.**

*Built for a more immersive Jellyfin experience.*

</div>
