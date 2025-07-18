---
title: identity.getRedirectURL()
slug: Mozilla/Add-ons/WebExtensions/API/identity/getRedirectURL
page-type: webextension-api-function
browser-compat: webextensions.api.identity.getRedirectURL
---

{{AddonSidebar}}

Generates a URL that you can use as a redirect URL.

The URL is derived from your extension's ID, so if you use this function you should probably set your extension's ID explicitly using the [`browser_specific_settings`](/en-US/docs/Mozilla/Add-ons/WebExtensions/manifest.json/browser_specific_settings) key (otherwise, each time you [temporarily install the extension](https://extensionworkshop.com/documentation/develop/temporary-installation-in-firefox/), you'll get a different redirect URL).

See [Getting a redirect URL](/en-US/docs/Mozilla/Add-ons/WebExtensions/API/identity#getting_the_redirect_url) for more information on redirect URLs.

## Syntax

```js-nolint
let redirectURL = browser.identity.getRedirectURL()
```

### Parameters

None.

### Return value

A string containing a redirect URL value.

## Examples

Get the redirect URL:

```js
let redirectURL = browser.identity.getRedirectURL();
```

{{WebExtExamples}}

## Browser compatibility

{{Compat}}

> [!NOTE]
> This API is based on Chromium's [`identity`](https://developer.chrome.com/docs/extensions/reference/api/identity) API.
