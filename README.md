![Banner](banner.png)

## What this is

A short, self-contained introduction to LaTeX, the typesetting system
used across mathematics, computer science, and the sciences to produce
clean documents (especially ones full of equations). The primer assumes
**no prior experience with LaTeX or any programming language**.

It walks through six worked examples, each isolating one concept, and
ends with a capstone: a complete assignment solution you could actually
hand in.

LaTeX is different from a word processor. You don't drag things around a
page; you *describe* the document in a plain-text file, and LaTeX lays
it out for you. That feels strange for about an hour and then becomes
the reason people never go back.

## Who it's for

- Students whose courses expect assignments typeset in LaTeX
- Anyone writing something equation-heavy: a math assignment, a lab
  report, a thesis
- Anyone who has seen `??` or a wall of red errors and bounced off

## Before you begin

We're using **Overleaf**, so there is nothing to install.

1. Go to overleaf.com and make a free account (your Ontario Tech email
   works).
2. Create a new blank project, or upload the `.tex` files from this
   primer.
3. Open a file and press **Recompile**. The PDF appears on the right.

Overleaf compiles in the cloud and updates the preview as you go, so you
never touch a command line. Everything in this primer runs there
unchanged.

## The files

| File | Topic | What you'll be able to do |
|---|---|---|
| `ex1.tex` | The document skeleton | Set up any document and a title |
| `ex2.tex` | Text, sections, characters | Format text; escape special symbols |
| `ex3.tex` | Math mode | Typeset equations, fractions, sums |
| `ex4.tex` | Lists and tables | Lay out itemized lists and tables |
| `ex5.tex` | Theorems and proofs | Write definitions, theorems, proofs |
| `ex6.tex` | Figures and references | Add figures; cross-reference by number |
| `proj.tex` | Capstone project | Typeset a full assignment solution |

Work through them in order. Each example assumes the ones before it.

Each file is a **complete document** — open any one, press Recompile,
and it produces its own PDF. In Overleaf, keep each in its own project,
or set the file you're working on as the main document.

## How to use the primer

Reading LaTeX is not the same as understanding it. Because there's no
console output to predict, the loop is visual:

1. Read the file and picture what the finished page will look like.
2. Recompile. Compare the PDF to what you pictured.
3. Where you were wrong, that gap is the thing worth studying.
4. Change something — a symbol, a section, a table cell — and picture
   the result again before recompiling.

Breaking the examples on purpose is encouraged. When a compile fails,
Overleaf points at a line number and shows a message; learning to read
those early will save you more time than anything else in this document.

## The capstone project

`proj.tex` describes a complete two-page assignment solution that pulls
every concept together:

- Title block → Ex1
- Sections and intro → Ex2
- A numbered equation and an aligned derivation → Ex3
- A list and a results table → Ex4
- A definition, theorem, or proof → Ex5
- A captioned figure, cross-referenced by number → Ex6

Build it section by section, recompiling as you go. Don't write the
whole thing and compile it for the first time at the end.

## Errors you will probably hit

**`Undefined control sequence`**: a mistyped command, or one that
lives in a package you haven't loaded. Check the spelling, then check
that the right `\usepackage{...}` is in your preamble.

**`Missing $ inserted`**: you used a math symbol (like `^`, `_`, or a
Greek letter command) outside of math mode. Wrap it in `$...$`.

**The rest of a line vanishes**: you typed a literal `%`, which starts
a comment. Escape it as `\%`. The same applies to `$ & _ # {}`.

**Wrong-looking quotation marks**: don't use the `"` key. Open with two
backticks and close with two apostrophes: `` ``like this'' ``.

**A reference shows up as `??`**: the number hasn't resolved yet.
Overleaf normally runs enough passes to fix this on its own; if a `??`
lingers, press Recompile once more. (This is the "two compilations"
problem that trips people up in a local setup — Overleaf mostly handles
it for you.)

**A stray `&` or missing `\\` breaks a table or equation**: every cell
in a row is separated by `&`, and every row ends with `\\`. Miscount
either one and the environment won't compile.

## Getting help

Student Learning Support offers:

- **1:1 appointments** (bookable on QuadC)
- **CS Primers sessions** (bookable on QuadC)
- **Math Study Hall**

Bring your `.tex` file (or share the Overleaf project) and the exact
error message. "It won't compile" is harder to help with than the line
Overleaf flagged.

## About

Written by Benjamin Fedoruk, Subject Specialist in Mathematics and
Computer Science, Teaching and Learning Centre, Ontario Tech
University.

benjamin.fedoruk@ontariotechu.ca

Last updated: July 22, 2026
