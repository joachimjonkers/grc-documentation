# Workday Organizer

The Workday Organizer is used to define your organization’s working calendar. This calendar is applied whenever a task series is planned using Repeat on → Work Day (for example, “the 10th working day of each month”). By configuring working days and holidays here, you control which days are counted as “working days” in those calculations.

You can access this configuration via Administration Controls → Workday Organizer.

### Holidays and Days off

Use Holidays and Days off to add specific dates that should not be considered working days (for example: public holidays, company-wide days off, or closure days).

* Click Add to create a new holiday/day off.
* Provide a name (so the date is recognizable in the list).
* Select the date.
* Use the Search field to quickly find existing entries.

All dates listed here are skipped when calculating Work Day scheduling.

### Working days of the week

Use Working days to define which weekdays are considered working days in your organization.

* Select the days that are working days (for example, Monday–Friday).
* Unselected days are treated as non-working days (for example, Sunday, or weekends in general).

This setting determines the baseline working week that Work Day scheduling uses, before holidays/days off are applied.

### How this affects Work Day scheduling

When a task series is configured to repeat on a Work Day, the system calculates the next occurrence by counting forward through the month using your Workday Organizer settings:

* Weekdays not selected under Working days are skipped.
* Holidays and Days off are skipped.
* If the selected work day number (e.g., 10) exceeds the number of available working days in a given month, the system schedules the task on the last working day of that month.

This ensures task scheduling stays consistent with your organization’s working calendar, even across months with different numbers of working days.



After updating holidays or working days, click Save to apply your changes.

Changes take effect for future Work Day calculations (and any series recalculation that depends on the working calendar).
