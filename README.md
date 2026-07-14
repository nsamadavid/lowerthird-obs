# Animated-Lower-Thrids
Animated Lower Thirds with dockable Control Panel - OBS Tool

With this tool you can use a control panel to add and change your own lower thirds on the fly. Feel free to customize. Basic knowledge of HTML, Javascript and CSS is required.
For communication between control panel and browser layer it use BroadcastChannel API.

1. Download the Zip file, unzip it.
2. See how to install and new features: https://youtu.be/tddMYWya7O0
3. See previus features: https://youtu.be/cQ0_1GwpwB0

Unfortunately, OBS doesn't support browser panels on macOs. It only works on Windows.

This project is based on Lower thirds in HTML/CSS https://obsproject.com/forum/resources/lower-thirds-in-html-css.928/, and Animated lower thirds with control panel https://obsproject.com/forum/resources/animated-lower-thirds-with-control-panel.922/.


I am a designer and my scripting knowledge is few. I made this tool (Frankenststool) because I needed it and I want to share it. You are welcome to improve it. I am aware that many parts of the code can make any expert cry. I'm really sorry :P


## Bilingual full-width lower third (English / Français)

A separate, self-contained lower third styled after a broadcast title design: a full-screen-width
white bar with an English section (left) and a French section (right) for live translations, plus
two accent tag boxes. The intro animates a line wipe, a color curtain reveal, sliding text and
tags that emerge from behind the bar; the outro reverses it.

Setup in OBS (works alongside the original 4 lower thirds, or on its own):

1. **Browser Source**: add a new Browser Source, check "Local file", pick
   `lower thirds/bilingual-browser-source.html`, set width 1920 and height 1080.
2. **Control panel**: OBS menu → Docks → Custom Browser Docks…, name it (e.g. "Bilingual LT") and
   point it at `lower thirds/bilingual-control-panel.html`.
3. Type your English and French texts in the dock and press **SHOW**. Texts, colors, sizes and
   timing update live; the animation only replays when you hide and show again.
4. Optional: set "Active time" to auto-hide after N seconds. Use "Replay" under the preview to
   test the animation without affecting the live source.

Quick standalone preview in a normal browser: open
`lower thirds/bilingual-browser-source.html?demo=1` (loops the animation with sample text).

## Donations.
If you like the extension and you want to support the development - please consider to donate by [Paypal](https://paypal.me/noealdac). Any donations are greatly appreciated.

## License.
The Animated Lower Thirds source code is made available under the [MIT license](https://github.com/noeal-dac/Animated-Lower-Thrids/blob/master/LICENSE).
