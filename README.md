# SFP Carousel Public Staging

**Purpose: ONE job.** Hosts finished Instagram carousel PDFs so Canva's
"import from URL" can fetch them. Nothing else ever goes in here.

## Rules

1. **Carousel PDFs only.** No working folders, no exports, no "misc" dumps.
2. **Never copy a folder into this repo.** Copy individual named files.
   The 2026-07 incident happened because a folder was copied in and a
   patient referral came with it.
3. **Everything here is world-readable.** Assume anything committed is public
   forever, including in history.
4. `.gitignore` blocks patient-shaped filenames as a backstop. It is a safety
   net, not permission to be careless.

## Workflow

    cp <one-carousel>.pdf .
    git add <one-carousel>.pdf     # never `git add .`
    git commit -m "add <name>"
    git push

Then import: `https://raw.githubusercontent.com/Beau77bro/sfp-carousel-public/main/<name>.pdf`

## History
Replaces `sfp-carousel-canva-staging`, deleted 2026-07-27 after a patient
referral PDF was found in it. Do not repeat the pattern that caused it.
