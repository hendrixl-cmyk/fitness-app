# Fitness Tracker

A single-page weekly fitness tracker built for phones. Open `index.html` in any browser. There's nothing to install.

## What's on the main screen
- **Weekly summary**: a workout ring toward your weekly goal (3 by default), plus progress bars for eating, supplements, and steps
- **Today**: tap a day, then tap the big tiles to check off *Ate right*, *Supplements*, and *10K steps*. Dots under each day show what you hit, and a green outline means all three were done that day
- **Workouts**: tap a workout to log it on the selected day
- **Weight**: enter your weight once a week and see your trend chart and change since last week
- **Past weeks**: workouts completed each of the last 8 weeks. Tap one to jump to that week

## Edit screen (✏️ Edit, top right)
- Add, rename, reorder, and delete workouts
- Change your weekly workout goal
- Fix or delete weight entries
- Set reminder times and add them to your calendar
- Back up and restore your data

## Reminders
In Edit → Reminders, set your supplement and nightly log times, then tap **Add daily reminders to my calendar**. That downloads a `.ics` file with two repeating daily events that have alerts. Open it on your phone and add both. You'll get the alerts even when the app is closed.

## Syncing steps from Apple Health
Web apps can't read Apple Health directly. An iPhone Shortcuts automation can send the day's step count to the tracker by opening
`https://<your-site>/index.html?steps=<number>`. The full steps are shown in Edit → Auto-sync steps. If the number is 10,000 or more, the 10K box is checked automatically. You can add `&date=YYYY-MM-DD` to log a different day.

## Putting it on your phone
1. Turn on GitHub Pages for this repo (Settings → Pages → Deploy from branch).
2. Open the Pages URL in Safari → Share → **Add to Home Screen**. It opens full-screen like an app.

Your data is saved in that browser. Use **Back up data** to move it to another device.
