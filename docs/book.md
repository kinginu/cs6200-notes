# Book profile

Everything that is specific to **this** book.  The generic rules are in
[`style-guide.md`](style-guide.md); writers and reviewers read both.  Fill
in every field when you create a book from the template, and keep it
current.

## Identity

- **Title**: Graduate Introduction to Operating Systems — Lecture Notes
  (CS 6200, Georgia Tech OMSCS, Fall 2026)
- **Kind**: course notes
- **Field**: operating systems
- **Chapter label**: Lesson  <!-- class default ("lesson") -->

## Source material

What each chapter summarizes, in the order the chapters follow.

- **Primary source**: the Georgia Tech CS 6200 lectures, whose lesson
  structure follows the public Udacity course ud923 (P1L2–P4L4; P1L1 is
  course logistics and has no chapter).
- **Version pinned**: not applicable (recorded lectures).
- **Unit list**: `docs/syllabus.json` (one entry per chapter; `lecture`
  gives the lesson code, e.g. P2L1; video-level titles are not recorded).
- **Reference in `\source` and `\lessoninfo`**: the lesson code and the
  topic, e.g. `video={P2L1}` and `\source{P3L1, preemptive scheduling;
  OSTEP ch.~7.}`.
- **Textbook / reference**: Arpaci-Dusseau & Arpaci-Dusseau, *Operating
  Systems: Three Easy Pieces* (bib key `ostep`; cite as "OSTEP ch.~4");
  Silberschatz, Galvin & Gagne, *Operating System Concepts*, 10th ed.
  (`silberschatz2018`; "Silberschatz et al.\ ch.~3").
- **Papers the source discusses**: listed per chapter in `bib/<slug>.bib`
  (e.g. `birrell1984` for RPC, `nelson1988` for Sprite, `li1989` for DSM).

## Code

- **Language in listings**: `language=C` (`language=Java` where the lecture
  shows Java, e.g. RMI).
- **Conventions**: C with POSIX threads (`posix2017`).

## Excluded

Never include (the reviewers treat any of it as a major issue):

- quiz, exam, homework and project questions, numbers and answers of the
  course (honor code);
- the course projects and problem sets.

## Real-world numbers

Typical kinds of numbers worth adding in margin notes (style guide §3.1),
and where they come from:

- context-switch, system-call and page-fault costs, page and TLB sizes —
  OSTEP, Silberschatz et al., the papers cited in the chapter;
- RPC and file-system latencies, datacenter scale — the papers the lecture
  discusses (`bib/<slug>.bib`).

## Reference chapters

Chapters whose style, density and macro use are approved and should be
imitated by new chapters (both editions):

- `en/lessons/01-introduction-to-operating-systems.tex`,
  `en/lessons/02-processes-and-process-management.tex`,
  `en/lessons/03-threads-and-concurrency.tex` and their `ja/` mirrors.
