# Enhancements – BITS Digital CodeForge V1.0 (Stage 2)

I asked one question: *what slows an instructor down, or makes them nervous, when they grade a course?* Each change below answers one of those problems. All 19 Stage 1 fixes are still in place and were tested again after these changes.

| # | Problem the instructor had | What I built | Why it helps |
|---|---|---|---|
| 1 | Setting grades meant juggling 16 dropdowns (a Min and a Max for each grade). One wrong value created a gap or an overlap. | **Cutoff-only editing.** You type just the lowest mark for each grade. The upper limit fills in automatically, and E always starts at 0. | Half the inputs, and gaps or overlaps can't happen at all. If a cutoff doesn't make sense (for example, A- set higher than A), that row turns red with a plain explanation and export is blocked. |
| 2 | The chart showed marks in 10-mark blocks, so you couldn't see where a boundary actually fell or who it affected. | **Colour-coded histogram.** There's one bar per mark, coloured by the grade it currently gets, with dashed cutoff lines and grade labels. You can **drag a cutoff line** on the chart to move it, and hovering over a bar shows the mark, the number of students and the grade. | You can see the effect of a cutoff on the class straight away. Dragging is quicker than typing when you're adjusting by eye, and the number boxes stay in sync. |
| 3 | The hardest grading decision is the student on 79 who misses an A by one mark. The old console gave no way to find them. | **Borderline tab.** It lists every student within 1, 2, 3 or 5 marks of the next grade, grouped by grade. A one-click button (e.g. "Lower A cutoff to 78") brings that group up if you decide to. | Puts the fairness decision in front of you before you export, not after a student complains. |
| 4 | There was no way to check a single student before finalising. | **All students table.** You can search by BITS ID, filter by grade, and sort by ID, mark or grade. It also shows how far each student is from the next grade. | You can spot-check anyone in seconds, for example when a TA asks about one student. |
| 5 | One click on "Finalize & Download" exported immediately, with no chance to check. | **Review before export.** Export opens a summary first: instructor, course, class average, the grade table with changed cutoffs marked, a warning if borderline students exist, and grades with no students. You then pick a format and download. | It stops accidental or unchecked exports, and gives one last look at the numbers that matter. |
| 6 | The CSV had no record of *how* the grades were decided. | **Excel export with an Audit sheet.** Sheet 1 has the grades. Sheet 2 records the instructor, course, source file, export time, time spent, the cutoffs used (and which were changed), the grade distribution, statistics and the borderline count. CSV is still available. | If grades are questioned later, the file itself shows who graded, when, and with which cutoffs. |
| 7 | A page refresh or an accidentally closed tab threw away all your work. | **Autosave.** Cutoffs are saved per course in the browser every time they change, and the instructor name is remembered. When you come back to a course you see "Restored your saved cutoffs… Last exported…", with a button to start from the defaults. | No lost work, and you can tell whether a course has already been exported. |

**Smaller improvements that came along the way:**

- Progress steps in the header (Upload → Set cutoffs → Review → Export).
- The course list shows student counts.
- A downloadable blank template.
- Inline messages instead of pop-up alerts.
- A standard-deviation stat.
- A layout that works on a phone with no sideways scrolling.
- Keyboard focus outlines, labelled inputs, and reduced-motion support.
- The grade colours are one violet shade that gets lighter from A to E, checked for colour-blind readability. Grade names are always shown next to the colour, so meaning never relies on colour alone.

**What I deliberately left out:** extra charts, themes and animations. They would add screen space without solving any grading problem.
