# [Family Recipes](https://recipes.jackthomas.io)

The theme is [minima](https://github.com/jekyll/minima) with overrides provided in a few spots.

## Build Locally

The build is automated for the published website. If you want to run some local testing, it basically boils down to the following commands.

```
git clone git@github.com:jack-thomas/recipes.jackthomas.io
bundle exec jekyll serve
```

## Known Issues

- [Desserts > Quick Breads](https://recipes.jackthomas.io/categories/desserts/quick_breads) is not working as expected. Banana bread, pumpkin bread, and zucchini bread should all show up in this list but do not. It's definitely something in the [categories layout](_layouts/category.html), but I'm not sure what.
