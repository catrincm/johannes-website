The repository for https://johannesstern.github.io/, the academic website for Johannes Stern

Created with [academic for hugo](https://sourcethemes.com/academic/)

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

To deploy:
- For truthandsemantics website, just push changes to the master branch on GitHub desktop. Netlify will automatically push it to truthandsemantics.netlify.app.
- For johannes-website you also need to run deploy.sh from terminal: `bash deploy.sh`. This will then push the changes from the johannes-website repo to johannesstern.github.io.
