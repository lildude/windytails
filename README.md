# WindyTails

A new Hugo theme that uses [TailwindCSS](https://tailwindcss.com/), its [typography plugin](https://tailwindcss.com/docs/typography-plugin), and a build setup using [PostCSS](https://postcss.org/) and PurgeCSS (when running the production build). This theme started from the base set out in <https://github.com/bep/hugo-starter-tailwind-basic>.

This setup can be used both as a starter project and a theme.

## As a Project

```bash
npm install
hugo server
```

## As a Theme

Import it into your project:

```bash
hugo mod init github.com/lildude/windytails
```

... and then run:

```bash
hugo mod npm pack
npm install
```

You need to add this to your `config.toml` (the stats are used by the CSS purging):

```toml
[build]
writeStats = true
```

Then run your project as usual.
