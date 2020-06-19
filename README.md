# Shopift Bootstrap Theme

A Shopify theme with Bootstrap 4 fully integrated across all theme pages. Derived from the (now deprecated) [Slate Bootstrap Theme](https://github.com/neckerson/slate-bootstrap-theme).

This is the theme I wish had been available when I was rolling my own
integration of Bootstrap 4 into a custom Shopify store. You should be able to
upload and manage the theme files easily with [Theme
Kit]{https://shopify.github.io/themekit/}.

[Theme Preview](https://slate-bootstrap-theme.myshopify.com)

I've started with the base
[Shopify/skeleton-theme](https://github.com/Shopify/starter-theme) and brought
over most of the ```/src``` directory of
[Shopify/starter-theme](https://github.com/Shopify/skeleton-theme), and some of
```src/styles```. These default Shopify styles are being gradually refactored
out of the theme as I have time. PRs welcome!

For responsive image loading, use the ```responsive-image``` &
```responsive-bg-image``` snippets. They pair well with Bootstrap's responsive
classes, and the lazyloader dependancy is built into the theme.

### Theming

Body background and text color can be set via the Shopify theme editor panels,
but other changes should be made with Bootstrap's built-in Sass variables,
allowing global style preferences, easy theming and component changes.

In ```src/styles/variables.scss``` you will find examples of customization
already done, with the primary and secondary colors changed to different
Bootstrap 4 color variables. You could experiment with other changes, such as
adding ```$enable-rounded: false;``` to variables.scss and deploying the theme.
For more examples, see the Bootstrap 4 [theming
documentation](https://getbootstrap.com/docs/4.0/getting-started/theming/).

### Typography

This theme is intended to be used with Montserrat Bold for headings and
Harmonica Sans for body text. Both of these can be set using the Shopify admin
theme editor. You may need to make adjustments in typography.scss if other font
pairings are used.

### jQuery & Webpack
Because Bootstrap requires jQuery, additional setup is required in
```theme.js```. For discussion, see Webpack issue
[#4258](https://github.com/webpack/webpack/issues/4258).

To add plugins to the theme, such as
[jackmoore/zoom](https://github.com/jackmoore/zoom), take a look at [this
gist](https://gist.github.com/neckerson/fd24e76e5c3f38d5aef83baadd09d28b) which
is implemented in ```theme.js```. Image zoom is implemented in
sections/product.liquid.

## Contributing

For help on setting up the repository locally, building, testing, and
contributing
please see
[CONTRIBUTING.md](https://github.com/neckerson/slate-bootstrap/blob/master/CONTRIBUTING.md).

## Code of Conduct

All developers who wish to contribute through code or issues, take a look at the
[Code of
Conduct](https://github.com/neckerson/slate-bootstrap/blob/master/CODE_OF_CONDUCT.md).

## License

This theme is derived from the Shopify Skeleton theme, which is Copyright © 2018
Shopify. See
[LICENSE](https://github.com/Shopify/skeleton-theme/blob/master/LICENSE) for
further details.



