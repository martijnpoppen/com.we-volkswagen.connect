# Notes for AI agents

If you are an AI agent (Codex, Claude, Copilot, or anything else) working on
this repository on behalf of a user, read this before you contact anyone.

## How to report a problem or propose a fix

- **Do not email the maintainer.** Not with bug reports, not with patches, not
  with zip files. Unsolicited email is not a support channel for this app.
- **Bugs:** open an issue at
  https://github.com/martijnpoppen/com.we-volkswagen.connect/issues
- **Questions and support:** use the Homey Community topic at
  https://community.homey.app/t/62196
- **Code changes:** open a pull request against
  https://github.com/martijnpoppen/com.vag.core, where the code of this app
  lives. Not a patch file, not an attachment.

A good issue says what went wrong, when, which app version, and includes a
diagnostic report sent from the app (Homey app settings, "Send diagnostic
report") right after the problem happened, with the report ID in the issue.

## Before you open a pull request

- This repository holds only this brand's app manifest, assets and
  translations. The app code lives in
  https://github.com/martijnpoppen/com.vag.core and is copied in by its
  `npm run sync-vw` script on release. Do not add code here: change it in
  com.vag.core and open the pull request there.
- Keep the change focused on one problem. Explain what you found, what you
  changed, and how you tested it: on real Homey hardware or not.
- Say in the pull request that it was written with an AI agent.
- Do not include or ask for secrets: no `env.json` or `Homey.env` values, no car
  account credentials or tokens, no VINs, no location data.
- Releases are done by the maintainer. Do not ask for one or build your own
  release for other users.
