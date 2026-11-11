# Changelog

All notable changes to Pupdate. Numbers follow MAJOR.MINOR.PATCH (see VERSIONING.md).

## 1.4.0 — 2026-11-11
### Added
- **Vet summary** (Profile → Vet summary): one page with details, microchip, vaccines, medications, weights, recent vet visits, health notes, open questions and documents on file. Share it as a file (Messages, Mail, AirDrop) or print / save as PDF.
- **Documents**: photos or PDFs of the rabies certificate, CDC import receipt, vaccine records, invoices, insurance, CKC papers and lab results, stored on the phone. The border checklist links straight to them ("Show it").
- **Care routine**: nail trims, teeth, baths, ear cleaning and more, each repeating every few days with a Done button. Due items appear in Needs attention, and the bell adds a repeating reminder to your phone's calendar.
- **Health notes**: "Something's off" lets you tick what you noticed (vomiting, low energy, limping…), add details, and add it to your vet questions in one step.
- **Training**: 12 common commands plus your own, each tapped from Not started → Learning → Solid.
- **Socialization checklist**: 27 experiences (people, animals, places, sounds, handling, surfaces) with progress, and a reminder about the puppy window.
- **Milestones**: a photo timeline of the firsts, showing how old your pup was.
- **Expenses**: food, treats and toys, medication, insurance, supplies, gear, licence and training. Costs now combine appointments and expenses, by category and by pet.
- **Send to family**: send a pet (with photos and documents) to another phone. Importing combines records from both phones instead of overwriting.

### Changed
- Backups now include document photos and milestone photos.
- Restoring a pet that already exists combines the records rather than replacing them.

### Fixed
- Semicolons in calendar reminders weren't escaped, which could cut off the text.
- "1 days overdue" now reads "1 day overdue".

## 1.3.0 — 2026-11-10
### Added
- **Looping video** of your pet. In Add/Edit pet, choose a video from your Photos, and a slider picks which 3 seconds to use. It plays silently on a loop in the round picture on Home and Profile.
  - Stored compactly on the phone (about 200 KB per pet) and included in backups.
  - Stays still when iPhone "Reduce Motion" is on.
  - The first frame becomes the small picture if there's no photo. "Remove video" goes back to the still photo.
  - Deleting a pet also deletes its video.

### Fixed
- Reminders for shots that are already due now were set for a date that had already passed, so they never alerted. They're now set for tomorrow at 9 am as "Book: …".

## 1.2.1 — 2026-11-10
### Changed
- The app is renamed **Pupdate** (previously Pawlette): title, header, Home Screen name and backup file names.
- Saved pets and older Pawlette backup files keep working, because the internal storage names are unchanged.

## 1.2.0 — 2026-11-10
### Added
- **Calendar** tab with a month view. Tap any day to book a vet, grooming, training, daycare or boarding appointment. Coloured dots show which pet each appointment is for.
- **Costs**: a cost on each appointment, a "Log it" step after it happens, and totals for this month, this year and all time, broken down by type and by pet.
- **Reminders**: after booking, add the appointment to iPhone Calendar (as a file with a built-in alert) or Google Calendar. The reminder fires even when Pupdate is closed. Home shows a reminder banner for today and tomorrow.
- **Canadian vaccine schedule** for puppies and dogs under 2 years: core DA2PP and rabies, 1-year boosters, and lifestyle vaccines (Bordetella, leptospirosis, Lyme). Check off each shot with one tap (it's dated today, or with the usual date if it was given long ago). Next-due dates fill in automatically, and you can add them to your calendar.
- **Ask the vet** list: jot down concerns between visits, mark them asked, and record what the vet said. Open questions are added to the calendar note for vet appointments.
- **Crossing into the USA** checklist per dog: age of 6 months, microchip, CDC Dog Import Form (valid 6 months), and rabies certificate, plus what you need to come back to Canada.
- **Canadian Kennel Club** breed list (224 breeds) in the breed field, with the CKC group shown on the profile.
- **Settings** page (gear icon): What's new for the last 3 versions, units, backup & restore, and the version number.
- Heartworm and tick season note for Canada.

### Changed
- The Appts tab is now Calendar.
- Backup & restore moved from Profile to Settings.
- Backups record the app version, and a backup from a newer app is refused instead of misread.

## 1.1.1 — 2026-11-10
### Fixed
- One word on the welcome screen was still slanted.

## 1.1.0 — 2026-11-10
### Changed
- New rounded, easier-to-read font (Nunito).
- Softer pastel palette (mint, sky, peach, lavender), a sea-green accent and a new app icon.

## 1.0.0 — 2026-11-10
### Added
- Standalone web app with no account needed. Data stays on the phone.
- Works offline and installs to the Home Screen.
- Backup to a file and restore from a file.
- Growth chart, vaccines, medications, vet visits, appointments and pet profiles.

## 0.1.0 — 2026-11-10
- First prototype, hosted on Claude, which needed a Claude account.
