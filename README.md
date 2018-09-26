# Status Technical Docs

This repo hosts the code for both [docs.status.im](https://docs.status.im) on the `master` branch (which builds and serves through `gh-pages`), and [dev-docs.status.im](https://dev-docs.status.im) on the `develop` branch.

There is an `edit` button on each page, which will take you directly to the document you need to edit on the `develop` branch. We can then allow a large group of people to push directly to `develop` and show their changes on the staging site when asking for review, which should smooth out and speed up the process considerably for everyone. `master` is protected, and will only have changes merged in from `develop` once accepted.

## Adding a New Page

If you want to add a page, rather than just edit, you'll need to make sure it appears on the sidebar and is accessible to everyone.

1. Add your page to `source/docs/<your_file_here>.md`
2. In `source/_data/sidebars.yml` add the appropriate text to the appropriate place.
3. In `themes/navy/languages/en.yml` edit the sidebar section to make sure that your new text in `sidebars.yml` is rendered correctly.
