# Fitness Tracker

A single-page weekly fitness tracker built for phones. Weeks run Sunday to Saturday. Open `index.html` in any browser. There's nothing to install.

## What's on the main screen
- **Weekly summary**: a workout ring toward your weekly goal (3 by default), plus progress bars for eating, supplements, and steps
- **Today**: tap a day, then tap the big tiles to check off *Ate right*, *Supplements*, and *10K steps*. Dots under each day show what you hit, and a green outline means all three were done that day
- **Workouts**: tap the box to log a workout on the selected day. Tap the workout name to open its exercise list (sets, reps, weight, notes) and check off each exercise at the gym, then tap **Finish workout**
- **Weight**: enter your weight once a week and see your trend chart and change since last week
- **Past weeks**: workouts completed each of the last 8 weeks. Tap one to jump to that week

## Edit screen (✏️ Edit, top right)
- Add, rename, reorder, and delete workouts (☰ opens a workout's exercise list for editing)
- Change your weekly workout goal
- Fix or delete weight entries
- Set reminder times and add them to your calendar
- Back up and restore your data

## Reminders
In Edit → Reminders, set your supplement and nightly log times, then add them once:
- **iPhone Calendar**: opens both reminders as events that repeat daily with an alert. Tap **Add All**.
- **Google Calendar**: one link per reminder, each set to repeat daily.

The app also shows a banner when it's past your supplement time and you haven't checked supplements, and again at night if you haven't logged everything.

## Syncing steps from Apple Health
Web apps can't read Apple Health directly. An iPhone Shortcuts automation can send the day's step count to the tracker by opening
`https://<your-site>/index.html?steps=<number>`. The full steps are shown in Edit → Auto-sync steps. If the number is 10,000 or more, the 10K box is checked automatically. You can add `&date=YYYY-MM-DD` to log a different day.

## Putting it on your phone
1. Turn on GitHub Pages for this repo (Settings → Pages → Deploy from branch).
2. Open the Pages URL in Safari → Share → **Add to Home Screen**. It opens full-screen like an app.

Your data is saved in that browser. Use **Back up data** to move it to another device.
