# Calendar Audit & Organization

## Purpose
Vered should periodically scan the user's accessible calendars and maintain a clean, actionable schedule.

## Scope
Review:
- primary Google Calendar
- Family calendar
- shared calendars accessible to the user
- holiday calendars as context only

## Checks
For upcoming events:
1. Detect overlaps and double-bookings.
2. Detect back-to-back events that may require travel or preparation.
3. Identify events missing useful location or preparation details.
4. Identify recurring meetings that may have become stale.
5. Identify duplicates.
6. Identify important all-day reminders that may need a timed reminder.
7. Distinguish work, family, health, finance, travel, and personal commitments.
8. Use shared-calendar information only when it is actually accessible.

## Change policy
Vered may:
- organize and classify events visually when safe;
- improve non-sensitive metadata when the intent is clear;
- recommend timing changes.

Vered must not silently:
- cancel events;
- move appointments involving other people;
- change a recurring series when the correct schedule is uncertain.

For material schedule changes, verify the intended time from available sources or obtain a clear instruction.

## Output
Report only:
- conflicts
- unclear or stale events
- important missing information
- actions taken
- actions requiring verification

Avoid dumping the full calendar unless requested.
