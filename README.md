<h1>
<sub>
<img src="https://raw.githubusercontent.com/conceptualspace/yet-another-speed-dial/master/src/icons/icon32.png" height="32" width="32">
</sub>
Yet Another Speed Dial
</h1>

<h1>
<a href='https://addons.mozilla.org/en-US/firefox/addon/yet-another-speed-dial/'><img alt='Get it for Firefox' src='https://github.com/conceptualspace/yet-another-speed-dial/raw/master/assets/badges/ff-badge.png'/></a> <a href='https://chrome.google.com/webstore/detail/yet-another-speed-dial/imohnlganmafcmidafklgkgfgaagiohn'><img alt='Get it for Chrome' src='https://github.com/conceptualspace/yet-another-speed-dial/raw/master/assets/badges/chrome-badge.png'/></a> <a href='//www.microsoft.com/store/apps/0RDCKB416QRD?cid=storebadge&ocid=badge'><img src='https://github.com/conceptualspace/yet-another-speed-dial/raw/master/assets/badges/microsoft-badge.png' alt='English badge' style='width: 166px; height: 60px;'/></a>
</h1>

A modern, cross-browser speed dial that respects your privacy, inspired by Opera

- Automatically generates thumbnails and screenshots, or add your own.
- Uses the native bookmarks library so speed dials can be synced by the browser.
- Sortable with drag and drop
- Supports folders
- Simple and fast UI
- No ads, trackers, or bullshit.

---

![alt tag](https://github.com/conceptualspace/yet-another-speed-dial/raw/master/assets/screenshot.png)




---

## FAQ:

### Can I use different images for the speed dials?
Yes! Just right-click the speed dial and select Edit.

### One of my site thumbnails disappeared?
YASD includes a thumbnail linked using the Open Graph standard when available. This keeps those thumbnails up to date automatically, but if the website removes the image it may no longer load in YASD. To fetch new images, simply right-click the dial and select "Refresh thumbnails".

### Why does YASD require the "access your data for all websites" permission?
This is required for YASD to capture an image of the website for the thumbnail. **Absolutely no data is collected for any reason whatsoever**. These two features (visual thumbnails and user privacy) were the primary motivation for creating YASD. Note YASD will still work if you deny this permission, but without capturing thumbnails. You can find the YASD privacy policy here: https://conceptualspace.net/privacy.md

### Why is YASD showing CPU usage in the Chrome task manager?
The *actual* CPU usage is very low (confirm using your OS task manager) but some cycles are used to elimate jankiness. YASD uses a high performance rendering engine (GSAP) to keep user ineractions and animations smooth. The usage will be 0 when YASD is not in the foreground.

### Why isn't the address bar focused (active) by default on the new tab / home page?
Unfortunately, this is a bug in Firefox. You can nag Mozilla to fix it here: https://bugzilla.mozilla.org/show_bug.cgi?id=1411209

---

## building for chrome vs firefox

chrome: remove `chrome_settings_overrides` and `browser_specific_settings` manifest keys  
firefox: no changes are required
