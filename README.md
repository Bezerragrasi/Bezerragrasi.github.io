# Grasiele R.Bezerra's Website

This is my personal Website.

## Credits

This site is built using [GitHub pages](https://pages.github.com/) and
[Jekyll](https://jekyllrb.com) and is based on the [*Feeling Responsive*][1]
theme and on the [Patricia Ternes' website][2].

## Development

The main content of this website is organized in data yaml files (`.yml`) at `_data/`
directory, and markdown files (`.md`) at `pages/` directory.

When new content is added in the `main` branch, a *GitHub action*
(`.github/workflows/merge-schedule.yml`) is automatically executed. This action
converts all the content into an `html` website.

[1]: http://phlow.github.io/feeling-responsive/
[2]: https://github.com/patricia-ternes/patricia-ternes.github.io
