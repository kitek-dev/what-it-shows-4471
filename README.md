# what-it-shows-4471

Ticket #4471 (412 merged date reports) split into problems. Issues:

1. Parser reads day-first dates month-first: 379 reports (5 footnoted as one-day shifts)
2. booking-v3 form hint says MM/DD/YYYY: 33 reports

Issue 3 (one-day shift) was folded into issue 1, as the desk counts them where filed.

The kb page is `src/routes/kb/incidents/4471-split/+page.svx`; its rendered text is in `page.md`.
