# Markdown to .epub project template

[![conventional commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-yellow.svg)](https://conventionalcommits.org)

This is a template you can use if you ever need to generate an epub file from markdown code. If I was to write a novel I'd use it not to worry about formatting.

## How does it work

### Start a project

- Click on Use this template
- Give a name to your project
- Clone your project.

### Write your stuff

- Write a markdown in src/ folder (with the header)
- Make sure markdown linter is happy
- Modify the css to your convenience.

Optionally if docker is installed on your system you can test epub conversion with the makefile :

- Set `MARKDOWN_FILE = src/test.md` at the beginning of the file
- `make build` command results in an epub file generation in your target folder

### Release

- Check `.releaserc.yml` and `.github/workflows/publish.yml` files : replace .epub and .md file name and changelog title
- Push to main
- Once you're happy, go to github action to trigger a release.

The result is downloadable as the `E-pub-book` asset of the [last release](https://github.com/YOUR-PROJECT/releases/latest).

## Sematic release

The repo uses [Semantic release](https://github.com/semantic-release/semantic-release) for the commit messages.

## Pandoc

E-pub conversion made with [pandoc](https://pandoc.org/)
