COOKIE PATROL - installable iPad app (PWA)

What's in this folder
  index.html            the whole game (works on its own as a web page)
  manifest.webmanifest  makes it installable (name, icon, full-screen, landscape)
  sw.js                 service worker: saves the game so it works with no internet
  icon-192.png, icon-512.png, apple-touch-icon.png   app icons

How to put it on the iPad (one time, needs internet)
  1. Put this folder on any free static web host. Easiest: open app.netlify.com/drop
     on a computer and drag this whole folder onto the page. (GitHub Pages and
     Cloudflare Pages also work.) You get an https:// link.
  2. Open that link in Safari on the iPad.
  3. Tap Share -> Add to Home Screen -> Add.
  4. Open it from the Home Screen. It runs full screen, with no Safari bars,
     and keeps working offline after the first launch.

Note: PWAs need to be served over https, so double-clicking the files on the iPad
will not install it. A real App Store app would need Xcode and an Apple developer account.
