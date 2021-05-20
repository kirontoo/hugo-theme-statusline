# hugo-theme-statusline

[![GitHub](https://img.shields.io/github/license/mashape/apistatus.svg)](https://github.com/kirontoo/hugo-theme-statusline/blob/master/LICENSE)

A simple theme for Hugo based on a custom VIM statusline I created.

[Demo](https://hugo-statusline-theme.netlify.app)  

## Screenshots

![statusline-showcase](images/statusline-deepspace.png)

## Installation
Clone this repo into your `themes` folder.

If you're using git:
```bash
$ git submodule add https://github.com/kirontoo/hugo-theme-statusline.git themes/statusline
```

Otherwise, you can download the `.zip` file and extract it into your `themes` folder.

Remember to add the theme to your config file
```bash
$ echo theme = \"statusline\" >> config.toml
```

**Important:** Take a look inside the [`exampleSite`](https://github.com/kirontoo/hugo-theme-statusline/tree/master/exampleSite) folder of this theme. 
You'll find a file called [`config.toml`](https://github.com/kirontoo/hugo-theme-statusline/blob/master/exampleSite/config.toml). 
This is an example config of parameters  you can set.

**To use it, copy the [`config.toml`](https://github.com/kirontoo/hugo-theme-statusline/blob/master/exampleSite/config.toml) in the root folder of your Hugo site.**
```bash
$ cp ./themes/statusline/exampleSite/config.toml ./config.toml
```

## Front Matter

The [`themes/statusline/archetypes/default.md`](https://github.com/kirontoo/hugo-theme-statusline/tree/master/archetypes/default.md) file shows all of the available front-matter params.
If you want to customize it, copy this file in the `archetypes` folder at the root of your project and make your changes.

```bash
$ cp ./themes/statusline/archetypes/default.md ./archetypes/default.md
```

## Shortcodes

This theme provides various shortcodes for your markdown. See all of the available shortcodes [here](https://github.com/kirontoo/hugo-theme-statusline/blob/master/exampleSite/content/blog/shortcodes.md).

## Update The Theme

```bash
$ cd ./themes/statusline/
$ git pull
```

## Local Development
[comment]: # ( TODO )
You can use the `exampleSite` folder as a content source to make changes to this theme.
Just run the development server with:
```bash
$ hugo server --source=exampleSite --themesDir=../.. --disableFastRender
```

or use the Makefile

## Important Notes

### Instagram
The instagram API endpoint has been deprecated since October 24th, 2020. 
If you want to use the instagram shortcode, you must register your Hugo site as an app to get a Facebook API key.
See the issue [here](https://github.com/gohugoio/hugo/issues/7879).

### Config File
Hugo supports	`yaml`,	`toml`, and `json` config files.

### Profile Image
Your profile image can be placed in `static/images`.

### Projects Page
Only pinned projects will be shown. Make sure you have `pinned` set as `true` in the front-matter.
If you use the archetypes for projects, `pinned` is set to `true` on default.

### About Page
The about page will only show one content file. Make sure you create an `_index.md` in `content/about`.

## License

Released under the [MIT](https://github.com/kirontoo/hugo-theme-statusline/blob/master/LICENSE.md) License.
