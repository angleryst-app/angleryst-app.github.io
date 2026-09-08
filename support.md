---
meta-description: Support and contact for Angleryst, a fishing log that keeps your data on your phone.
meta-viewport: width=device-width, initial-scale=1
title: Angleryst — Support
permalink: /support/
---

# Angleryst Support

## Contact

Email: <angleryst.app@gmail.com>

I read every message. Angleryst is written and maintained by one person, so
replies usually take a day or two, sometimes longer on a weekend.

**When reporting a problem, it helps to include:**

- your iPhone model and iOS version (Settings → General → About)
- the Angleryst version (Settings, at the bottom of the screen)
- what you were doing when it went wrong, and what you expected instead

Screenshots are welcome. Please don't send your export file unless I ask for
it — it's your catch log, and I'd rather not have a copy.

## Common questions

**Weather isn't loading for a catch.**
Angleryst fetches conditions from an outside weather service, so it needs an
internet connection at the moment you log. If you were out of signal, the catch
still saved — the conditions just weren't attached. Reception on the water is
the usual cause.

**Conditions are missing on an older catch.**
Historical weather comes from a different archive than the current forecast,
and that archive lags roughly three months behind. Catches from that in-between
window can come up empty. This is a limit of the weather source, not something
lost on your end.

**I don't want to share my location.**
Location is optional. If you decline the permission, you can still log catches
by picking a spot you've saved before, typing coordinates yourself, or logging
with no location at all. Conditions can't be attached without a position, since
weather is specific to a place. You can change your mind anytime in Settings →
Privacy & Security → Location Services → Angleryst.

**Water temperature looks off.**
It's an estimate derived from air temperature, not a reading from the water.
Treat it as a rough trend rather than a measurement — a thermometer will always
beat it, especially in spring and fall.

**How do I back up my log?**
Settings → Export writes your full log as JSON and CSV and hands it to the
share sheet, so you can save it to Files, email it to yourself, or put it in
whatever cloud storage you use. Angleryst also keeps three rolling backups on
the device, but those go away if the app does. An export you've saved somewhere
else is the only backup that survives losing the phone.

**How do I move my log to a new phone?**
Export on the old phone, save the file somewhere you can reach from the new
one, install Angleryst, then Settings → Import. Entries already present are
skipped rather than duplicated, so importing twice is safe.

**Can I get my data out in a normal format?**
Yes. The CSV export opens in Numbers, Excel, or Google Sheets. The JSON export
keeps everything, including the conditions snapshot on each catch, and is the
one to use for restoring into Angleryst.

**How do I delete everything?**
Settings → Delete all data erases every catch, blank trip, and saved spot,
along with the automatic backups and cached weather. It can't be undone, and
the confirmation tells you how much is about to go. Deleting the app removes
everything too.

**Can I switch between pounds and kilograms?**
Settings → Units toggles the whole app between US and metric. Existing entries
convert on display; nothing is rewritten.

**Is there an Android version?**
Not at the moment.

## Feature requests

Send them to the address above. I can't promise anything specific will get
built, but I'd rather hear what's missing than guess.

## Privacy

Angleryst has no account, no analytics, and no server. Full details are in the
[privacy policy](https://angleryst-app.github.io/).

---

Angleryst — Copyright © 2026
