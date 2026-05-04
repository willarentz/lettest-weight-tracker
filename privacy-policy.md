# Lettest – Privacy Policy

_Last updated: 2026-04-18_

Lettest is a weight-tracking app for iPhone and iPad. This policy explains, in plain language, what data Lettest handles and what we do (and don't do) with it.

## The short version

- Lettest stores **only what you log**: your weight entries, your goal, your unit preference, your optional profile (sex, date of birth, height).
- Your data is stored in your **private iCloud database** and on your devices. It never reaches our servers — we don't have any.
- Lettest reads body-weight and body-fat samples from **Apple Health** only if you grant permission, and writes back the entries you log so other Health-aware apps can use them.
- We don't use analytics. We don't use ad SDKs. We don't track you across apps.

## What data Lettest handles

| Data | Where it lives | What we do with it |
|---|---|---|
| Weight entries (date, weight in kg, optional body fat %) | Your private iCloud database (CloudKit) and locally on your devices | Display them, average them, render charts |
| Goal (target weight, target date, weekly rate) | Same as above | Compute on-track / off-track / ahead state |
| Unit preference (kg or lb) | Same as above | Format the display |
| Profile (biological sex, date of birth, height) | Same as above | Compute your BMI healthy range and suggested target |
| Apple Health samples (read) | Apple Health | Imported into your Lettest history; we never see them |
| Apple Health samples (write) | Apple Health | New entries you create are written back so other Health apps see them |

## What Lettest does not do

- We do not collect analytics. There is no third-party SDK in this app.
- We do not show advertising.
- We do not transmit your data to any server we control.
- We do not sell your data. We could not — we don't have it.
- We do not require an account, an email address, or a sign-in.

## How sync works

Lettest uses Apple's CloudKit. Your weight history is stored in the **private database** of your iCloud account. Apple manages the storage; only your devices, signed in to your iCloud account, can read it. We have no access to it.

If you sign out of iCloud or disable iCloud Drive on your device, Lettest falls back to local-only storage. Your data is then on the device only and won't sync.

## HealthKit details

If you grant Apple Health permission:

- **Read access:** body weight (`HKQuantityType.bodyMass`), body fat percentage (`HKQuantityType.bodyFatPercentage`), date of birth, biological sex, height. Used only to populate your history and prefill your profile.
- **Write access:** body weight (`HKQuantityType.bodyMass`). Each entry you create in Lettest is written back so other Health-aware apps see it.
- All HealthKit access happens locally on your device. Apple's HealthKit framework enforces this; we cannot bypass it even if we wanted to.

You can revoke HealthKit access at any time in Settings → Health → Data Access & Devices → Lettest.

## Children

Lettest is not directed at children under 13. If you are a parent or guardian and believe your child has used Lettest and you wish to delete their data, simply uninstall the app from their device and remove the data from iCloud (Settings → Apple ID → iCloud → Manage Storage → Lettest → Delete Data).

## Data retention and deletion

Your data lives in your iCloud account for as long as you keep the app installed and your iCloud is active. You can delete individual entries at any time from the History view.

To remove **all** Lettest data:
1. Uninstall the app from each device.
2. In iOS Settings, go to Apple ID → iCloud → Manage Storage → Lettest → Delete Data.

This is a complete, irreversible deletion.

## Changes to this policy

If we ever update this policy, the new version will be posted at the same URL with an updated date at the top. We will not change Lettest to collect more data than this policy describes without prior notice.

## Contact

For questions, bug reports, or data-deletion requests, please open an issue on our public tracker:

**[github.com/willarentz/lettest-weight-tracker/issues](https://github.com/willarentz/lettest-weight-tracker/issues)**

Issues are visible to anyone with the link — please don't include private personal information in them.
