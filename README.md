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

> **Pro Tip**: You can just run `yo` and it'll give you a list of all your installed generators which you can select & run. Much faster and easier to remember.

This will provide you a list of all the Pattern Bundles you can get (which is simply a list of folder we have in this repo under `app/templates/`). After chosing, it'll copy the patterns into your directory. This can be ran inside a pre-existing project and it can even be ran with other patterns already present! It'll ask you before overriting any file.

**This project is in the very early stages, so the list will be pretty limiting for the moment.** However, the architecture is laid for the easy contribution of more Pattern Bundles.

So, you may ask *What's a Pattern Bundle*? Well, we're simply referring to the `source/_patterns/` and `_source/_data/` folders and all their contained JSON and Template files (currently just Mustache, but other formats are easily added).

## Contributing

No knowledge of Yeoman necessary!! Just fork this repo and make a new directory in `app/templates/` that contains it's own `_data/` and `_patterns/` directories! 

To test locally, run this from your repo root:

```bash
npm link
```

This will make your local repo the yeoman generator used. Then you can go elsewhere on your machine and test the generator by running:

```bash
yo pattern-lab-patterns
```

If all looks as you'd expect, then submit a Pull Request! Afterwards, you'll want to unset your local Yeoman generator by running this from your repo:

```bash
npm unlink
```

### Pattern Bundles Needed

- [ ] Prototyping toolkit
- [ ] Drupal 7 Forms
- [ ] Drupal 8 Forms
- [ ] A suggested starter set
