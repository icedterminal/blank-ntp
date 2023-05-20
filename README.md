# Blank New Tab

For Chromium based browsers.

- Chrome
- Edge
- Vivaldi
- Opera
- Brave
- Comodo Dragon
- Torch
- Yandex Browser
- etc.

# How To
Most Chromium based browsers are restrictive in nature to prevent malicious extensions from being installed. I have not yet tested all browsers to provide instructions for them.

## Load the Extension
You need to enable Developer Mode first from the Extensions page in the browser. EX: `[chrome|edge|vivaldi|etc.]://extensions`. You can load an unpacked extension from the folder where the extension files are located.

Some browsers do not like this. Vivaldi does not constantly nag you about an unpacked extension. Chrome and Edge will. You need to compile the extension, drag and drop it into the Extensions window. The extension will not load. This is expected. To enable it, you need to download the Policy files/templates.

- https://support.google.com/chrome/a/answer/187202?hl=en#zippy=%2Cwindows
- https://www.microsoft.com/en-us/edge/business/download

The extension will now load normally. You will see a prompt the first time asking if this was the new tab you were expecting. If you accept, this warning will go away and the extension will remain enabled.

# Your Modifications
Because this extension is open source, you can freely fork and modify the empty page to include what ever you want. For advanced configuration, read the [developer documentation](https://developer.chrome.com/docs/extensions/). Remember, you must pack it and white-list it so the warnings no longer appear.