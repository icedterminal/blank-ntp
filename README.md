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
You can either download a pre-compiled version from the releases page, or compile it yourself. With either method, you need to enable Developer Mode first from the Extensions page in the browser. EX: `chrome://extensions` or `edge://extensions`.

With a compiled extension, drag and drop it into the Extensions window. The extension will not load. This is expected. To enable it. follow the steps below for the browser you use.
<!--
## Google Chrome
https://support.google.com/chrome/a/answer/187202?hl=en#zippy=%2Cwindows
-->
## Microsoft Edge
1. You must have Windows Pro or higher to access Group Policy Editor.
    - Note: When "hacking" Windows Home to enable a feature that is part of Pro is piracy. Additionally, Windows will detect this as corruption and can repair itself. It can also prevent you from installing updates. They will fail until Windows is repaired. Thus undoing your "hack".
2. [Download the Policy files/templates.](https://www.microsoft.com/en-us/edge/business/download)
3. From the downloaded zip, go to `windows\admx` and extract `msedgeupdate.admx`, `msedgewebview2.admx` and `msedge.admx`.
4. Then from your language code (EX: `en-US`) extract `msedgeupdate.adml`, `msedgewebview2.adml`, and `msedge.adml`.
5. Copy the files to following locations:
   - `admx` goes in `C:\Windows\PolicyDefinitions\`
   - `adml` goes in `C:\Windows\PolicyDefinitions\<lang>`
6. Open Local Group Policy Editor (gpedit).
7. Navigate to [Computer Config] > [Administrative Templates] > [Microsoft Edge] > [Extensions] > [Allow specific extensions to be installed].
8. Click [Enable] and then [Show...]
9. Copy the extensions ID (EX: `abibhdeafodcmlcgiikhmhkiigehlhgh`) from the Extensions page and paste it into the box.
10. Click [OK] and [OK].
11. Restart Edge.
12. Disable Developer Mode.

The extension will now load normally. You will see a prompt the first time asking if this was the new tab you were expecting. If you accept, this warning will go away and the extension will remain enabled.

# Your Modifications
Because this extension is open source, you can freely fork and modify the empty page to include what ever you want. For advanced configuration, read the [developer documentation](https://developer.chrome.com/docs/extensions/). Remember, you must pack it and white-list it so the warnings no longer appear.