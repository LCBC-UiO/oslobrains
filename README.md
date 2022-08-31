# oslobrains

You need [hugo](https://gohugo.io/getting-started/installing/) installed to render the website.

You can then serve the site locally with

```sh
hugo serve
```

Everything in `content` mainly creates new pages or posts. 
Should be written in `md`.

Everything in `data` should be in json, yaml or toml, and are data that might be rendered in the pages.
https://gohugo.io/templates/data-templates/#:~:text=In%20addition%20to%20Hugo's%20built,root%20of%20your%20Hugo%20project.

[assets/scss/style.css](./assets/scss/style.css) is the scss to overwrite the existing stylesheet of the theme we use dynamically. 

Never, ever ever change files in the `themes/sometheme` dir, this will make the theme impossible to update when needed.
Any filepath that is identical to the subpaths of `themes/sometheme` will override the theme's files, and is the best way to go if we want to adapt the theme.
