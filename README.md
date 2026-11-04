# JCU research website starter

This is a starter site for the JCU research website theme. It uses the theme as a remote Jekyll theme, so project teams can edit Markdown content and publish through GitHub Pages.

## Setup

1. Rename this repository for your project.
2. Update `title`, `description`, `url`, and `baseurl` in `_config.yml`.
3. Edit `index.md` and `contact.md`.
4. Update `_data/navigation.yml` when you add or remove pages.

## Theme settings

The `theme_settings` block in `_config.yml` configures PacELF branding, fonts, and colours. Leave optional settings commented to use the theme defaults. Dark secondary backgrounds use explicit white text and link colours.

The JCU logo is provided by the theme by default. To add a project logo, add an image to `assets/images/` in this site and set `project_logo` in `_config.yml`.

## Homepage layout

The starter homepage uses `layout: landing-page`, which is the theme layout for polished landing pages driven by front matter. Edit the `hero` and ordered `blocks` list in `index.md` to customise the homepage. Blocks include `achievements`, `carousel`, `standard`, and `partner-logos`. Use `background: primary` or `background: secondary` on standard sections for coloured bands.

Use `sample-content/pages/landing-page-blocks.md` as a reference for the available full-width page blocks and optional fields.

## Sample content

The `sample-content/` directory is an exact copy of the pinned theme version’s sample directory, including filenames and supporting files. When updating the theme, replace this directory with the samples from the same version; keep the sample pages unchanged.

This starter includes optional sample content under `sample-content/`, plus sample images in `assets/images/`. Use these pages to see how theme configuration changes affect Markdown formatting, content blocks, galleries, logos, tables, colours, and responsive layouts.

When the project site is ready for real content, delete `sample-content/`, remove the `Sample Content Styles` section from `_data/navigation.yml`, and remove any unused sample images from `assets/images/`.

## Theme version

The site pins `jcu-eresearch/jcu-research-website-theme@v1.1.0` in `_config.yml`. Update this version deliberately and preview the homepage, contact page, samples, navigation, and library after each theme update.

Use `image_fit: contain` for the hero logo, and `image_shape: original` with `image_fit: contain` for diagrams, carousel maps, and book covers that should remain uncropped.

## Local preview

Install dependencies:

```bash
bundle install
```

Run the site locally:

```bash
bundle exec jekyll serve
```

Then open the local URL printed by Jekyll.

## GitHub Pages

For a project site at `https://USERNAME.github.io/REPOSITORY-NAME/`, set:

```yml
url: "https://USERNAME.github.io"
baseurl: "/REPOSITORY-NAME"
```

For an organisation or user site at `https://USERNAME.github.io/`, set:

```yml
url: "https://USERNAME.github.io"
baseurl: ""
```
