# Kuraz books

Sunday-school curriculum (ሥርዓተ ትምህርት) PDFs, Grades 1–10, used by the Kuraz app.

- `grade N/` — the books for each grade.
- `catalog.json` — the list the app reads: one entry per book with its grade, subject, page count, size and
  `pdfUrl` (the file's path in this repo). The app loads it from
  `https://raw.githubusercontent.com/HenokTade/Kuraz-books/main/catalog.json`.

To add or replace a book, put the PDF in its grade folder and regenerate `catalog.json` with `prepare_books.py`
(in the Kuraz project), then commit both. Phones pick up the change the next time the app opens.
