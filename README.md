# singgah

a sortable train-options table for a trip, on github pages. phone-first. it is a reading aid, not a booking site: seats and fares are not checked live.

live site: https://vanipy.com/singgah/

first trip: jakarta to jogja for PyJogja (sat 5 dec 2026, 09:00-17:00 WIB, Garuda Spark Innovation Hub, Mlati, Sleman). includes the overnight, day-train-plus-hotel and cheapest combos, and flags which trains arrive before the event or leave before it ends.

## what is in the data

public timetable information only: train, class, stations, times and indicative fares, each with a note and a source link. nothing personal, no ticket or booking details.

- schedule: valid from 1 dec 2026, from detik and 168railway (links on the page).
- fares: indicative. Taksaka 34 is "Rp680k and up", Progo 300 about Rp330k from a 4 nov listing, Senja Utama about Rp590k. the Taksaka 31 return fare is an assumption (same as Taksaka 34). other fares were not found and show as n/a.
- Senja Utama Yogyakarta 196: arrival time not found.
- nothing was checked live. confirm seats and prices on https://booking.kai.id/ before relying on them.

## add another trip

edit `data/trips.json` and add an object to `trips` (copy the first one): `event`, `legs` (each with `dir` out/back, dates, times, price or null, note), and `combos` (lists of leg ids). the page picks it up in the trip menu, or open `?trip=<id>`. open a pull request or just edit.

## license

agpl-3.0. see LICENSE.

---

Built with AI assistance (Instinct and others). Not everything has been reviewed by Irvan.
