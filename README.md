# cs6200-notes

Bilingual (English / 日本語) lecture notes for **CS 6200 Graduate Introduction
to Operating Systems** (Georgia Tech OMSCS, Fall 2026), written as a
textbook-style summary of what the lectures cover.  Built with
[latex-lecture-notes-template](https://github.com/kinginu/latex-lecture-notes-template).

- **Read the latest PDFs in the browser** (rebuilt by CI on every push):
  <https://kinginu.github.io/cs6200-notes/> —
  [English](https://kinginu.github.io/cs6200-notes/notes-en.pdf) ·
  [日本語](https://kinginu.github.io/cs6200-notes/notes-ja.pdf)
- Local build: `make docker-all` → `en/build/main.pdf`, `ja/build/main.pdf`.
- `en/` English edition, `ja/` Japanese edition — same chapter files under
  `lessons/`, one chapter per lesson; `figures/` and `references.bib` shared.

## Status

Chapters appear here as soon as both editions are finished and pushed.

| # | Lecture | Lesson | en | ja |
|---|---|---|---|---|
| 1 | P1L2 | Introduction to Operating Systems | | |
| 2 | P2L1 | Processes and Process Management | | |
| 3 | P2L2 | Threads and Concurrency | ✅ | ✅ |
| 4 | P2L3 | Threads Case Study: PThreads | | |
| 5 | P2L4 | Thread Design Considerations | | |
| 6 | P2L5 | Thread Performance Considerations | | |
| 7 | P3L1 | Scheduling | | |
| 8 | P3L2 | Memory Management | | |
| 9 | P3L3 | Inter-Process Communication | | |
| 10 | P3L4 | Synchronization Constructs | | |
| 11 | P3L5 | I/O Management | | |
| 12 | P3L6 | Virtualization | | |
| 13 | P4L1 | Remote Procedure Calls | | |
| 14 | P4L2 | Distributed File Systems | | |
| 15 | P4L3 | Distributed Shared Memory | | |
| 16 | P4L4 | Datacenter Technologies | | |

The lesson structure follows the public Udacity course (ud923, P1L2–P4L4);
P1L1 is course logistics and has no chapter.

## Writing conventions

See [`docs/style-guide.md`](docs/style-guide.md).  In short:

- Textbook register: no lecture anecdotes or metaphors; scope limited to what
  the lectures cover.  Pointers to OSTEP and to the papers the lecture
  discusses go in the margin via `\source{}`.
- Every new term is introduced with `\term[reading]{word}[gloss]` so it lands
  in the index; [`glossary.tsv`](glossary.tsv) fixes the English index key,
  the Japanese term, its reading and the chapter that owns it.
- Numbers in worked examples are our own; **no project, problem-set, quiz or
  exam content is reproduced** (Georgia Tech honor code).
- Build a single chapter with `tools/chapter-check.sh en 07-scheduling`, or
  by opening it in VS Code (LaTeX Workshop builds the subfile alone).

## License

`format/` and the build files come from the template (MIT).  The notes
themselves (`en/`, `ja/`, `figures/`) are © kinginu and released under
[CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/).
