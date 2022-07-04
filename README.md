The repository for https://johannesstern.github.io/, the academic website for Johannes Stern

Created with [wowchemy for hugo](https://wowchemy.com/)

# How to use:

Getting started
- Just download the repository from github.

A number of hugo commands are run from the terminal.
- Open terminal
- Locate to folder, e.g., `cd Documents/GitHub/johannes-website`. You can then run `cd ..` to return to the "GitHub" folder to then "cd" into the truthandsemantics-website.

To run hugo server which builds a local version of the site:
- In terminal run `hugo server`
- then it will give you the url to locate the website.

To create a new page:
- In terminal run `hugo new publication/name-of-publication`, or as appropriate.
- You can modify the archetype to change what's created by default. Duplicate file, e.g, `themes/academic/archetypes/publication/index.md` to `archetypes/publication/index.md` and modify.

Editing content:
- I suggest using atom editor.
- Most content is located in `content` folder. Some settings are in `config` folder.
- Don't edit files in `themes\academic`. To modify the theme create a \`local\` version of the folder from `themes\academic`. E.g. in `layouts` there's code that overwrites the theme.

To deploy, simply push changes to the master branch using GitHub desktop.
- For truthandsemantics website, this will then trigger Netlify to automatically do it.
- For johannes-website, it is running a github action, see `gh-pages.yml`


To update
- See https://wowchemy.com/docs/hugo-tutorials/update/
- Update `hugo-version` in `gh-pages.yml` for johannes-website.




----------
Troubleshooting

`Error: from config: failed to resolve output format "headers" from site config`
In the terminal type `open $TMPDIR`.
Simply delete the folder called `hugo_cache`
Then all should be fixed and you shoud be able to run `hugo server` now without problems.
See https://wowchemy.com/docs/hugo-tutorials/troubleshooting/#error-failed-to-resolve-output-format
