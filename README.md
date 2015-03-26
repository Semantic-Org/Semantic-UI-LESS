# LESS Distribution

This repository is automatically synced with the main [Semantic UI](https://github.com/Semantic-Org/Semantic-UI) repository to provide lightweight LESS only version of Semantic UI. The contents are identical to `src/` of the main repository.

You can view instructions on using LESS on [LearnSemantic.com](http://www.learnsemantic.com)

## Importing LESS

> LESS files do not contain vendor prefixes. If you are to use these files directly you must add them during your build step.

Before using source files you will need to create a `theme.config` by renaming `theme.config.example`, and a site folder by renaming `_site/` to `site/`

You can then import Semantic from your own LESS files:
```less
/* Import all components */
@import 'src/semantic';
```

To import individual components you will have to create a scope for each import using `& {}`
```less
/* Import a specific component */
& { @import 'src/definitions/elements/button'; }
```

### Config Files

filename | usage | Initial Name
--- | --- | ---
**theme.config** | config file that stores each element's current theme for LESS | theme.config.example
**site/** | folder storing all your site's variables and css overrides for each UI component | _site/

