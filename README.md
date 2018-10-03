# gusuku Customine Help

URL: [https://docs-customine.gusuku.io/](https://docs-customine.gusuku.io/)

## Requirement

Since we are using multilingual mode, you need hugo v0.32.4 or later.

```
$ hugo version
Hugo Static Site Generator v0.48 linux/amd64 BuildDate: 2018-08-29T06:33:51Z
```

You can get binary via [https://gohugo.io/](https://gohugo.io/).


## Content directory structure

Content will be created under markdown below the content directory.

* Japanese versions Action `list_add_checkbox` in the button category will create in `content/actions/button/list_add_checkbox.ja.md`
* This will deploy to [https://docs.gajumaru.io/ja/actions/button/list_add_checkbox/](https://docs.gajumaru.io/ja/actions/button/list_add_checkbox/).


```
content/
├── actions
│   ├── _index.en.md
│   ├── _index.ja.md
│   ├── aggregate
│   │   ├── _index.en.md
│   │   ├── _index.ja.md
│   │   ├── calc_records_average.en.md
│   │   ├── calc_records_average.ja.md
│   ...
└── conditions
    ├── _index.en.md
    ├── _index.ja.md
    ├── condition_event
    │   ├── _index.en.md
    │   ├── _index.ja.md
    │   ├── after_record_saved.en.md
    │   ├── after_record_saved.ja.md

```

## Create content

Follow the directory structure above to create directories and necessary files.
The file name ends with .md and it is written with markdown.

You can use marmaid to draw diagrams and a number of shortcuts for writing documents. See [https://themes.gohugo.io/theme/docdock/shortcodes/](https://themes.gohugo.io/theme/docdock/shortcodes/).


## Image installation location

Place images other than markdown files below "static".

For example, the image to be used in ``content/actions/button/add_button_at_header.ja.md`` is placed with the prefix of "images/ja/" and same path.

```
mkdir -p static/images/ja/actions/button/add_button_at_header/
```

Create a dedicated directory as described above and put it in it.

From the markdown side, you can write like below.

```
![Image description](/images/ja/actions/button/add_button_at_header/1.png)
```

## Shortcodes

You can use all shortcodes in [https://themes.gohugo.io/theme/docdock/shortcodes/](https://themes.gohugo.io/theme/docdock/shortcodes/).


## Preview

```
$ hugo server --disableFastRender
```

This command generates contents and the server starts up. Please check [http://localhost:1313/](http://localhost:1313/).
Since the live reload is attached, the browser side is automatically reloaded the moment you change markdown or setting.
