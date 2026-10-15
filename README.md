# SchoolRunbook course site

The student-facing course site, built with [mdBook](https://rust-lang.github.io/mdBook/) and published to GitHub Pages at https://schoolrunbook.github.io/course/.

Pages live in `src/`, and the sidebar order is set in `src/SUMMARY.md`. Every push to `main` rebuilds and publishes the site in about a minute.

To preview locally: `mdbook serve --open`.
