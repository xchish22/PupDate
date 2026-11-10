# Pupdate versioning protocol

Pupdate uses version numbers in the form **MAJOR.MINOR.PATCH**, for example `1.2.0`.

| Part | Goes up when… | Example | What users should do |
|---|---|---|---|
| **MAJOR** (first number) | A change that could break existing data or backups, or a big redesign that changes how the app works | `1.4.2` → `2.0.0` | Save a backup **before** updating |
| **MINOR** (middle number) | New features that work with existing data | `1.1.1` → `1.2.0` | Nothing, just enjoy |
| **PATCH** (last number) | Bug fixes, wording or small visual fixes, no new features | `1.2.0` → `1.2.1` | Nothing |

When a number goes up, the numbers to its right reset to 0 (`1.2.3` → `1.3.0`, `1.9.4` → `2.0.0`).

## Release checklist

Every release, however small:

1. **Pick the number** using the table above.
2. **Update the app** in `index.html`:
   - `APP_VERSION` = the new number
   - Add a new entry at the **top** of `VERSIONS` with the date and 1–3 short, plain-English bullet points. Settings shows the 3 newest versions, and the What's new pop-up shows the newest one.
   - Raise `DATA_VERSION` **only** for a MAJOR change to the saved-data format. Older copies of the app will then refuse newer backups instead of misreading them.
3. **Update `sw.js`**: set `CACHE` to `"pupdate-<new version>"`. This makes phones download the new files.
4. **Update `CHANGELOG.md`** with the same notes, in a little more detail if useful.
5. **Test** on a phone-sized screen: add a pet, save a backup, restore it, and check the new feature.
6. **Publish**: drag the `pupdate-app` folder onto your site's **Deploys** tab in Netlify.

## Saved data

- Data lives on each phone (browser storage). It isn't sent anywhere.
- Backup files include `version` (the data format, currently `1`) and `appVersion`.
- MINOR and PATCH releases must keep reading every older backup.
