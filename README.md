## We are working on the next version of the Flex theme. See https://github.com/reflexjs/reflexjs

<div align="center">
<img src="./www/assets/images/logos.svg" width="300px" />
<h1>@arshad/gatsby-themes</h1>
</div>

<p align="center">
A collection of <strong>open source</strong>, <strong>well designed</strong>, <strong>highly customizable</strong> and <strong>100% free</strong> Gatsby themes for <em>blazing fast sites</em>.
</p>

<p align="center">
  <a href="https://github.com/arshad/gatsby-themes/blob/master/LICENSE"><img src="https://img.shields.io/npm/l/@arshad/gatsby-theme-phoenix.svg" alt="License"></a>
  <a href="https://github.com/arshad/gatsby-themes/pulls"><img src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg" alt="PRs welcome!" /></a>
  <a href="https://twitter.com/arshadcn"><img src="https://img.shields.io/badge/Follow-%40arshadcn-1da1f2" alt="Follow @arshadcn" /></a>
</p>

## Themes

### Flex

<p>
<a href="https://flex.arshad.io"><img src="https://img.shields.io/badge/demo-netlify-success" alt="Demo"></a>
<a href="https://www.npmjs.com/package/gatsby-theme-flex"><img src="https://img.shields.io/npm/v/gatsby-theme-flex.svg" alt="Version"></a>
</p>

Flex is a Gatsby theme that lets you build your site by writing simple components inside Markdown files.

<img src="https://arshad.io/uploads/gatsby-theme-flex.gif" />

### Phoenix

<p>
<a href="https://arshad-gatsby-example-phoenix.netlify.com"><img src="https://img.shields.io/badge/demo-netlify-success" alt="Demo"></a>
<a href="https://www.npmjs.com/package/@arshad/gatsby-theme-phoenix"><img src="https://img.shields.io/npm/v/@arshad/gatsby-theme-phoenix.svg" alt="Version"></a>
</p>

<p>A Gatsby theme that bundles a <strong>blog, portfolio, photography</strong> and <strong>podcast</strong>. It uses <strong>Tailwind CSS</strong> for theming and includes <strong>code highlighting with Prism, RSS feed, a dark mode</strong> and <strong>great typography</strong>.</p>

<img src="https://arshad.io/uploads/gatsby-theme-phoenix-screenshot.jpg" />

## Architecture

All included themes are composed themes, which means they make use of multiple core themes for core types and a child theme for styles and [latent component shadowing](https://johno.com/latent-component-shadowing). This architecture allows themes to be flexible and customizable.

The following diagram shows an example of theme composition for @arshad/gatsby-theme-phoenix.

![Theme composition](./www/assets/images/architecture.jpg)

As you can see, you can easily swap `@arshad/gatsby-theme-phoenix` with your own theme and styles, keeping all functionality unchanged.

## Core themes

The following core themes are available. They bundle core types and functionality. They include **no styles** and are meant to be **consumed by other themes or sites**. Use them to compose and build your own themes.

To learn more about theme composition, check out the [official docs](https://www.gatsbyjs.org/docs/themes/theme-composition/).

| Name                                                                                                                          | Version                                                                                                                                                                        | Description                                                                                                                          |
| ----------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------ |
| [`@arshad/gatsby-theme-core` ](https://github.com/arshad/gatsby-themes/tree/master/core/gatsby-theme-core)                    | <a href="https://www.npmjs.com/package/@arshad/gatsby-theme-core"><img src="https://img.shields.io/npm/v/@arshad/gatsby-theme-blog-core.svg" alt="Version"></a>                | Shared types and helpers for @arshad/gatsby-themes                                                                                   |
| [`@arshad/gatsby-theme-blog-core`](https://github.com/arshad/gatsby-themes/tree/master/core/gatsby-theme-blog-core)           | <a href="https://www.npmjs.com/package/@arshad/gatsby-theme-blog-core"><img src="https://img.shields.io/npm/v/@arshad/gatsby-theme-blog-core.svg" alt="Version"></a>           | Adds a `Post` type that you can use to build a blog. Includes post excerpt, featured image, tags/categories and paginated pages.     |
| [`@arshad/gatsby-theme-page-core`](https://github.com/arshad/gatsby-themes/tree/master/core/gatsby-theme-page-core)           | <a href="https://www.npmjs.com/package/@arshad/gatsby-theme-page-core"><img src="https://img.shields.io/npm/v/@arshad/gatsby-theme-page-core.svg" alt="Version"></a>           | Adds a `Page` type with MDX support. Includes code highlighting with prismjs.                                                        |
| [`@arshad/gatsby-theme-photo-core`](https://github.com/arshad/gatsby-themes/tree/master/core/gatsby-theme-photo-core)         | <a href="https://www.npmjs.com/package/@arshad/gatsby-theme-photo-core"><img src="https://img.shields.io/npm/v/@arshad/gatsby-theme-photo-core.svg" alt="Version"></a>         | Adds a `Photo` type that you can use to build a photography site.                                                                    |
| [`@arshad/gatsby-theme-podcast-core`](https://github.com/arshad/gatsby-themes/tree/master/core/gatsby-theme-podcast-core)     | <a href="https://www.npmjs.com/package/@arshad/gatsby-theme-podcast-core"><img src="https://img.shields.io/npm/v/@arshad/gatsby-theme-podcast-core.svg" alt="Version"></a>     | Adds a `Podcast` and `PodcastEpisode` types that you can use to build a podcast site. Podcast episodes are pulled from podcast feed. |
| [`@arshad/gatsby-theme-portfolio-core`](https://github.com/arshad/gatsby-themes/tree/master/core/gatsby-theme-portfolio-core) | <a href="https://www.npmjs.com/package/@arshad/gatsby-theme-portfolio-core"><img src="https://img.shields.io/npm/v/@arshad/gatsby-theme-portfolio-core.svg" alt="Version"></a> | Adds a `Project` types that you can use to build a portfolio site.                                                                   |

Click on the theme page to learn more about the core theme and how to use it.

## Usage

[Browse our free themes](https://github.com/arshad/gatsby-themes/tree/master/themes) or create your own. You can mix and match core themes to compose your Gatsby site.

### Example

To build a portfolio site with a blog, run the following command in your site.

```shell
yarn add @arshad/gatsby-theme-portfolio-core @arshad/gatsby-theme-blog-core
```

Then enable the themes in your `gatsby-config.js`

```js
// gatsby-config.js
...
  plugins: [
    `@arshad/gatsby-theme-blog-core`,
    `@arshad/gatsby-theme-portfolio-core`
  ]
...
```

To disable a core theme, run `yarn remove @arshad/gatsby-theme-name` and then remove it from your `gatsby-config.js` file.

## Support

Need help? Create an issue on the main repo [@arshad/gatsby-themes](https://github.com/arshad/gatsby-themes/issues) or ask me [@arshadcn](https://twitter.com/arshadcn).

## License

<a href="https://www.npmjs.com/package/@arshad/gatsby-theme-phoenix"><img src="https://img.shields.io/npm/l/@arshad/gatsby-theme-phoenix.svg" alt="License"></a>
