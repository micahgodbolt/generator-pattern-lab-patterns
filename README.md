# Pattern Lab Patterns Generator

## Prerequistes 

- [Node.js](http://nodejs.org) installed
- [Yeoman](http://yeoman.io) installed by running: `npm install --global yo`
- Install this generator with: `npm install --global generator-pattern-lab-patterns`

## Useage

Navigate to a [Pattern Lab](http://patternlab.io) site, then `cd` into the `source/` directory. If you run `ls` and see the `_data/` and `_patterns/` directory, then you're in the right place. Finally, run this generator:

```bash
yo pattern-lab-patterns
```

**Pro Tip**: You can just run `yo` and it'll give you a list of all your installed generators which you can select & run. Much faster and easier to remember.

This will provide you a list of all the Pattern Bundles you can get (which is simply a list of folder we have in this repo under `app/templates/`). After chosing, it'll copy the patterns into your directory. This can be ran inside a pre-existing project and it can even be ran with other patterns already present! It'll ask you before overriting any file.

So, you may ask *What's a Pattern Bundle*? Well, we're simply referring to the `source/_patterns/` and `_source/_data/` folders and all their contained JSON and Template files (currently just Mustache, but other formats are easily added).
