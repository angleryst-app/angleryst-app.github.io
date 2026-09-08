# Angleryst Privacy Policy

**Effective August 1, 2026**

Angleryst is a fishing log that runs on your phone. It has no server, no
account, and no analytics. This policy describes exactly what the app does with
information, and it is written to be checkable against the app's source code
rather than to cover every hypothetical.

## The short version

- There is no account and no sign-in. The app never asks who you are.
- Your catch log stays on your phone. I never receive it and have no way to.
- One outside service is involved: a weather provider that receives the
  coordinates you are fishing at, and nothing else about you.
- No analytics, no crash reporting, no advertising, no tracking.
- Delete the app and every trace of your log goes with it.

## What stays on your device

Everything you enter lives in a single database file in the app's private
storage, which other apps cannot read:

- Catches: species, weight, length, your notes, the date and time, and the
  coordinates where you logged it.
- Blank trips, so the app can tell a slow day from a day you did not fish.
- The conditions snapshot captured with each entry: air temperature, barometric
  pressure and its trend, wind, cloud cover, chance of rain, moon phase, and a
  water temperature estimate derived from air temperature.
- Names and coordinates of any spots you save.
- Up to three rolling backups of that database, so a crash or a bad import
  cannot cost you your history.
- A cached copy of the most recent weather response, so switching screens does
  not refetch it.
- Your two app preferences — the theme and whether measurements read in US or
  metric units. Nothing about you, and nothing that leaves the device.

None of this is uploaded anywhere. Your notes in particular are never read,
analyzed, or transmitted by the app — they exist only for you to read back.

## What leaves your device, and who receives it

Angleryst makes network requests to exactly one place: **Open-Meteo**, a free
weather API, at `api.open-meteo.com` and — for catches older than about 92
days — `archive-api.open-meteo.com`.

Each request contains:

- the latitude and longitude you are asking about, at full GPS precision
- which weather variables are wanted, and for which date range
- unit preferences (Fahrenheit, miles per hour, local time zone)

That is the entire request.

Like any internet request, it also reveals your device's IP address to
Open-Meteo, which is unavoidable for any app that fetches anything. I mention
it because a policy that claimed "only coordinates are sent" would be leaving
something out.

What is **not** sent, ever: species, weights, lengths, your notes, spot names,
your catch history, your device identifier, an advertising identifier, or
anything else that could distinguish you from any other person requesting the
weather. Angleryst has no account with Open-Meteo and sends no API key, so
there is nothing tying one request to another or to you.

Open-Meteo's own terms and privacy statement:
<https://open-meteo.com/en/terms>.

## Location

Location is what makes the app work: it is how conditions get attached to a
catch, and the whole analysis rests on knowing what the weather was where you
were.

It is optional. If you decline the location permission, or your device has no
GPS, catches still save — you can pick a spot you have saved before, type
coordinates yourself, or log a catch with no location at all. You can revoke
the permission at any time in your device's Settings, and the app will fall
back to those same options.

Coordinates are sent to Open-Meteo at the precision your device reports. They
are stored on your phone with the catch.

## What Angleryst does not do

- No analytics or usage tracking of any kind.
- No crash or diagnostic reporting.
- No advertising, and no advertising identifiers.
- No third-party SDKs beyond the app framework itself and the weather request
  described above.
- No selling, sharing, renting, or disclosure of your information, because none
  of it reaches me in the first place.
- No access to your photos, camera, contacts, microphone, or calendar. Location
  is the only permission the app requests.
- No server holding your data, and therefore no server that can be breached and
  lose it.

## Your copy of your data

**Export.** The app exports your entire log as JSON and CSV and hands the files
to the system share sheet, so you can save them to Files, email them to
yourself, or put them wherever you like. The exported files are also written
into the app's private storage and stay there until the app is removed. Where
you send a copy from the share sheet is up to you and outside the app's
control.

**Import.** You can restore an export through the document picker, in either
JSON or CSV. Entries already present are skipped rather than duplicated, so
re-importing a backup is safe.

**Delete.** Any catch or trip can be deleted individually from within the app.
To remove everything at once, use **Settings → Delete all data**. That erases
every catch, blank trip and saved spot, and also removes the app's automatic
backups and the cached weather response — deliberately, so nothing recoverable
is left behind. The database is compacted afterwards, so the deleted rows are
not merely unlinked but actually released back to the filesystem. It cannot be
undone, so the confirmation tells you exactly how much is about to go. Your
theme and unit preferences are the one thing kept, since they describe the app
rather than your log.

Deleting the app removes everything too, preferences included: all of it lives
in the app's private storage and goes with it. There is nothing left on any
server, because there never was anything on one.

## Children

Angleryst is not directed to children under 13, and I do not knowingly collect
information from them. In practice the app collects nothing that identifies
anyone of any age.

## California residents

I do not collect, sell, or share your personal information, and I do not engage
in cross-context behavioral advertising or targeted advertising. No personal
information is disclosed to any third party for any business or commercial
purpose. The coordinates sent to Open-Meteo to retrieve a weather forecast are
the only information that leaves your device, and they are not retained by me
in any form.

Because I hold no personal information about you, there is nothing for me to
access, delete, or correct on request. Your data is entirely in your hands
through the export and delete features above.

## Availability

Angleryst is currently offered only in the United States App Store.

## Changes to this policy

If this policy changes in a way that matters, the effective date at the top
changes with it. This page is always the current version. Because the app has
no way to contact you, there is no notification to send — checking this page is
the only mechanism, which is another consequence of collecting nothing.

## Contact

Questions about privacy in Angleryst: **angleryst.app@gmail.com**
