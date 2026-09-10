# Space Wolves IND Management

A windows application used by members of the Space Wolves IND corporation.

Character, industry and corporation data straight from CCP's ESI, plus the
corp's own Alliance Auth — structures, the forum, moons and mining taxes — in
one window, next to the game.

**[⬇ Download the latest release](../../releases/latest)**

---

## What it does

- **Dashboard** — who you are, where you are, what you are flying, what you are
  worth, on a widget grid you arrange yourself.
- **Industry** — jobs in flight, your blueprints, and what any blueprint in the
  game costs to build against what it sells for.
- **Fleet Commander** — live fleet composition: logistics, tackle, command, and
  what the fleet is short of.
- **Intel alerts** — watches an in-game intel channel and puts a banner over
  EVE when something is called within your chosen jump range.
- **Assets, Wealth, Finances, Skills, Killboard, Mail, Planetary Interaction,
  Calendar, Faction War**, and a map of New Eden that works offline.

## Installing

1. Download the `.exe` from [releases](../../releases/latest).
2. Run it. Windows SmartScreen will warn about an unrecognised publisher —
   **More info → Run anyway**. The installer is not code-signed; a certificate
   costs more per year than this project spends on everything else.

<img width="526" height="490" alt="image" src="https://github.com/user-attachments/assets/baa63800-7a22-4624-bb63-34331b19dc60" />

   
4. Click **add character** and log in through EVE SSO.

The login opens **your own browser**, never a window inside the app. CCP asks
that third-party tools do not put a login form in an embedded window, and an
embedded window could read your password. The app never sees it — EVE hands back
a token, and that token stays on your PC.

## Requirements

- Windows 10 or 11
- An EVE Online account, and membership of Space Wolves ind.
- *Optional:* an Alliance Auth API key, for the forum, structures, moons and
  mining taxes. Ask a director. Everything else works without one.

**Characters from outside the corporation cannot be added.** This is built for
one corp, and it says so rather than letting an outsider add a character and
find half the app empty.

## Your data stays yours

- **ESI tokens are stored on your PC**, encrypted with Windows' own credential
  store, and are never sent anywhere except to CCP.
- **The app installs nothing by itself.** When there is a new version it tells
  you and opens the download — a tool holding your ESI tokens should not be
  quietly replacing its own code.
- Corporation data is read with **your** character's in-game roles. If you are
  not a director, CCP refuses the request; the app is not deciding what you may
  see, EVE is.

## Something wrong?

Post in the corp forum or the Discord. Include the version number from the
bottom of the sidebar.

## Source

This repository holds the releases and this page. The source is kept in the
corp's private Gitea.

Built with [EVE-CARBON](https://github.com/mcpanayides/EVE-CARBON) by
Mia Christina Panayides as a design reference — the look and the flow are its
work, followed with admiration; the code is our own.

---

*Author: Tenaya Masai. All EVE Online related materials are property of CCP hf.
This is a third-party tool and is not endorsed by CCP.*
