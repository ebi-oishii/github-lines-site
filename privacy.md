---
layout: default
lang: en
title: Privacy Policy
description: The privacy policy for the Chrome extension GitHub Lines.
permalink: /privacy/
alt: /ja/privacy/
alt_label: 日本語
---

# Privacy Policy

This is how the provider of the Chrome extension "GitHub Lines" (the extension) — the party shown as its developer on the Chrome Web Store — treats information about the people who use it.

**Last updated: 19 September 2026**

<div class="notice">
The provider collects nothing from the people who use this extension. There is no server behind it: the only party it communicates with is GitHub (github.com and api.github.com).
</div>

## 1. What is not collected

The provider collects no information whatsoever about you through this extension. In particular, none of the following happens:

- Creating an account, signing in, or obtaining an email address
- Analytics, crash reporting, or advertising identifiers
- Serving advertisements
- Sending the provider the names of repositories or files you looked at, their line counts, or their contents

The extension contains no code that transmits anything to a server run by the provider. No analytics, advertising or other third-party SDK is embedded in it.

## 2. What is stored on your device

The following is held inside your browser, and nowhere else.

| Where | What |
| --- | --- |
| Extension storage (`chrome.storage.local`) | Your settings (colour thresholds, what is shown, the counting mode, fetch limits, concurrency, exclusion patterns, display language) and any access tokens you registered |
| Extension database (IndexedDB) | The cache of what has been fetched (line counts per file, directory listings, and the contents of `.gitattributes`) |

All of it lives in your browser profile. The provider cannot reach it.

## 3. Access tokens

To display private repositories, or to raise the hourly API limit, you may register an access token that you issued yourself on GitHub.

- The token is stored in the extension storage described above
- It is used only in the authorization header of requests to the GitHub API (`api.github.com`). GitHub is the only place it is sent
- The provider never receives it. You can delete it from the options page, and removing the extension deletes it with them

Registering a token is optional. Without one the extension still works on public repositories, within GitHub's unauthenticated limit of 60 requests an hour.

## 4. Communication

The extension communicates in exactly two ways.

- **On GitHub's pages**: it adds its display to the file list on `github.com`
- **To the GitHub API**: it fetches the tree of the repository you are viewing, file contents (in order to count their lines), and how much of the API budget is left, from `api.github.com`

What comes back is used only to count lines and display them, and is cached on your device. Nothing is sent anywhere other than GitHub.

## 5. Permissions

The permissions shown on the Chrome Web Store are requested for these purposes.

- **Storage**: to keep your settings, tokens and cache on your own device
- **Access to github.com**: to add the display to the file list
- **Access to api.github.com**: to fetch the data the line counts are calculated from

The extension requests access to none of the following: browsing history, location, camera, microphone, contacts.

## 6. Disclosure to third parties

Since the provider collects no information, there is none to disclose to anyone.

## 7. Deletion

- "Clear the cache" on the options page deletes everything that has been fetched
- Tokens can be deleted on the options page
- Removing the extension from Chrome deletes the settings, the tokens and the cache together

## 8. Children

This extension is not directed at any particular age group. Because it collects no information, it does not collect information from children either.

## 9. Changes

Any material change will be announced on this site. A revised policy applies from the effective date shown on it.

## 10. The provider, and getting in touch

- Email: [ebi.apps.support@gmail.com](mailto:ebi.apps.support@gmail.com)
- Bugs and requests: [GitHub Issues](https://github.com/ebi-oishii/github-lines/issues)

Matters that must be disclosed by law, such as the provider's name and address, will be answered without delay upon a lawful request from the person concerned.

**Effective from: 19 September 2026**
