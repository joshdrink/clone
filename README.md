# Clone

A lightweight, themeable design system.

Produced at [Talent Cloud](https://talent.canada.ca/).

### Getting Started

#### CDN

Coming Soon

Note: While using this version of Clone makes updates seamless, using the CDN version of Clone locks you into the theme associated to the CDN link unless you manually override styles in your project.

#### NPM

Clone is built in a way that allows you to theme the aesthetic of the system without the need to alter Clone's source files. This means that you'll be able to update Clone without any worry of losing or modifying your changes. All theming will occur in your project's root Sass directory and pull Clone's primary `.scss` file from `node_modules`.

While it doesn't matter how your project compiles Sass, theming Clone requires that your project be running [Sass](https://sass-lang.com/) and [Autoprefixer](https://github.com/postcss/autoprefixer).

Clone uses [Gulp](https://gulpjs.com/) to manage dependencies. If you haven't already, install Gulp globally by running `npm install gulp-cli -g` and `npm install gulp -D` in your terminal.

1. From inside your project, run `npm install clone-design`
2. Create a `.scss` file inside of your Sass directory that has the following:

```
// =============================================================================

    // My Custom Clone Theme
    // Please note that Clone must be included last, after all of your custom variables.

// =============================================================================

// Custom Variables

    // All available custom variables can be found at https://github.com/joshdrink/Clone/blob/dev/app/scss/core/_defaults.scss

// Include Clone

    @import "../node_modules/clone-design/app/scss/clone";
```

### Usage

Clone uses HTML5 custom data attributes to allow for easy, standardized, namespaced access to styles. Clone data attributes are prefixed with `data-clone` and in some cases, allow direct manipulation of styles. The following are Clone's current data attributes:

#### Accordion

Usage: `data-clone-accordion="OPTIONS"`

Accordion attributes are used exclusively to define the moving parts of an accordion:
- `data-clone-accordion="object"`
- `data-clone-accordion="trigger"`
- `data-clone-accordion="content"`
- `data-clone-accordion="icon--add"`
- `data-clone-accordion="icon--remove"`

#### Alert

Usage: `data-clone-alert="ALERT-TYPE"`

#### Alignment

Usage: `data-clone-alignment="TEXT-ALIGNMENT"`

#### Backgrounds

Usage: `data-clone-background="THEME-COLOUR(ALPHA-VALUE)"`

#### Borders

Usage: `data-clone-border="ORIENTATION(THICKNESS, STYLE, THEME-COLOUR)"`

#### Buttons

Usage: `data-clone-button="STYLE(THEME-COLOUR)"`

#### Carousels

Usage: `data-clone-carousel="OPTIONS"`

#### Containers

Usage: `data-clone-container="STYLE"`

#### Fonts

Usage: `data-clone-font="STYLE"`

##### Font Colour

Usage: `data-clone-font-colour="THEME-COLOUR"`

##### Font Style

Usage: `data-clone-font-style="STYLE"`

##### Font Weight

Usage: `data-clone-font-weight="NUMBER/VALUE"`

#### Grid & Grid Items

Usage (Grid): `data-clone-grid="OPTIONS"`

Usage (Grid Items): `data-clone-grid-item="OPTIONS"`

#### Headings

Usage: `data-clone-heading="HVALUE"`

#### Margins

Usage: `data-clone-margin="ORIENTAION(AMOUNT)"`

#### Padding

Usage: `data-clone-padding="ORIENTAION(AMOUNT)"`

#### Radius

Usage: `data-clone-radius="STYLE"`

#### Visibility

Usage: `data-clone-visibility="VALUE"`

You can find a list of default variables [here](https://github.com/joshdrink/Clone/blob/dev/app/scss/core/_defaults.scss).

### Dependency Checklist

[] jQuery
[] Slick Carousel
