# navigation-stats
Fork of https://github.com/mdn/webextensions-examples/tree/main/navigation-stats  
I am working on a browser extension, and this sample is a good starting point.
I don't do much JavaScript programming or GitHub source management. If you see something wrong or could be done better, please give me feedback. I literally don't know what I'm doing here! If it wasn't for ChatGPT, I wouldn't have even gotten this far!

## What it does
The extension includes:
* a background which collects navigation stats using the webNavigation API, and store the stats using the storage API.
* a browser action with a popup including HTML, CSS, and JS, which renders the stats stored by the background page  

When the user navigate on a website from any of the browser tabs, the background page collected every completed navigation with the "http" or "https" schemes (using an UrlFilter for the listener of the webNavigation events)

When the user clicks the browser action button, the popup is shown, and the stats saved using the storage API are retrived and rendered in the popup window.

## What it shows
* use the webNavigation API to monitor browsing navigation events
* use an UrlFilter to only receive the webNavigation event using one of the supported criteria.
* use the storage API to persist data over browser reboots and to share it between different extension pages.
