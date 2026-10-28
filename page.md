
#4471 merged **412 reports** as one known bug. They are two problems with two fixes.

Not one ticket. Two issues: parser and form hint.

## What was merged

## The problems

1. **Parser reads dates month first: 379 reports.** The shared parser reads every date month
   first. Day-first tenants (11) get flipped dates. Issue 1 in `kitek-dev/what-it-shows-4471`.
   Five of these (R-41202, R-41209, R-41236, R-41344, R-41620) describe a one-day shift, not a
   month flip. The desk notes record them, and they stay counted here.
2. **booking-v3 form hint: 33 reports.** On the form channel, copper.studio, alder.physio and
   pale.harbour see `MM/DD/YYYY` under the date field, so people type month first. Issue 2.

The intake tag is a guess: 23 of the reports tagged `parser` belong to the hint problem.

## Lessons

- Group by tenant locale and form, not by the intake tag.
- A merged ticket can hold more than one bug. Count each once.


_desk ref: shown by RenderStamp from the page signature (not computed here)._
