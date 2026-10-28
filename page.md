
#4471 merged **412 reports** as one known bug. They are three problems.

Not one ticket. Three issues: parser (fixed), form hint (won't fix), one-day shift (open).

## What was merged

## The problems

1. **Parser reads dates month first: 374 reports.** The shared parser reads every date month
   first. Day-first tenants (11) get flipped dates. Fixed: `parse dd/mm for eu locales`. Issue 1.
2. **booking-v3 form hint: 33 reports.** On the form channel, copper.studio, alder.physio and
   pale.harbour see `MM/DD/YYYY` under the date field, so people type month first. Won't fix:
   the booking-v3 form was retired. Issue 2.
3. **One-day shift: 5 reports** (R-41202, R-41209, R-41236, R-41344, R-41620). The bodies
   describe a day moving, not a month flip, so the dd/mm fix does not cover them. The desk notes
   (`oneDayMove`) list them. Open. Issue 3.

The intake tag is a guess: 23 of the reports tagged `parser` belong to the hint problem.

## Lessons

- Group by tenant locale and form, not by the intake tag.
- A merged ticket can hold more than one bug. Count each once.
- A fix for one problem does not close the others.


_desk ref: shown by RenderStamp from the page signature (not computed here)._
