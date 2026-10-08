# Workday Countdown (GitHub Pages)

A fullscreen, clock-synchronized work/break timer for a managed Chrome kiosk.

## Schedule

- Work: 15 minutes
- Break: 5 minutes
- Workday: 6:00 AM–11:00 PM, using the kiosk device's local time zone
- The last block starts at 10:40 PM and runs for 20 minutes, so the workday ends on work at exactly 11:00 PM.
- Outside 6:00 AM–11:00 PM, the screen displays an after-hours message.
- The timer recalculates from the system clock, so a refresh or restart does not reset the schedule.

## Publish with GitHub Pages

1. Create a GitHub repository, for example `workday-countdown`.
2. Upload `index.html` to the repository root.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Choose the `main` branch and `/ (root)`, then click **Save**.
6. Wait for GitHub Pages to publish and open the provided URL on the kiosk device.
7. Configure managed Chrome to open that URL in fullscreen/kiosk mode.

## Notes

- The timer uses the device's local time. Set the kiosk device to the correct time zone and enable automatic time synchronization.
- No server, account sign-in, database, or external JavaScript library is needed.
- To change the workday or durations, edit the constants near the top of the script in `index.html`.
