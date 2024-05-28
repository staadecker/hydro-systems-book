# What's happening here?

This webpage contains all the code for the Hydro Systems Book available [here](https://staadecker.github.io/hydro-systems-book/). Here's how it works.

## Markdown

Inside the `src` folder there are a bunch of Markdown files (files that end in `.md`). Markdown is a ubiquitious and easy to learn text format for creating rich text directly from a plain text file. In fact, this `README.md` is written in Markdown. You can view the raw text file that generates **these** _effects_ [here](https://raw.githubusercontent.com/staadecker/hydro-systems-book/main/README.md). Spme useful resources to learn Markdown.

* A very [brief summary](https://rust-lang.github.io/mdBook/format/markdown.html) of the Markdown format, just enough to get writing.
* A [full tutorial](https://commonmark.org/help/tutorial/) of Markdown.
* A longer [cheat sheet](https://www.markdownguide.org/cheat-sheet/) with the syntax for things like tables!
* Google / ChatGPT is always your friend if you're unsure of the Markdown syntax for something.

## mdBook

So how do these markdown files get assembled into a book? For this we use mdBook() a convenient library that provides a command line utility (downloadable [here](https://github.com/rust-lang/mdBook/releases)) to generate a website from the .md files. Run `mdbook serve` to turn on the website locally and have it update as you write. When you upload ("push") your changes to this online repository, the live website will automatically be updated (re-"built").

The [documentation for mdBook](https://rust-lang.github.io/mdBook/index.html) is great and provides information on e.g. how to create new chapters.


## Steps to make edits to the book

1. Install [Git](https://git-scm.com/downloads).
1. Clone this repository by running `git clone https://github.com/staadecker/hydro-systems-book`. This will download the latest version to your local computer.
1. Write the book! I.e. make edits to the Markdown (`.md`) files in the `src` folder.
1. Save ("commit") your changes with `git commit -a -m "Some message describing the change"`
1. Upload ("push") your changes with `git push`. This will only work if you have write access permissions to the repository. (Those who don't can "fork" the repository, push their changes to their fork, and open a "pull request" to request that their changes get integrated into the main version).

## To-do List

* Find a better title than "Hydro Systems"
* Choose a license for the book
* Update the information in `book.toml` to ensure the metadata like the authors, book description, etc. are correct.
* Build some interactive stuff!