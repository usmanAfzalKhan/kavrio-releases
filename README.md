# Kavrio

Kavrio is a web browser for Windows. It is built on Chromium, the same engine as Chrome and Edge, so websites look
and work the way they do there. On top of that it adds a few things built in, with nothing extra to install:
blocking of ads, trackers and pop-ups, a VPN, a coupon helper for shopping, split view, and profiles.

**[Download the latest version](https://github.com/usmanAfzalKhan/kavrio-releases/releases/latest)** (Windows 10 and
11, 64-bit). Run `Kavrio-Setup-<version>.exe`. Kavrio updates itself after that.

> The installer is not code-signed yet, so Windows may say "Windows protected your PC". Choose **More info**, then
> **Run anyway**.

## What it does

### Ads, trackers and pop-ups
Ads and trackers are blocked on every site using the same public filter lists as uBlock Origin, plus lists of
known scam and malware sites. Pop-ups, pop-unders and pages that redirect you somewhere you did not click are stopped.
The shield in the address bar shows how many were blocked on the page, and lets you turn blocking off for one site.

### VPN
Open the menu and choose **VPN**.
- **Kavrio VPN** is free and needs no app and no account. Pick a country, or "Fastest available", and websites see an
  address there instead of yours. Only Kavrio's traffic changes, not the rest of the computer. It runs on
  [Tor](https://www.torproject.org/), which is included with Kavrio. It is slower than a normal connection.
- **My own VPN** uses the proxy details from a VPN you already pay for (HTTP or HTTPS with a login, or SOCKS5).
  The password is encrypted by Windows.
- If the VPN drops (Wi-Fi change, sleep), Kavrio reconnects by itself. While it reconnects, pages wait instead of
  using your real address.
- Some sites refuse all VPNs. Kavrio opens those directly, says so, and lists them in the VPN panel so you can switch
  the VPN back on for them.
- A small red dot on the VPN badge appears when a page asks for payment or an address, because some shops decline
  payments made through a VPN.

### Coupons
On a shop's cart or checkout page, a tag in the toolbar shows how many promo codes Kavrio has for that shop.
**Try codes** enters each one into the shop's own promo box, reads the shop's answer, keeps the code that saves the
most, and removes codes the shop says are expired or invalid. Codes you type into a shop yourself are remembered
when the shop accepts them. Kavrio also downloads a small shared list of codes once a day. You can add or remove codes
yourself, or switch the helper off. Kavrio never opens extra tabs or adds affiliate links.

### Tabs and split view
- Show 2 to 5 tabs side by side in one window: the **split view** button (two columns) in the toolbar, or
  right-click a link > **Open link in split view**.
- Drag tabs to reorder, pin, mute, tab search (Ctrl+Shift+A), reopen closed tab (Ctrl+Shift+T).
- Tabs you have not used for 30 minutes go to sleep to save memory and wake when you click them.
- Task manager (Shift+Esc) shows memory and CPU for each tab.

### Right-click menu
Everything you expect (back, reload, save, print, copy, inspect) plus: create a QR code for the page, translate the
page or a selection, search for a selection, copy a link without its tracking tags, copy a link to highlighted text,
open a link in split view or a private window, and view page source.

### Profiles and privacy
- Each profile has its own history, bookmarks, logins and look, with an optional password lock.
- Private windows keep nothing after you close them.
- Saved logins (cookies) are encrypted on disk with your Windows account.
- Clear browsing data (Ctrl+Shift+Delete) for a time range.

### Everything else
New-tab page with search and shortcuts, bookmarks (import from and export to Chrome, Edge and Firefox), history,
downloads with pause and resume, find on page, real page zoom, full screen, save page as PDF, error pages that say what
went wrong, and automatic updates.

## Security
- Every website runs in Chromium's sandbox, separated from Kavrio and from your files.
- Websites cannot talk to Kavrio's own controls; every internal message is checked for where it came from.
- The Kavrio program is locked so other programs cannot use it to run their own code, and its files are checked
  for tampering when it starts.
- Camera, microphone, location and notifications are asked for per site.
- No account, no ads, no data sent to Kavrio's developer. The only things Kavrio downloads on its own are filter-list
  and coupon-list updates and its own updates, all from public addresses.

## Privacy notes
- Kavrio VPN uses the Tor network: the website sees a Tor address, and your internet provider sees that you use Tor
  but not which sites. Do not use it for anything that needs strong anonymity; use Tor Browser for that.
- Some sites block VPNs or ask for more checks while one is on.

## Reporting a problem
Open an issue on this page with what you did, what you expected, and what happened.

The source code is kept in a private repository.
