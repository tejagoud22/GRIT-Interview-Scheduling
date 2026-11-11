# GRIT Interview Scheduling (Prototype)

Round 1 assignment for AI Product Engineer. A prototype of an interview scheduling feature for GRIT, where students take a Level Clearance Interview to earn a Track Badge.

## What it does

- Eligible students book an interview slot from their dashboard, and can reschedule or cancel.
- Interviewers set and manage their availability, see their daily schedule, and record the outcome: pass, fail, or retake later.
- Students see their interview status and result on their dashboard. Badge and Miles stay locked until the result.
- The interview team sees which eligible students have booked and which haven't, against the number of open slots.

## Screens

- Student: home dashboard (before and after the result), slot booking
- Interviewer: daily schedule with outcome recording, availability manager
- Interview team: booked vs not-booked tracker
- Student messages: the key messages shown in the flow

Use the yellow preview bar on the Student tab to switch between before and after states.

## Interview states

Not eligible, Eligible, Booked, Needs rebooking, In progress, Passed, Failed, Retake later, No-show, Revoked.

## Key decisions

- Miles and Badge are released only on Pass.
- A slot is locked in one transaction so two students can't book the same slot.
- Cancellation window (24h) and cooldown after a fail (7 days) are assumptions and would be configurable.
- Every status change is logged with who made it and when.

## Run it

It's a single self-contained file with no build step. Open `index.html` in a browser, or view it on GitHub Pages: <paste your link here>

All data is sample data held in the browser tab and resets on reload.

## Docs

Write-up (states, edge cases, data model): <paste your doc link here>

## Author

Vasamsetti Teja
