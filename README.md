# Bank Senior Officer Exam Tracker (website)

A free, static website (plain HTML/CSS/JS - no build, no server, no libraries) to record your daily study and mock tests.
Subject -> Topic -> Subtopic dropdowns, dashboard, revision schedule, reports.

## Publish on GitHub Pages (free) - 5 steps
1. Create a new GitHub repository (e.g. `study-tracker`), public.
2. Upload **all files in this folder** (drag & drop the *contents*, so `index.html` is at the top level of the repo). Include the `.nojekyll` file and `.github` folder if your upload tool shows hidden files; they are optional.
3. Repo **Settings > Pages > Build and deployment > Source: "Deploy from a branch"**, Branch `main`, folder `/ (root)` > Save.
4. Wait about a minute. Your site is at `https://YOUR-USERNAME.github.io/study-tracker/`.
5. Open it on your phone/laptop and bookmark it.

## How your records are kept (important)
- Every change is **saved automatically** in your browser (localStorage). Refresh, close, reopen - everything is still there.
- Data stays **in that browser on that device**; it is never sent anywhere (private, free).
- Different browser/device, or clearing site data, = empty tracker. So use **Backup & Restore > Download backup (JSON)** weekly, and **Restore** on any device. Restore first downloads a safety copy of the current data.
- Keep using the same address (same GitHub Pages URL) - browsers keep data per website address.

## Daily use
Daily Log: Date > Subject > Topic > Subtopic (choosing a new Subject/Topic clears the dependent choices automatically) > hours, status, MCQs > Save.
Dashboard, Revision, Reports and Syllabus progress update instantly.

## Rules used (same as the Excel tracker)
- Subtopic **Completed** = at least one session marked Completed. Progress counts unique subtopics, never sessions.
- A session counts as study when it has Date, Subject, Topic, Subtopic and status In Progress / Completed / Review Required ("Not Started" = plan only).
- Next revision = latest session date + interval N (N = sessions logged for that subtopic, max 5; defaults 1, 3, 7, 14, 30 days), while the latest session has Revision Required = Yes or status Review Required.
- Streak = consecutive days with Actual Hours > 0 (continues from yesterday if today not logged yet).

## Edit the syllabus
Use **Syllabus > Add to syllabus** in the app (saved with your data), or edit `js/syllabus.js` (built-in framework, not an official syllabus - follow the official circular).

## Files
`index.html`, `css/style.css`, `js/app.js`, `js/syllabus.js`, `.nojekyll`, `.github/workflows/pages.yml` (optional).
