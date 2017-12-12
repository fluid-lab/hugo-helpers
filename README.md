# Hugo Helpers

A collection of shortcodes that generate accessible HTML for Hugo websites.

## Installing

Put a copy of the shortcodes into the `layouts/shortcodes/` directory in your Hugo site, or in the Hugo theme.

You can do this by downloading a zip file and extracting the contents into the `shortcodes` directory, or by cloning this repository into your `shortcodes` directory:

```
git clone https://github.com/fluid-lab/hugo-helpers ./layouts/shortcodes
```

*NOTE:* In Hugo, shortcodes only work within the `shortcodes/` directory. Nesting shortcodes in subdirectories will not work.

Be careful to rename any duplicate shortcode names to avoid any conflicts.

See the [Shortcode Templates](https://gohugo.io/templates/shortcode-templates/) documentation.

## Using the Helpers

### figure

Create a caption and a longer description for an image, video, etc.

A caption appears immediately below the element, which can be expanded to reveal
a longer text description.

Input:
caption - A short description for the image. Should not duplicate the Alt text.
description (optional) - A longer description of the image with additional
                         detail.

Usage Example:
```
{{% figure
    caption="Apples are harvested in the fall."
    description="A photo of a boy climbing a ladder to pick ripe, red apples on
                 a tree. A older man is holding the ladder at the bottom. Both
                 of them are smiling. On the ground there is a large basket of
                 apples which have already been picked. There are 4 other apple
                 trees nearby. The sky is blue." %}}
    ![A photo of apples being picked at an apple orchard.](/images/apple.png)
{{% /figure %}}
```
## License

Copyright 2017 OCAD University, BSD 3-Clause License.
