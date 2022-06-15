# HTML `<portal>` Demo

## Description
This demo showcases Chrome's experimental `<portal>` element which functions very similarly to an `<iframe>`, but with the added ability to click directly into the portal source page. The goal of Chrome's portal project is to enhance prerendering with a inset preview of the content. At the time of this demo, `<portal>` is in the [draft](https://wicg.github.io/portals/) development stage.

This demo shows a simple list of webcomics. Each comic has a preview hero image and upon mousing over the section, a portal of the the webcomic page will load and display inline. A user can then click the portal to be taken immediately to the new page with it already preloaded.

<img src="https://github.com/doctafaustus/html-portal/blob/preview-gif/chrome_1sXGgQBBtJ.gif?raw=true">

## Prerequisites
You must be using Chrome and have the following flags enabled at `about://flags/#enable-portals`:
- 🚩 Enable Portals
- 🚩 Enable cross-origin Portals

Chrome will prompt you to relaunch your Browser and after doing so, you should see the `HTMLPortalElement` function available in your console:
<br/>
<br/>
<img width="400px" src="https://web-dev.imgix.net/image/admin/aUrrqhzMxaEX865Fk5zX.png?auto=format&w=1252">

## Setup
The easiest way to preview this demo is to use VSCode's [Live Preview](https://marketplace.visualstudio.com/items?itemName=ms-vscode.live-server) extension where you can start a local server to serve the `index.html` and `style.css` files. Note that `<portal>` will NOT work if viewing the page without a server, otherwise you will see the following warning in the console: `<portal> use is restricted to the HTTP family.`

## Further Resources
- Portal introduction @ Chrome Dev Summit 2018: https://www.youtube.com/watch?v=Ai4aZ9Jbsys
- MDN article: https://developer.mozilla.org/en-US/docs/Web/HTML/Element/portal
- Chrome blog post: https://web.dev/hands-on-portals/
- GitHub proposal: https://github.com/WICG/portals
- Browser support: https://caniuse.com/portals
