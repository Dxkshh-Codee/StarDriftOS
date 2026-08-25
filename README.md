# StarDriftOS

A personal webOS that runs in the browser. Landing page + desktop with draggable windows and small apps. Single HTML file, no frameworks.

Live demo: https://dxkshh-codee.github.io/StarDriftOS/

## What it is

Landing screen with a boot typing line, starfield, ticker and status window. Click "enter my os" and it loads a desktop with a taskbar, clock, calendar and windows. There is a small easter egg with the satellite that follows the cursor.

## Apps

- browser - opens Wikipedia random article in an iframe
- calculator - basic calculator with keyboard support
- camera - live camera preview and capture (needs https)
- hubble - gallery with 6 images from hubble/ folder
- notes - auto-saves to localStorage, shows word count
- terminal - small shell with commands like help, open, close, wallpaper, neofetch
- snake - canvas snake game, saves best score

Settings lets you switch between 10 wallpapers. Choice is saved in localStorage.

## Running it

Clone and just open index.html. No build step.


git clone https://github.com/Dxkshh-Codee/StarDriftOS.git
cd StarDriftOS
# then open index.html in your browser


Or serve it locally:

npx serve .


## Project structure


StarDriftOS/
├── index.html          # main file to deploy
├── StarDriftOS.html    # same as index.html
├── satellite.png
├── pfp.webp
└── hubble/             # images for the gallery


## Customizing

Search for these tags inside index.html:

- [EDIT: NAME] - your name
- [EDIT: BIO] - bio paragraph
- [EDIT: LINKS] - links under the hero
- [EDIT: TICKER] - scrolling facts
- [EDIT: IMAGE] - replace satellite.png
- [EDIT: GALLERY] - edit HUBBLE_PHOTOS array

Terminal commands: help, about, apps, open <app>, close <app>, wallpaper, neofetch, echo, date, uptime, clea, exit.

## Deploy to GitHub Pages

It is a static site. Push index.html to main, then in GitHub go to Settings -> Pages -> Source: Deploy from a branch -> Branch: main / root -> Save. After a minute it will be live at https://yourname.github.io/StarDriftOS/.

## Notes

Built with plain HTML.
